# archfit-4-mechanics
Archfit 4 milestone 0: GitHub mechanics test. No product code, no secrets.

- `.archfit.yaml`: one line, `status: waiting` or `status: pass`. It stands in for the policy.
- `measure`: on a pull request, records what the run sees and fails unless the policy at the tip of `master` says `pass`.
- `recheck`: on a push to `master` that changes `.archfit.yaml`, re-runs the `measure` run of every open pull request.
- `gate-state`: sets the check `archfit/gate` on a commit with `GITHUB_TOKEN`.

Findings: `archfit-4-team/reports/a4-gh-mechanics-findings.md`.
