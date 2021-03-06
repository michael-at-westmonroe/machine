# machine

This repository contains everything I need to quickly get a brand new machine ready for development.

After setting up a user account on an Apple machine, I login with that user and run the following
command in Terminal.app, there are prompts for information as it runs and a few manual steps to
be completed after:

```zsh
$ curl "https://raw.githubusercontent.com/michael-at-westmonroe/machine/master/install.sh" | zsh
```

Once complete I have the following on my machine:

1. XCode
2. Homebrew
3. Machine configuration files
4. Programs
    - zsh (latest)
    - [coreutils](https://www.gnu.org/software/coreutils/)
    - curl (latest)
    - git (latest)
    - gpg
    - vim (latest)
    - [rcm](https://github.com/thoughtbot/rcm)
    - [fzf](https://github.com/junegunn/fzf)
    - [ag](https://github.com/ggreer/the_silver_searcher)
    - [grc](https://github.com/garabik/grc)
5. Apps
    - Kitty (Terminal)
    - Firefox Developer Edition
    - Phoenix (window management)
    - Zoom
    - Slack
    - Microsoft Teams
6. Dotfiles
7. Colors
    - [Base16](https://github.com/chriskempson/base16-shell)
    - [grc](https://github.com/garabik/grc)
8. Fonts
9. SSH key

The following will need to be completed manually:

1. Set MacOS settings (i.e. tap to click, ctrl to capslock, etc)
2. Select default base16-shell theme (i.e. `$ base16_tommorrow-night`)
3. Generate gpg key `gpg --full-generate-key`
4. Set correct GPG key in `dotfiles/gitconfig` for signing commits
5. Upload public keys
6. Add `/usr/local/bin/zsh` to `/etc/shells` and `chsh -s /usr/local/bin/zsh`
