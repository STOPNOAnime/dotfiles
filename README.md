# Dotfiles
Repo for my dotfiles managed using chezmoi.

# Installation
1. Install Fedora, make sure to enable third party repositories.
2. Run chezmoi: `curl -fsLS get.chezmoi.io/lb | CHEZMOI_SECRETS=1 sh -s -- init --apply stopnoanime`
3. Login to Firefox, Bitwarden, Discord and VS Code

# Post installation tasks


# Secrets
I store secrets on Bitwarden and acess them using `rbw`.
I'm using a `CHEZMOI_SECRETS` variable to conditionally update secrets to avoid entering the password on every `apply`.

To update the secrets just run `CHEZMOI_SECRETS=1 chezmoi apply`
