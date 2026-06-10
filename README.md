# homebrew-tap

Official [Homebrew](https://brew.sh/) tap for **MyHomeGames Server** on macOS.

The cask downloads the `.pkg` installer from [GitHub Releases](https://github.com/myhomegames/myhomegames-server/releases) (Intel and Apple Silicon).

## Install

```bash
brew tap myhomegames/tap
brew trust myhomegames/tap
brew install --cask myhomegames-server
```

Repository: [github.com/myhomegames/homebrew-tap](https://github.com/myhomegames/homebrew-tap)

### Untrusted tap (Homebrew 5.x+)

Third-party taps are not trusted by default. If install fails with:

```text
Error: Refusing to load cask myhomegames/tap/myhomegames-server from untrusted tap myhomegames/tap.
```

trust the tap once (same machine):

```bash
brew trust myhomegames/tap
```

Or only this cask:

```bash
brew trust --cask myhomegames/tap/myhomegames-server
```

Then run `brew install --cask myhomegames-server` again.

### Apple Silicon (M1/M2/M3)

Use native Homebrew (`/opt/homebrew/bin/brew`), not the Intel install under `/usr/local`, so the cask installs the **arm64** `.pkg`. Check with `brew config`: `HOMEBREW_PREFIX` should be `/opt/homebrew` and macOS should show `arm64`, not `x86_64`.

After installation, open **MyHomeGames** from `/Applications`. Default configuration:

```
/Applications/MyHomeGames.app/Contents/Resources/.env
```

Web app: [myhomegames.vige.it/app/](https://myhomegames.vige.it/app/)

## Upgrade

```bash
brew update
brew upgrade --cask myhomegames-server
```

## Uninstall

```bash
brew uninstall --cask myhomegames-server
```

## Without Homebrew

Download the `.pkg` from [releases](https://github.com/myhomegames/myhomegames-server/releases). Use `mac-arm64` on Apple Silicon and `mac-x64` on Intel.

## Links

- [myhomegames-server](https://github.com/myhomegames/myhomegames-server)
