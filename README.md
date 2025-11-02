# Mini Collatz Demo (Coq)

A minimal demonstration of the Collatz iteration and a small proof in Coq.

This repository contains one self‑contained Coq file that defines:

- the Collatz step function `step : nat -> nat`
- an iterator `iter : nat -> nat -> nat`
- a tiny 2‑adic counter `v2`
- a boolean termination test `term n := (n =? 1)`
- proofs that `27` hits `1` within `111` steps

## Files

- `mini_collatz_demo.v` — the code (compile this)
- `_CoqProject` — Coq project file
- `LICENSE` — MIT

## How to run

```bash
coqc mini_collatz_demo.v
```

You should see the `Compute` outputs and the lemmas closing.

**Tested with:** Coq ≥ 8.18

## Notes

This is intentionally tiny and didactic. Feel free to extend by
- adding more start values,
- turning the boolean checks into lemmas over `Prop`,
- or experimenting with other Lyapunov‑style measures.
