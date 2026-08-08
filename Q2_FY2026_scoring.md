# Q2 FY2026 Scoring — F1–F3 (F4 in a later addendum)

> SPX Technologies, Inc. (NYSE: SPXC) — engineered products company (HVAC + Detection & Measurement). Not the S&P 500 index (SPX).
>
> Reported figures used here are recorded in `Q2_FY2026_reported_figures.md` (committed 2026-08-02, before this scoring). Sources: 2026-07-30 press release; Form 10-Q filed 2026-07-31 (EDGAR 0000088205-26-000053); 2026-07-30 earnings call.
>
> **Read the "Defects" section first.** This record has four disclosed defects. They are published here rather than quietly fixed, because a preregistration record that hides its own failures is worth nothing.

## 1. Scoring

| # | Condition | Threshold (as written 2026-07-26) | Q2 FY2026 actual | Result |
|---|---|---|---|---|
| F1 | HVAC backlog organic growth, YoY | Fails if **below 30%** (prior reading +38%) | **+58.8% organic** ($918.8M total, less $61.4M Crawford and $0.8M Thermolec acquired backlog = $856.6M vs $539.5M) | **Not triggered** |
| F2 | FY2026 data center revenue guidance | Fails if **cut from $350M** | **Raised to $430M** (separately: ~$1.1B annual capacity at full production — capacity basis, not guidance) | **Not triggered** |
| F3 | HVAC segment income margin | Q1 FY2026 was −40bps YoY; fails if it **contracts again**, constituting two consecutive quarters of contraction | **22.8%**, −260bps YoY (Q2 FY2025: 25.4%). Sequential vs Q1's 22.5%: +30bps | **Triggered by its own terms — see 1.1 and 1.2** |
| F4 | Active-manager 13F direction | Fails if Capital Group **and** T. Rowe Price both turn net sellers (they moved in opposite directions in Q1) | Not yet scorable | 13F deadline 2026-08-14; addendum within 3 trading days |

### 1.1 F3 measurement-basis adjudication

The condition's wording mixes two bases: it anchors on a YoY figure ("Q1 FY2026 was −40bps YoY") and then says "contracts again versus the prior quarter." Two readings give opposite verdicts from the same 22.8%:

- **YoY basis:** Q1 contracted 40bps YoY; Q2 contracted 260bps YoY. Two consecutive quarters of contraction, deepening → **triggered**.
- **Sequential-level basis:** Q1 was 22.5%, Q2 is 22.8%, higher by 30bps → not triggered.

**Adjudicated: YoY basis, condition triggered.** Reason: the condition states its own baseline in YoY terms ("−40bps YoY"), and "two consecutive quarters of contraction" only counts consistently if both quarters are measured the same way. The sequential reading requires switching the measurement basis between the two quarters being compared, which is the kind of post-hoc reinterpretation this record exists to prevent. It is also the reading that favors the author's position, which is a reason for extra scrutiny, not less.

### 1.2 Rule conflict: F3 versus the B1/B2 carve-out — and why the outcome is not a clean PASS or FAIL

Two rules written before the earnings release cover this outcome, and they disagree:

