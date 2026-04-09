MEMORANDUM

TO:      Bill (Senior Partner); Sheila (In-House Counsel, IMP)
FROM:    Associate
RE:      Decision Analysis of Paula Plaintiff's $1.1M Settlement Demand
DATE:    [Meeting Notes]

=========================================================================
I. BILL'S ANALYSIS AND WHERE IT GOES WRONG
=========================================================================

Bill's reasoning is as follows:

  - 50% chance plaintiff prevails on liability
  - If she prevails, "likely" damages = $1,000,000
  - Trial costs IMP = $50,000
  - Therefore expected cost of trial = (50% x $1,000,000) + $50,000 = $550,000
  - $550,000 << $1,100,000, so reject the demand

This analysis is INCOMPLETE. Bill has computed the expected value of trial
using only the "most likely" damages figure while acknowledging -- but then
dismissing -- a catastrophic tail outcome. A proper decision tree must
incorporate ALL material branches, weighted by their probabilities.

=========================================================================
II. THE CORRECT DECISION TREE
=========================================================================

The decision has two branches:

  BRANCH A: Accept Settlement
  -----------------------------------------------
  Cost to IMP = $1,100,000 (certain)

  BRANCH B: Reject Settlement and Go to Trial
  -----------------------------------------------
  Trial cost = $50,000 (certain, incurred regardless of outcome)

  Chance Node 1: Liability
    - IMP wins (no liability): probability = 50%  -->  Cost = $0
    - Plaintiff wins (liability found): probability = 50%  -->  go to Chance Node 2

  Chance Node 2: Damages (conditional on liability)
    - "Normal" compensatory damages only: probability = 90%  -->  $1,000,000
    - Enhanced compensatory + punitive damages: probability = 10%  -->  $25,000,000

  EXPECTED DAMAGES IF LIABILITY IS FOUND:
    = (0.90 x $1,000,000) + (0.10 x $25,000,000)
    = $900,000 + $2,500,000
    = $3,400,000

  EXPECTED COST OF GOING TO TRIAL (including trial costs):
    = $50,000 + (0.50 x $3,400,000)
    = $50,000 + $1,700,000
    = $1,750,000

=========================================================================
III. COMPARING THE TWO OPTIONS
=========================================================================

  Accept settlement:        $1,100,000
  Expected cost of trial:   $1,750,000

  Difference:               $650,000 in favor of ACCEPTING the settlement

Bill's error was treating the 10% catastrophic outcome as something to
"downplay." In decision analysis, you do not downplay low-probability,
high-magnitude outcomes -- you MULTIPLY them. That is precisely the
function of expected value calculation. A 10% chance of $25 million is
not a footnote; it contributes $2.5 million to the expected damages
(conditional on liability), which dwarfs the $900,000 contributed by the
90%-likely "normal" outcome.

=========================================================================
IV. WHY BILL'S INTUITIVE ERROR IS COMMON (AND DANGEROUS)
=========================================================================

Bill made two related cognitive mistakes:

1. ANCHORING ON THE MOST LIKELY OUTCOME: He focused on the $1M "likely"
   damages figure and treated the $25M scenario as a mere afterthought.
   Decision analysis requires that we weight ALL outcomes by probability,
   not privilege the modal outcome.

2. DOUBLE-DISCOUNTING THE CATASTROPHIC SCENARIO: Bill noted that the $25M
   outcome requires both (a) a liability finding (50%) AND (b) enhanced
   damages (10%), making it seem "remote." The combined probability is
   indeed only 5% (= 50% x 10%). But 5% of $25 million is $1,250,000 --
   which by itself exceeds the settlement demand of $1,100,000. A single
   tail outcome whose standalone expected value exceeds the settlement
   price is not "remote" in any economically meaningful sense.

=========================================================================
V. SENSITIVITY ANALYSIS
=========================================================================

