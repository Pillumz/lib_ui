# Kirill's UI toolkit fork

This repository is `Pillumz/lib_ui`, the companion to `Pillumz/tdesktop`.
Its default branch is `omarchy`; ordinary fixes start from `origin/omarchy`.

- `origin` points to `https://github.com/Pillumz/lib_ui.git`. Push branches and
  open pull requests in that fork. Set the local GitHub CLI default to
  `Pillumz/lib_ui` when configuring a checkout.
- `upstream` points to `https://github.com/desktop-app/lib_ui.git` for fetching
  and comparison only. Its push URL is deliberately disabled; do not repair
  or bypass that protection. Never push or submit an upstream PR without
  explicit user approval.
- Preserve the opt-in translucent-window behavior and unchanged rendering
  when that option is off. Keep the toolkit generic: Omarchy palette mapping
  and desktop integration belong in `Telegram/build/omarchy` in the app repo.
- Publish library changes before updating the app's submodule pin. Do not
  replace the fork with an official revision or discard its patches during
  an upstream update. Integrating upstream is a deliberate, separate operation.
- Work in an agent-owned checkout, not the primary checkout. Follow the parent
  Telegram guide when this repository is used as its submodule. Use real GUI
  verification in app-sandbox; never test against a personal Telegram account.
