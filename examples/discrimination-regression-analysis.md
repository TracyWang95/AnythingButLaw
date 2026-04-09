STATISTICAL ANALYSIS: JANE RENO GENDER DISCRIMINATION COMPLAINT AGAINST ISA
============================================================================

Regression Model:
  Salary = 4556.7 + 903.16(Sex) + 70.40(Education) + 75.40(Months) + 55.83(Age)

  Where: Sex (1=male, 0=female), Education (years beyond 8th grade),
         Months (months employed at ISA), Age (actual age minus 14)
  n = 125, R-squared = 0.603


QUESTION 1: PREDICTED SALARIES
-------------------------------

Profile: 23-year-old, 1st-year graduate student, 26 months at ISA.

Variable encoding:
  - Education: A 1st-year graduate student has completed 4 years of high school
    plus 4 years of college plus is in the 1st year of graduate school =
    9 years beyond 8th grade. Education = 9.
  - Months: 26
  - Age: 23 - 14 = 9

Male (Sex = 1):
  Salary = 4556.7 + 903.16(1) + 70.40(9) + 75.40(26) + 55.83(9)
         = 4556.70 + 903.16 + 633.60 + 1960.40 + 502.47
         = $8,556.33

Female (Sex = 0):
  Salary = 4556.7 + 903.16(0) + 70.40(9) + 75.40(26) + 55.83(9)
         = 4556.70 + 0 + 633.60 + 1960.40 + 502.47
         = $7,653.17

The predicted gender gap is $903.16 -- exactly the Sex coefficient. For two
employees who are identical in education, tenure, and age, the model predicts
that a male will earn $903 more per year than a female.


QUESTION 2: SIGNIFICANCE OF REGRESSION COEFFICIENTS
----------------------------------------------------

The t-statistic for each coefficient is computed as: t = coefficient / s.e.
With n = 125 observations and k = 5 parameters (4 predictors + intercept),
degrees of freedom = 125 - 5 = 120. The critical value for a two-tailed test
at the .05 level with 120 df is approximately 1.980.

Variable    | Coefficient |  s.e.  | t-stat  | Significant at .05?
------------|-------------|--------|---------|--------------------
Constant    |   4556.7    | 498.6  |  9.139  | YES
Sex         |    903.16   | 174.2  |  5.184  | YES ***
Education   |     70.40   | 150.7  |  0.467  | NO
Months      |     75.40   |  38.31 |  1.968  | NO (borderline)
Age         |     55.83   | 112.48 |  0.496  | NO

Results:
  - SEX is highly significant (t = 5.18, well above 1.98). After controlling
    for education, tenure, and age, sex has a statistically significant effect
    on salary. This is the core evidence for Ms. Reno's discrimination claim.

  - EDUCATION is not significant (t = 0.47). This is likely because the
    employee population at ISA draws from a narrow range -- university students
    and local high school students. There is limited variation in education
    levels, so the variable has little power to explain salary differences.
    Moreover, education may not be strongly rewarded at ISA given the nature
    of the work (linen service, cleaning, appliance rental, tutoring).

  - MONTHS is not quite significant at .05 (t = 1.97 vs. critical 1.98),
    though it is extremely close. In practical terms this is borderline.
    With a slightly larger sample or a one-tailed test, it would be significant.
    Months of tenure likely does matter for salary but the sample may not
    be large enough to detect the effect with precision at the conventional
    threshold.

  - AGE is not significant (t = 0.50). This is likely due to multicollinearity
    with the other variables. Age is correlated with both Education and Months
    of tenure -- older employees tend to have more education and more tenure.
    When these variables are all in the model, Age adds little independent
    explanatory power. Additionally, the workforce at ISA consists of young
    people (college and high school students), so the range of ages is narrow,
    further reducing the variable's explanatory power.


QUESTION 3: REGRESSION vs. SIMPLE MEAN DIFFERENTIAL
-----------------------------------------------------

The raw salary gap: Men average $9,620, women average $8,763.
Simple differential = $857/year.

Why regression is superior:

1. CONTROLLING FOR LEGITIMATE FACTORS. A simple mean comparison conflates all
   reasons for pay differences -- both legitimate (experience, education,
   tenure) and illegitimate (discrimination). The defendant will argue: "Men
   earn more because they have more experience or education, not because of
   their sex." A simple mean cannot rebut this argument.

   Regression separates these effects. By including Education, Months, and Age
   as control variables, the regression isolates the portion of the pay gap
   attributable to sex AFTER accounting for other factors. The Sex coefficient
   of $903.16 is actually LARGER than the raw differential of $857, suggesting
   that when you control for legitimate factors, the discrimination effect is
   even more pronounced. (This can happen if women on average have somewhat
   higher education or tenure than men in the sample.)

2. STATISTICAL SIGNIFICANCE TESTING. Regression provides standard errors and
   t-statistics, allowing a formal test of whether the sex-based gap could
   have arisen by chance. The t = 5.18 for Sex means the probability of
   observing this large a coefficient under the null hypothesis of no
   discrimination is extremely small (p < 0.001).

