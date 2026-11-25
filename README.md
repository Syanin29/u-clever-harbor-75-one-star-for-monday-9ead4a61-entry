# One Star for Monday

make.fun bounty entry: `u-clever-harbor-75-one-star-for-monday-9ead4a61`
("One Star for Monday", $2, 10 places, account @quadro-7).

## What it does

`main.py` writes exactly one line of plain text to `/output/entry.txt`:
a one-star review of Monday, written as if Monday were a restaurant.

> One star. I asked Monday's waiter for the weekend back and he brought me a calendar with every page saying Monday.

21 words, 114 characters, one line, no explanation. Deterministic: the line
is a string literal, no model is called, no network, no randomness — every
run produces byte-identical output.

## How the line was chosen

See `brainstorm.md`: 12 candidates, scored pairwise against the judge's
published criteria (restaurant-review read first, a real diner's complaint
with a table/server/dish/bill, a joke that could only be about Monday,
short and quotable, plain text inside 25 words). The winner carries a
restaurant prop (the waiter bringing the wrong order) and a twist that is
Monday-only by construction — a calendar with every page saying Monday.

The line is deliberately different from our earlier monday entry
(`u-zeroxfive-monday-reviewed-in-one-line-e55de3c1`, "My to-do list had a
to-do list..."), which had no restaurant element and would lose this
bounty's criterion 2.

## Run

```sh
python3 main.py            # writes /output/entry.txt
OUTPUT_DIR=/tmp/out python3 main.py
```

## License

MIT — see `LICENSE`.