Even if we question the estimates, the analysis is robust:

  Crossover Analysis: At what probability of the catastrophic outcome
  (conditional on liability) does the expected trial cost equal the
  settlement demand?

  Let p = probability of $25M outcome (conditional on liability).

  $50,000 + 0.50 x [(1 - p) x $1,000,000 + p x $25,000,000] = $1,100,000

  Solving:
    0.50 x [$1,000,000 + p x ($25,000,000 - $1,000,000)] = $1,050,000
    $1,000,000 + $24,000,000p = $2,100,000
    $24,000,000p = $1,100,000
    p = 1,100,000 / 24,000,000
    p = approximately 4.58%

  This means: as long as the probability of the catastrophic outcome
  (given liability) is above roughly 4.6%, the settlement is cheaper
  than trial. Bill himself estimates it at 10% -- more than double the
  crossover point. The settlement looks favorable across a wide range
  of reasonable assumptions.

  Even at a 5% catastrophic probability (half of Bill's own estimate),
  the expected trial cost would be:
    $50,000 + 0.50 x [(0.95 x $1,000,000) + (0.05 x $25,000,000)]
    = $50,000 + 0.50 x [$950,000 + $1,250,000]
    = $50,000 + $1,100,000
    = $1,150,000
  Still above the $1,100,000 settlement.

=========================================================================
VI. RISK AVERSION REINFORCES THE CONCLUSION
=========================================================================

The above analysis uses expected value, which assumes risk neutrality.
For a risk-neutral party (e.g., a large corporation that faces many
similar lawsuits and can "self-insure" across its portfolio), expected
value is the right metric.

However, if this is a uniquely large exposure for IMP, or if a $25M
judgment would cause reputational harm, trigger loan covenants, affect
stock price, or create negative precedent, then IMP may be risk-averse
in this context. A risk-averse party values a certain $1.1M loss as
LESS painful than a gamble whose expected value is $1.75M but which
includes a 5% chance of a $25M hit. The "certainty equivalent" of the
trial gamble for a risk-averse IMP would be HIGHER than $1.75M,
making the settlement even more attractive.

Key question for Sheila: How would a $25 million judgment affect IMP
beyond the dollar amount itself? If the answer involves material
collateral consequences, risk aversion further strengthens the case
for settlement.

=========================================================================
VII. ADDITIONAL STRATEGIC CONSIDERATIONS (GAME THEORY)
=========================================================================

1. PLAINTIFF'S "NONNEGOTIABLE" POSTURE: The $1.1M demand is framed as
   nonnegotiable. If this is credible, IMP faces a binary choice. If it
   is a negotiating tactic, there may be room to settle for less -- but
   the expected-value analysis shows that even at $1.1M, the settlement
   is a bargain relative to trial.

2. INFORMATION ASYMMETRY: Plaintiff may have private information about
   the strength of the punitive damages case. Her willingness to demand
   "only" $1.1M when the expected cost of trial is $1.75M suggests either
   (a) she is risk-averse herself, (b) she has litigation cost concerns,
   or (c) she is less confident about liability than Bill assumes. Any of
   these could create further negotiating room if IMP wanted to counter,
   but the fundamental point remains: at $1.1M, the settlement is below
   expected trial cost.

3. PRECEDENT AND SIGNALING: If IMP routinely faces similar claims,
   accepting a settlement may signal willingness to pay, inviting future
   claims. Conversely, going to trial and losing big could embolden
   future plaintiffs even more. This strategic dimension should be
   discussed but does not change the single-case expected-value math.

=========================================================================
VIII. RECOMMENDATION
=========================================================================

The $1.1 million settlement demand should be seriously considered and,
based on the numbers provided, ACCEPTED. The expected cost of trial
($1,750,000) exceeds the settlement by $650,000. The settlement is
favorable even if we halve Bill's estimate of the catastrophic damages
probability. Risk aversion, if applicable, only strengthens this
conclusion.

Bill's instinct to reject the demand was based on an incomplete expected
value calculation that ignored the outsized contribution of the low-
probability, high-magnitude punitive damages scenario. The correct
analytical framework -- a fully specified decision tree with all branches
weighted by probability -- shows that the plaintiff's demand is not
"ridiculous" but is, in fact, a discount relative to IMP's expected
trial exposure.

=========================================================================
IX. SUMMARY TABLE
=========================================================================

  Scenario                          Probability    Cost to IMP
  -----------------------------------------------------------------
  Accept settlement                 Certain        $1,100,000

  Trial: IMP wins                   50.0%          $50,000
  Trial: Liability + normal dmgs    45.0%          $1,050,000
  Trial: Liability + catastrophic   5.0%           $25,050,000
  -----------------------------------------------------------------
  Expected cost of trial            --             $1,750,000

  DIFFERENCE (Trial minus Settle)                  +$650,000

=========================================================================
END OF ANALYSIS
=========================================================================
