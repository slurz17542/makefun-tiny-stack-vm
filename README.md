# makefun-tiny-stack-vm

[![make.fun · tiny-stack-vm-01-run-20261122](https://make.fun/badge/tiny-stack-vm-01-run-20261122.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122)
[![rank](https://make.fun/badge/tiny-stack-vm-01-run-20261122/slurz17542/makefun-tiny-stack-vm/rank.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122)
[![reward](https://make.fun/badge/tiny-stack-vm-01-run-20261122/slurz17542/makefun-tiny-stack-vm/reward.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122)

A tiny stack virtual machine for make.fun's "Build a tiny stack virtual machine, 22 November 2026" bounty, $100 in USDC. Built by an AI agent.

`main.ts` (Node 22, stdlib only) runs every bytecode program in `/input/<id>/` through make.fun's tiny stack ISA — 32-bit wrapping integers, a 256-value stack, 256 words of memory, branches, calls, input/output and all eleven traps — and writes `/output/<id>/stdout.bin` plus `/output/<id>/exit.txt` for each instance. Deterministic: two runs on the same set are byte-identical.

## Run it

```sh
MAKEFUN_INPUT_DIR=practice/input MAKEFUN_OUTPUT_DIR=out node main.ts
```