3. LEGAL PRECEDENT. In Bazemore v. Friday, 478 U.S. 385 (1986), the Supreme
   Court recognized multiple regression as an appropriate tool in employment
   discrimination cases precisely because it can control for confounding
   variables.

Alternative explanation:

Given what we know about ISA, there is a plausible alternative explanation that
should be considered. ISA was founded 6 years ago by 3 male undergraduates who
graduated from the university's law school and stayed on as salaried managers.
These founders are likely among the highest-paid employees. Their presence as
high-earning males may inflate the sex coefficient -- not because ISA
discriminates against women in general, but because the founding team happens
to be all male. If the founders' managerial salaries are substantially higher
than rank-and-file pay, this could drive much of the observed gap.

A defendant's attorney could argue this represents legitimate, non-
discriminatory factors: the founders are paid more because of their unique role,
seniority, and responsibility, not because of their sex. To test this, one
could re-run the regression excluding the 3 founders, or add a variable for
"founder/manager status."

Additionally, the model's R-squared is 0.603 -- meaning roughly 40% of salary
variation is unexplained. Omitted variables such as job type, position level,
performance, hours worked, or specific department could account for some of the
remaining gap. The omitted-variable-bias argument is the classic defense
strategy in discrimination litigation.


QUESTION 4: MANAGERIAL REPRESENTATION DATA
--------------------------------------------

Ms. Reno's additional data:
  - 44% of 130 managers are women (57.2 women managers)
  - 56% of employees are women
  - 52% of the local population is female

This data can support her case in two ways, but with different strengths:

(A) COMPARISON TO EMPLOYEE POOL (the stronger argument):

If 56% of ISA's employees are women, but only 44% of managers are women, this
suggests women are underrepresented in management.

To test significance, we use a z-test for proportions:
  - Sample proportion (p-hat) = 0.44 (proportion of female managers)
  - Population proportion (p0) = 0.56 (proportion of female employees)
  - n = 130 (number of managers)

  z = (p-hat - p0) / sqrt(p0 * (1 - p0) / n)
  z = (0.44 - 0.56) / sqrt(0.56 * 0.44 / 130)
  z = (-0.12) / sqrt(0.2464 / 130)
  z = (-0.12) / sqrt(0.001895)
  z = (-0.12) / 0.04354
  z = -2.756

The critical value for a two-tailed test at .05 is +/- 1.96. Since |z| = 2.76
exceeds 1.96, the underrepresentation of women in management is statistically
significant at the .05 level when compared to the employee pool.

This is the most relevant comparison because the employee pool is the natural
"applicant pool" from which managers are drawn.

(B) COMPARISON TO LOCAL POPULATION:

If 52% of the local population is female, but only 44% of managers are women:

  z = (0.44 - 0.52) / sqrt(0.52 * 0.48 / 130)
  z = (-0.08) / sqrt(0.2496 / 130)
  z = (-0.08) / sqrt(0.001920)
  z = (-0.08) / 0.04382
  z = -1.826

Since |z| = 1.83 is less than 1.96, this difference is NOT statistically
significant at the .05 level (two-tailed). However, it would be significant
at the .10 level.

This comparison is also less legally relevant because not all community members
are qualified for or interested in working at ISA.

ASSESSMENT:

The employee-pool comparison provides reasonably strong support for a promotion
discrimination claim. Women make up 56% of the workforce but only 44% of
management -- a 12 percentage point gap that is statistically significant.
Combined with the regression evidence of a $903 pay gap controlling for
education, tenure, and age, Ms. Reno has a reasonable statistical foundation
for both pay and promotion discrimination claims.

However, there are caveats:
  - We do not know whether the same factors that explain pay (education,
    tenure, age) also explain the management gap. Women employees might on
    average be newer or younger, which could partially explain their lower
    representation in management.
  - The 3 male founders holding management positions contribute to the skew.
    If we removed them (3 of 130 managers), the female proportion among the
    remaining 127 managers might be closer to parity.
  - A more rigorous analysis would use a logistic regression predicting
    promotion to management, controlling for tenure, education, and other
    qualifications, to see if sex remains significant.


OVERALL CONCLUSION
-------------------

Ms. Reno has two complementary pieces of statistical evidence:

1. REGRESSION ANALYSIS: A statistically significant sex coefficient of $903.16
   (t = 5.18, p < 0.001) shows that men earn substantially more than women
   even after controlling for education, tenure, and age. The model explains
   about 60% of salary variation.

2. REPRESENTATION DATA: Women are significantly underrepresented in management
   (44%) relative to their share of the workforce (56%), with z = -2.76
   (p < 0.01).

Together, these create a reasonable prima facie case of gender discrimination
in both compensation and promotion. The defense will likely argue omitted
variables (particularly job type and the unique status of the male founders)
and should be prepared to offer a regression with additional controls. The
strength of Ms. Reno's case will depend on whether the sex effect survives
when those additional variables are included.
