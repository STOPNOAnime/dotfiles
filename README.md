# Dotfiles
Repo for my dotfiles managed using chezmoi.

# Installation
```
curl -fsLS get.chezmoi.io/lb | CHEZMOI_SECRETS=1 sh -s -- init --apply stopnoanime
```

# Secrets
I store secrets on Bitwarden and acess them using `rbw`.
I'm using a `CHEZMOI_SECRETS` variable to conditionally update secrets to avoid entering the password on every `apply`.

To update the secrets just run `CHEZMOI_SECRETS=1 chezmoi apply`