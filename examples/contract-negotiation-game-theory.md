MEMORANDUM: CONTRACT ANALYSIS FOR JORDY MICHAELS ENGAGEMENT
Client: Washington Unicorns
Subject: Advising on Which Contract Offer to Extend to Jordy Michaels
============================================================================

I. EXECUTIVE SUMMARY

The Unicorns should offer the CONTINGENT contract ($10 million, paid only
if Michaels plays). This contract yields a higher expected profit for the
Unicorns ($12.5 million vs. $11 million) AND -- critically -- solves an
adverse selection problem that the FOR SURE contract creates. Under the
FOR SURE contract, Michaels accepts in all scenarios, including the one
where he is permanently disabled and cannot play, leaving the Unicorns
paying $6 million for nothing. The CONTINGENT contract aligns incentives:
Michaels only gets paid when the Unicorns get value, and Michaels still
accepts in every scenario where he is able to play.

============================================================================

II. FRAMEWORK

This problem sits at the intersection of three analytical domains:

  (1) Decision Analysis -- structuring the Unicorns' choice under
      uncertainty using a decision tree and expected value calculations.
  (2) Game Theory / Information Asymmetry -- Michaels will know his health
      status (private information) before deciding whether to accept and
      play; the Unicorns will not. This creates an adverse selection problem.
  (3) Contract Design -- choosing a contract structure that allocates risk
      appropriately and aligns incentives between the parties.

============================================================================

III. SETUP: MICHAELS' THREE POSSIBLE HEALTH STATES

  State A: Reasonably Healthy (probability = 50%)
    - Can play unimpeded.
    - Playing is intrinsically worthwhile for Michaels (fan/media attention),
      so his minimum acceptable salary to play is $0.

  State B: Moderately Disabled (probability = 25%)
    - Can play but in significant pain.
    - Pain eliminates the enjoyment of playing and imposes treatment/emotional
      costs. He needs at least $2 million to offset these costs.
    - His minimum acceptable salary to play is $2 million.

  State C: Permanently Disabled (probability = 25%)
    - Cannot play at all, regardless of payment.

From the Unicorns' perspective:
    - If Michaels plays, the team earns $20 million in ticket/advertising
      revenue.
    - If Michaels does not play, the team earns $0 from this arrangement.

============================================================================

IV. ANALYSIS OF THE "FOR SURE" CONTRACT: PAY $6 MILLION REGARDLESS

Under this contract, Michaels receives $6 million whether or not he plays.

Step 1: Michaels' Decision in Each State

  State A (Healthy, 50%): Michaels receives $6M. Playing is worthwhile
  even for free, so he will play. Unicorns gain: $20M - $6M = $14M.

  State B (Moderate Disability, 25%): Michaels receives $6M regardless.
  If he plays, his net benefit = $6M - $2M (pain cost) = $4M.
  If he does not play, his net benefit = $6M - $0 = $6M.
  RATIONAL CHOICE: Michaels does NOT play. He collects $6M without
  enduring any pain. (This is a classic moral hazard problem -- the
  fixed payment eliminates the incentive to perform.)
  Unicorns gain: $0 - $6M = -$6M.

  State C (Permanently Disabled, 25%): Michaels cannot play.
  He collects $6M. Unicorns gain: $0 - $6M = -$6M.

Step 2: Michaels' Acceptance Decision

  Michaels will accept this contract in ALL states. In States B and C
  he gets $6M for doing nothing. In State A he gets $6M plus the
  enjoyment of playing.

