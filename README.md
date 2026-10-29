# PoC: PR headRefName -> run: command injection

Mirrors the final step of `.github/workflows/comments.yaml` in
ClickHouse/terraform-provider-clickhouse (issue_comment trigger).
The org-membership gate is stubbed to a static allow so a single actor can
exercise the primitive; the branch-name interpolation into `run:` is
byte-identical to the target.
