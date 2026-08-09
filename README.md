# Dot Files

My personal dotfiles, managed with [chezmoi](https://www.chezmoi.io).

## Setup

### 1. Install chezmoi

```bash
brew install chezmoi
```

Not on macOS? See [other install methods](https://www.chezmoi.io/install/).

### 2. Pull and apply the dotfiles

```bash
chezmoi init --apply https://github.com/KaySum/dotfiles.git
```

You will be prompted for each machine-specific value the dotfiles need — currently your
git name and email. The answers are yours, not mine: they are saved to
`~/.config/chezmoi/chezmoi.toml` on your machine and never end up in this repo.

### 3. Confirm it worked

```bash
chezmoi status          # no output means everything is applied
chezmoi data            # shows the values you were prompted for
```

## Staying up to date

```bash
chezmoi update          # pull the latest changes and apply them
```

## Making it your own

The steps above track my repo, so you have no push access and your own edits go nowhere.
To take it further, fork it and run step 2 against your fork's URL instead.
