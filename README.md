# vibecook-dev/homebrew-tap

[Homebrew](https://brew.sh) formulae for [flux](https://github.com/vibecook-dev/flux),
a self-hosted media server.

```sh
brew install vibecook-dev/tap/flux
brew services start vibecook-dev/tap/flux     # now, and at every login
```

Then open <http://localhost:8096> and set flux up.

Use the full name, `vibecook-dev/tap/flux`: Homebrew's own `flux` is another
program (InfluxData's), as is fluxcd's, and neither can be installed beside
this one, since each installs a `flux` command.

`Formula/flux.rb` is written by flux's release workflow at each release
([`scripts/package/homebrew-formula.sh`](https://github.com/vibecook-dev/flux/blob/main/scripts/package/homebrew-formula.sh)):
change that script, not the formula.