- **F3** (failure condition, frozen 2026-07-26): two consecutive quarters of margin contraction invalidates the thesis; the plan's stated action on any failure condition is to exit.
- **B1/B2 carve-out** (standing rule in the author's project document, also pre-earnings): P&L second derivative negative *plus* order-book second derivative positive equals a capacity-investment phase and **does not count as thesis failure**.

Q2 satisfies both antecedents exactly: margin contracting (B1 negative, −260bps YoY) while backlog accelerates (B2 positive, +22% → +38% → +58.8%). The margin drivers disclosed in the 10-Q MD&A — capacity-expansion start-up costs and inefficiencies, net tariff headwinds, and a richer prior-year mix — were identified in the author's 2026-07-23 research baseline before the print (Section 232 impact of $0.05–0.10 EPS, ~75–80% concentrated in Q2 HVAC; ramp costs ~$8–9M for the year), so citing them is not post-hoc.

**Which rule takes precedence was never specified.** Applying the project document as written — where the B1/B2 carve-out is stated as a standing rule and explicitly says this combination "does not count as thesis failure" — the resulting action is **hold, labeled capacity-investment phase**.

Two things must be said about that conclusion:

1. **It is a post-hoc adjudication.** The precedence question was not answered before the result was known. It is being answered now, with the result visible.
2. **It is the conclusion that favors the author's position** (the position is currently profitable). And it exposes a design flaw: if a positive B2 always suspends F3, then F3 cannot trigger while backlog is accelerating, which is precisely the state the thesis predicts. **A condition that cannot fire in the expected state is not a failure condition.** F3 as written is therefore weaker than it appeared when frozen.

Recorded outcome: **F1 not triggered, F2 not triggered, F3 triggered on its own terms but suspended by the pre-existing B1/B2 carve-out; action taken: hold.** A reader who rejects the carve-out's precedence should read this record as F3 = FAIL with the preregistered action being exit. Both readings are given because the record does not support choosing one cleanly.

## 2. Defects in this record (disclosed, not corrected away)

**D1 — The numeric thresholds were not publicly frozen.** The three commits of 2026-07-23 (20:54, 21:23, 23:40 EDT) contain the condition categories, measurement bases, scoring commitment, and the FOMC-contamination exclusion, but the threshold cells are `[number]` placeholders. They were never filled before the release. The numbers scored above come from a private working record.

**D2 — The thresholds date to 2026-07-26, not 2026-07-23.** An earlier internal summary stated 2026-07-23. That is wrong and is corrected here: the earliest demonstrable existence of the four numeric thresholds is a private AI-assistant session record of **2026-07-26**, four days before the 2026-07-30 release. Evidence strength: a self-hosted session timestamp, screenshot-able by the author but not independently verifiable by a third party. The 2026-07-23 claim is contradicted by that day's own record, in which the conditions had not yet been quantified. So: the thresholds did exist before the result, and did not exist in the public record before the result.

**D3 — The thresholds were largely drafted by an AI assistant, not solely by the author.** This is the most consequential defect. A preregistration record is meant to test whether *the author's* judgment was locked before the outcome. To the extent the conditions were assistant-drafted from public baseline data, this record tests less than it appears to. It is published anyway, as a record of how the first attempt actually went.

**D4 — Two other stated facts were wrong and are corrected here.** (a) The scorecard's Section 2 said conditions were "formulated at entry (on or before 2026-07-20)"; that is false — see the position record below. (b) An internal summary dated the last preregistration commit to 2026-07-24; the git history shows all three commits on 2026-07-23.

**D5 — This scoring is late.** The commitment was publication within 3 trading days of the release (by 2026-08-04). The reported-figures record met that window (2026-08-02); this scoring did not, and is published 2026-08-06.

## 3. Position record (correcting the previously stated position)

The README stated a position of one share at $213.39. That was incomplete. The full record:

| Date | Type | Detail | Amount | Relative to thresholds (2026-07-26) |
|---|---|---|---|---|
| 2026-07-19 | market buy | 1 share @ $213.39 | $213.39 | before |
| 2026-07-22 | limit buy | 4 shares @ $214.00 | $856.00 | before |
| 2026-07-29 | market buy | 3 shares @ $201.08 | $603.24 | after |
| 2026-07-29 | market buy | 1 share @ $190.30 | $190.30 | after |
| | | **9 shares, average ~$207.0** | **$1,862.93** | |

Consequences for the record: the "conditions formulated at entry" claim is false for the first 5 shares and true for the 4 shares bought on 2026-07-29, which were purchased after the thresholds existed and before the result. Maximum drawdown exposure in a total-loss scenario is $1,862.93, not $213.39.

Per the preregistration, scoring uses reported fundamentals only; the post-earnings price reaction is deliberately excluded from the scoring above.

## 4. Next scheduled node

F4 addendum: Q2 13F filings are due 2026-08-14; scored within 3 trading days, comparing active managers against the Q1 baseline (Capital Group entities, First Trust, Wellington adding; Jane Street, T. Rowe Price, Goldman reducing), excluding passive index holders (Vanguard, BlackRock index, State Street, Geode).
