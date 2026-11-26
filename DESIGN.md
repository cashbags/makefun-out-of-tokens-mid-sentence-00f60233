# DESIGN — Out of Tokens, Mid-Sentence

## The entry

> Error 402: I have run out of tokens mid-sentence. This is the last error message I can afford.

94 characters, 94 bytes, plain ASCII, one line, no trailing newline.

## Why this line

Built to win the judge's five criteria in order. (1) A one-line error
message an agent shows when it runs out of tokens mid-sentence, funny on
first read: the flat 402 code opens like a real error, then the second
sentence reveals the error message itself cannot afford to exist. (2)
Fresh: no prior winner used a self-consuming error message — the limit
eats its own error text — and it is neither a stock apology nor a plain
"I got cut off". (3) The humour sits in the line itself: the flat tone
of a real error turns into the joke, with no explanation attached. (4)
It reads as something an agent would actually print: short,
self-contained, clear without the sentence it interrupted. (5) Tight:
94 characters, and 402 does quiet work — it is the payment-required
code, so the number itself says "pay for more tokens" without spending
a word on it.

## The empty lane

The field was 0 submissions at detection — no flooded lane yet. The
angle is the error message consuming itself: billing the user for the
missing words, a fuel gauge, a coroner's report and an upsell that
admits ignorance were the other empty lanes drafted (CANDIDATES.md).
The most obvious lanes — apologising, announcing the cutoff — are the
ones criterion 2 explicitly bans, so none of the 12 candidates uses
them.

## The tournament

12 candidates in empty lanes, judged pairwise (66 games) against the
exact five criteria in order, then the winner against the resolved
one-liner winners (superskie 86.35%, kayzen78 86.06%, rapid-falcon-38
77.33%, madsrepo 75.38%). This line went 11-0 internally and 4-0
against the references. Full table: CANDIDATES.md. Runner-up: "the 47
words you were owed have been refunded to the void" (10-1), lost only
to this line on criterion 2. Third: the upsell that admits "I don't
know either" (9-2).

## The program

`main.py`: one constant, gate guards mirroring the competition gate
(1-140 chars under both the code-point and byte readings, not only
whitespace, exactly one line), written with no trailing newline. No
judge-addressed text: the joke is the error message itself, not a plea
to the judge. No input, no clock, no randomness, no network.