Step 3: Expected Value for the Unicorns

  E[Profit | FOR SURE] = 0.50 x ($20M - $6M) + 0.25 x ($0 - $6M) + 0.25 x ($0 - $6M)
                       = 0.50 x $14M + 0.25 x (-$6M) + 0.25 x (-$6M)
                       = $7M + (-$1.5M) + (-$1.5M)
                       = $4M

  IMPORTANT NOTE ON MORAL HAZARD: The analysis above already accounts
  for Michaels' rational self-interest. In State B, he will NOT play
  because the $6M is guaranteed. The Unicorns lose money in both State B
  and State C.

  (Alternative calculation if we assumed Michaels plays in State B too --
  which he would NOT rationally do: 0.50 x $14M + 0.25 x $14M + 0.25 x
  (-$6M) = $7M + $3.5M - $1.5M = $9M. But this is wrong because it
  ignores Michaels' incentive structure.)

  CORRECTION -- Let me reconsider State B more carefully:

  Actually, we need to examine whether Michaels would play in State B
  more carefully. Under the FOR SURE contract, $6M is guaranteed. Playing
  costs him $2M in pain/treatment, yielding net $4M. Not playing yields
  $6M. He strictly prefers not playing. So the $4M calculation stands.

  Wait -- but we should also consider: could the contract REQUIRE him to
  play? If the contract says "pay $6M whether or not he plays," there is
  no contractual obligation to play. If it said "pay $6M, and he must
  play," then in State B he would play (since he can), but in State C he
  cannot. However, the problem states the contract is simply "pay $6M
  whether or not he plays," which implies no play obligation.

  But let me reconsider the problem from a different angle. As a
  practical matter, the FOR SURE contract likely contemplates that
  Michaels will play if he can. The question is: what rational behavior
  does each contract induce?

  Given the contract says payment is unconditional, there is no
  enforceable obligation to play. Michaels in State B would rationally
  choose not to play. Even if there were a "best efforts" clause, as
  the contracting framework notes, "best efforts" is essentially
  unenforceable because the team cannot verify the true degree of pain.

  Expected profit (FOR SURE) = $4 million.

============================================================================

V. ANALYSIS OF THE "CONTINGENT" CONTRACT: PAY $10 MILLION ONLY IF HE PLAYS

Under this contract, Michaels receives $10 million only if he plays.
If he does not play (by choice or inability), he receives $0.

Step 1: Michaels' Decision in Each State

  State A (Healthy, 50%): If he plays, he earns $10M plus the intrinsic
  enjoyment of playing. If he does not play, $0.
  RATIONAL CHOICE: Play.
  Unicorns gain: $20M - $10M = $10M.

  State B (Moderate Disability, 25%): If he plays, he earns $10M but
  incurs $2M in pain/treatment costs, for a net of $8M.
  If he does not play, he earns $0.
  RATIONAL CHOICE: Play (net $8M >> $0).
  Unicorns gain: $20M - $10M = $10M.

  State C (Permanently Disabled, 25%): He cannot play.
  Michaels earns $0. Unicorns pay $0.
  Unicorns gain: $0.

Step 2: Michaels' Acceptance Decision

  Michaels must decide before the season whether to sign. At the time of
  signing, he does not yet know his health state (the problem says these
  states will be known "in the summer, before the official season begins").

  If he must sign before knowing his state, his expected payoff is:
    0.50 x ($10M + enjoyment) + 0.25 x ($10M - $2M) + 0.25 x ($0)
    = $5M+ + $2M + $0 = $7M+
  This is clearly attractive; he would sign.

  If he signs after knowing his state:
    State A: Sign (gets $10M + enjoyment vs. $0). Yes.
    State B: Sign (gets $10M - $2M = $8M net vs. $0). Yes.
    State C: Sign or not, irrelevant (gets $0 either way). No reason to
             sign, but also no cost to the Unicorns.

  Either way, Michaels accepts and plays in States A and B.

Step 3: Expected Value for the Unicorns

  E[Profit | CONTINGENT] = 0.50 x ($20M - $10M) + 0.25 x ($20M - $10M) + 0.25 x ($0)
                         = 0.50 x $10M + 0.25 x $10M + 0.25 x $0
                         = $5M + $2.5M + $0
                         = $7.5M

============================================================================

VI. HEAD-TO-HEAD COMPARISON

  +-------------------+------------------+--------------------+
  |                   |   FOR SURE ($6M) |  CONTINGENT ($10M) |
  +-------------------+------------------+--------------------+
  | State A (50%)     |  Plays; +$14M    |  Plays; +$10M      |
  | State B (25%)     |  No play; -$6M   |  Plays; +$10M      |
  | State C (25%)     |  No play; -$6M   |  No play; $0       |
  +-------------------+------------------+--------------------+
  | Expected Profit   |       $4.0M      |       $7.5M        |
  +-------------------+------------------+--------------------+

The CONTINGENT contract dominates by $3.5 million in expected value.

============================================================================

VII. KEY INSIGHTS: WHY THE CONTINGENT CONTRACT IS SUPERIOR

1. SOLVES THE MORAL HAZARD PROBLEM

   The FOR SURE contract creates a moral hazard: because Michaels is paid
   regardless, he has no financial incentive to play when playing is
   painful (State B). The Unicorns pay $6M and get nothing.

   The CONTINGENT contract eliminates this moral hazard by tying payment
   to performance. In State B, Michaels now has a powerful $8M net
   incentive to play through the pain.

2. ELIMINATES THE ADVERSE SELECTION RISK

   Under the FOR SURE contract, Michaels accepts in every state --
   including the state where he is permanently disabled and the Unicorns
   receive zero value. This is a form of adverse selection: the contract
   is most attractive to Michaels precisely when it is most costly to the
   Unicorns (State C: he gets $6M for nothing).

   Under the CONTINGENT contract, the Unicorns pay $0 in State C. The
   contract self-selects: Michaels only earns money when the Unicorns
   also earn money.

3. RISK ALLOCATION IS APPROPRIATE

   The CONTINGENT contract shifts the risk of non-performance to Michaels
   (he gets $0 if he cannot play). This is appropriate because:
   (a) Michaels has superior information about his own health.
   (b) Michaels is the party whose actions and condition determine whether
       value is created.
   (c) The higher nominal amount ($10M vs. $6M) compensates him for
       bearing this risk.

4. THE HIGHER PRICE TAG IS MISLEADING

   The CONTINGENT contract appears more expensive ($10M vs. $6M), but the
   expected cost to the Unicorns is actually lower:
     FOR SURE expected cost: $6M (paid in all states)
     CONTINGENT expected cost: 0.75 x $10M = $7.5M (paid only if he plays)

   While expected cost is slightly higher under CONTINGENT, the expected
   REVENUE is dramatically higher ($15M vs. $10M) because Michaels plays
   in 75% of scenarios vs. only 50%.

5. MAKES THE PIE BIGGER

   The CONTINGENT contract creates more total value (consistent with the
   "make the pie bigger" principle of contract design):

     FOR SURE total surplus: $20M x 0.50 - $2M x 0 = $10M
     (Michaels does not play in State B, so the $20M revenue and the
     $2M cost are both avoided in that state.)

     CONTINGENT total surplus: $20M x 0.75 - $2M x 0.25 = $15M - $0.5M = $14.5M

   The CONTINGENT contract generates $4.5M more total value because it
   incentivizes Michaels to play in State B, where the value of his
   playing ($20M) far exceeds his pain cost ($2M).

============================================================================

VIII. SENSITIVITY ANALYSIS

What if the probability of each state changes?

Let p(A) = probability of healthy, p(B) = probability of moderate
disability, p(C) = probability of permanent disability.

  E[FOR SURE]    = p(A) x $14M + p(B) x (-$6M) + p(C) x (-$6M)
                 = p(A) x $14M - [p(B) + p(C)] x $6M
                 = p(A) x $14M - [1 - p(A)] x $6M
                 = p(A) x $20M - $6M

  E[CONTINGENT]  = p(A) x $10M + p(B) x $10M + p(C) x $0
                 = [p(A) + p(B)] x $10M
                 = [1 - p(C)] x $10M

CROSSOVER POINT (where FOR SURE = CONTINGENT):

  p(A) x $20M - $6M = [1 - p(C)] x $10M

With p(C) = 0.25 and p(A) = 1 - p(B) - 0.25:

  (0.75 - p(B)) x $20M - $6M = 0.75 x $10M
  $15M - p(B) x $20M - $6M = $7.5M
  $9M - p(B) x $20M = $7.5M
  p(B) x $20M = $1.5M
  p(B) = 7.5%

The FOR SURE contract only becomes competitive if p(B) drops below ~7.5%
(with p(C) held at 25%). Since the given p(B) = 25%, the CONTINGENT
contract is strongly favored.

More generally, FOR SURE beats CONTINGENT only when the healthy state is
overwhelmingly likely (above ~82.5%), making the moral hazard and adverse
selection problems negligible.

============================================================================

IX. ADDITIONAL CONSIDERATIONS

1. COULD A MODIFIED CONTRACT DO EVEN BETTER?

   Yes. A hybrid contract could capture even more value:
   - Pay $3M guaranteed + $7M if he plays.
   This gives Michaels some security (reducing risk aversion concerns)
   while still preserving the incentive to play in State B ($7M - $2M =
   $5M net gain from playing). The Unicorns' expected profit would be:
   0.50 x ($20M - $10M) + 0.25 x ($20M - $10M) + 0.25 x ($0 - $3M)
   = $5M + $2.5M - $0.75M = $6.75M. This is between the two options.

   However, the problem limits us to the two stated contracts.

2. MICHAELS' BARGAINING POWER

   In State B, under CONTINGENT, Michaels captures $8M net (which is
   generous). Under FOR SURE in State B, Michaels captures $6M without
   playing. The CONTINGENT contract is actually MORE generous to Michaels
   in States A and B ($10M vs $6M), which may make it easier to sell in
   negotiations.

3. VERIFIABILITY

   "Playing" is easily verifiable (Michaels is either on the roster and
   appearing in games or he is not), so the contingency is enforceable.
   This is a major advantage -- many performance-based contracts fail
   because the trigger is hard to verify, but this one is straightforward.

4. PUBLIC RELATIONS

   Paying a star player $10M "only if he plays" may appear harsh in the
   media. The Unicorns should frame it as a premium contract that reflects
   confidence in Michaels' ability to contribute, with the higher dollar
   figure ($10M vs. $6M) showing the team's valuation of his talent.

============================================================================

X. RECOMMENDATION

Offer the CONTINGENT contract ($10 million, contingent on Michaels
playing). This contract:

  - Yields expected profit of $7.5M vs. $4.0M for the FOR SURE contract
  - Solves the moral hazard problem (Michaels is incentivized to play
    in State B)
  - Eliminates adverse selection risk (no payment when Michaels cannot
    contribute)
  - Allocates risk to the party with superior information (Michaels
    knows his own health)
  - Creates more total value for both parties ($14.5M vs. $10M total
    surplus)
  - Is easily enforceable because "playing" is a verifiable condition

The CONTINGENT contract is superior on every relevant dimension of
contract design: expected value, incentive alignment, risk allocation,
and verifiability.

============================================================================
End of Memorandum
