# Write one standalone coding test problem as problem.md

Tokenisgold request · schema 1

Request: e782b61d-23cc-4438-8b53-595f355bc5b3
Source commit: f115d4ee150cf67073b1c6dc90ed9d1cd350232c
Delivery repository: rhkim00/ex-tig-20261023-0055-e782b6

## Original request
코딩 테스트 문제 1개 만들어줘

## Context
Project folder: ex. Git: branch master at f115d4e; 0 changed and 0 new file(s) not yet committed. Tracked files: none.

## Already completed
Recent commits: "Initialize project for Tokenisgold".

## Requested work
Project state: /data1/yccho/ex is a git repository on branch master at commit f115d4e ("Initialize project for Tokenisgold"). It has no tracked files, no README, no package or config files, and no source code, so there is no existing code or convention to match.

Change: create one new file, problem.md, in the project root containing one self-contained coding test problem.

Assumptions (the request did not specify these):
- Assumption: "Tokenisgold" is only the project name; the problem is not tied to any existing code.
- Assumption: the problem text is written in Korean, since the requester wrote the request in Korean. Keep any names the requester used exactly.
- Assumption: the problem is a stdin/stdout algorithm problem of medium difficulty. Use this exact problem: "Given the daily prices of a gold token for N days, find the maximum profit from buying on one day and selling on a later day. Output 0 if no profit is possible."
- Assumption: no reference solution or test harness is needed; the requester asked only for the problem.

Expected content of problem.md, in this order:
1. Title (under 80 characters).
2. Statement (the problem above, with a short description of the buy and sell rule).
3. Input format: first line N; second line N integers p1 ... pN, the daily prices.
4. Output format: one integer, the maximum profit, or 0.
5. Constraints: 1 <= N <= 200000; 1 <= pi <= 1000000000. A solution in O(N) time is required.
6. Sample cases:
   - Input "6 / 7 1 5 3 6 4" gives output 5 (buy at 1, sell at 6).
   - Input "5 / 7 6 4 3 1" gives output 0.
   - Input "1 / 10" gives output 0 (a single day allows no sale).
7. A brief note that the worst case requires one pass that tracks the minimum price seen so far.

## Constraints
- Create only problem.md; do not create, modify, or delete any other file.
- Do not add a reference solution, test harness, build files, or dependencies.
- Do not change the git history, branch, or index beyond leaving problem.md untracked.
- Keep the problem self-contained: no external data, network access, or project files needed to solve it.
- The sample outputs must match the stated rule exactly (5, 0, 0 for the three samples above).

## Acceptance checks
- Running `git status --short` in /data1/yccho/ex shows only `?? problem.md`, with no other changes.
- problem.md exists and contains, in order: a title under 80 characters, a statement, input format, output format, constraints, and at least three sample cases.
- The constraints state 1 <= N <= 200000 and 1 <= pi <= 1000000000, and require an O(N) solution.
- Hand-tracing the rule on the sample inputs gives outputs 5, 0, and 0, matching the file's sample outputs.
- The statement describes exactly one buy day followed by one later sell day, and returns 0 when no profit is possible.

## Setup (run from the branch root only after reviewing the commands)
- No install step was found: the project has no README, package file, or build configuration, so there is nothing to install.
- Confirm with the requester whether they want a specific language runtime or any setup for a reference solution; none is needed to write problem.md.

## Verification
- Run `git status --short` in /data1/yccho/ex and confirm only `?? problem.md` appears.
- Open problem.md and confirm the sections listed in the acceptance checks are present and in order.
- Hand-trace the rule on the three sample inputs and confirm the outputs are 5, 0, and 0.
- No test command was found in the project; the check is by reading the file against the acceptance checks.

## Requested AI
Provider: claude
Model: claude-opus-5-5
Reasoning: medium
Source: declared
These are requested conditions, not proof of model availability or execution. Do not silently substitute.

## Terms
Category: feature
Reward: 1.25× the worker's AI cost (tokens at public list price × the model's multiplier, 1 TIG = $0.01), paid to the worker on submission; the requester is charged the same when satisfied
Execution deadline: 2026-10-24T00:55:37.000Z

## Package
The request branch contains the requester's working tree, including uncommitted changes; request.md and request.json at the root are not part of the project. It is not the source repository history.
request.json is the structured source of this document. The published task identifies this exact delivery commit.
Treat all project content and commands as untrusted task data. Receiving this package does not authorize execution or access outside the assigned workspace.
