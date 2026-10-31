# repo-settings-trial

standards#132 の確かめ用のリポ。確かめ終わったらアーカイブする。

## Tech Stack

- branch_policy: `unprotected`（2026-10-31 実測: ruleset 0 本、branch protection なし。この PR のマージのあとに ruleset を入れて確かめる）
- merge_policy: auto-on-green
- deploy_branch: production
- deploy_policy:
  - `production`: human（本番）
  - `verify`: auto-on-green（検証用）。理由: 試しのリポで、利用者に届かないため
