# GitHub topics

Topics are repository settings, not files. Add these in **Settings -> Topics** or
with the GitHub CLI when the repository is published.

```text
dota2
dota
dota-2
community-hub
documentation
overlay
configuration
windows
x64
source2
gaming
setup-guide
troubleshooting
ui-concept
assets
mit-license
fan-project
ancient-dota2
ancient
```

CLI equivalent:

```powershell
gh repo edit --add-topic dota2,dota,dota-2,community-hub,documentation,overlay,configuration,windows,x64,source2,gaming,setup-guide,troubleshooting,ui-concept,assets,mit-license,fan-project,ancient-dota2,ancient
```

Machine-readable copy: [`repo-metadata.json`](repo-metadata.json) and
[`spec.json`](spec.json).
