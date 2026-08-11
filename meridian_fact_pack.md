# Meridian Business Bank — internal fact pack (SYNTHETIC test data)
You are modelling the Business Banking unit of Meridian Bank. These are the only
"internal actuals" available. Where a number you need is missing, do NOT invent it —
flag it, state your assumption explicitly, and carry a [low, high] band.

## Customers & segments
- Business customers: 45,000 · reachable business market: 300,000
- Relationship-managed share: 12% (larger/complex customers) · customers per RM: 90
- Annual customer churn: 10%

## Products held (penetration of customers · average balance/usage)
- Business current account: 100% · avg credit balance £14,000 · monthly fee £6 · net transaction income £90/account/yr
- Instant-access savings: 35% · avg £22,000 · rate paid 3.20%
- Fixed deposits (1yr): 10% · avg £60,000 · rate paid 4.30%
- Term loans: 9% · avg £180,000 · customer rate 6.40% · avg life 5 years · arrangement fee 1.2%
- Overdrafts: 20% · avg limit £12,000 · utilisation 40% · rate 9.50% · annual fee 1% of limit
- Business credit cards: 25% · avg spend £1,800/month · 20% of cards revolve avg £1,500 · APR 15.9% · card fee £30/yr
- International payments & FX: 15% of customers · avg £60,000 conversion/yr · 20 intl payments/user/yr @ £15 fee
- NOT offered: asset finance, invoice finance, merchant acquiring.

## Market & funding
- Bank Rate: 3.75% · term funding premium: +55bps
- Liquidity buffer 14% of deposits, yield give-up vs Bank Rate 0.9%
- Behavioural credit for stable non-maturing deposits: 45bps

## Credit risk & capital
- Term loans: PD 2.0% · LGD 30% · risk weight 65%
- Overdrafts: PD 2.8% · LGD 60% · risk weight 75%
- Cards: PD 4.0% · LGD 80% · risk weight 75%
- Op-risk RWA: 1.875 × gross income · CET1 target 13.5% · cost of equity 11.5% · tax 28%

## People (salaries; on-costs 14%; 150 productive hours/FTE/month)
- Relationship manager £58,000 · credit analyst £48,000 · service & ops £30,000 · team manager £75,000 · span of control 8

## Activity times (per unit)
- Onboarding (KYC+setup) 3.0h · BCA servicing 0.5h/acct/yr · savings/deposit servicing 0.15h/acct/yr
- Loan underwriting 12h/new loan · loan annual review 2.5h · overdraft renewal 1.2h
- Card servicing 0.1h/card/yr · payments/FX support 0.3h/user/yr
- Collections: 4% of facilities/yr enter collections · 5h/case
- Collateral administration: 0.8h/secured facility/yr

## Overheads & other (per customer/yr unless stated)
- Unit platform £50 · HQ technology £380 · HQ risk & compliance £210 · HQ corporate centre £220
- Fraud & APP losses £38 per BCA/yr · FSCS levy 0.05% on 55% of deposit balances protected
- Change-the-bank £100/customer/yr · premises £5,500/FTE · depreciation £1,000/FTE · other 5% of HR cost
- KYC onboarding £120/new customer · KYC refresh £50/customer/yr · payments processing £100/BCA/yr · core banking £25/account/yr · credit systems £150/facility/yr

## Known missing (deliberately not available)
- Commercial card interchange rate · recoveries/workout hours · RM time-split between sales and stewardship
