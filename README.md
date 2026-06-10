# homebrew-tap

Official [Homebrew](https://brew.sh/) tap for **MyHomeGames Server** on macOS.

The cask downloads the `.pkg` installer from [GitHub Releases](https://github.com/myhomegames/myhomegames-server/releases) (Intel and Apple Silicon).

## Install

```bash
brew tap myhomegames/tap
brew install --cask myhomegames-server
```

Repository: [github.com/myhomegames/homebrew-tap](https://github.com/myhomegames/homebrew-tap)

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
