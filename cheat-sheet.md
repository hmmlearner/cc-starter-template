# Claude Code — Recovery Cheat Sheet
## Config won't load
- Run /config to confirm project settings are loaded
- Validate JSON: python -m json.tool .claude/settings.json
## A permission is blocking you
- Check the deny list in .claude/settings.json
- Widen an allow rule, e.g. Edit(src/**) -> Edit(**)
## Auth / login expired
- /status to check the account, then re-login via /login
## Roll back a bad change
- git diff to review, git checkout -- <file> to revert