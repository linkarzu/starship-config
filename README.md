# Installation
To install starship go to the [main page](https://starship.rs ){:target="_blank"} and follow the instructions for your OS

## Linux using bash

Install the latest version
```bash
curl -sS https://starship.rs/install.sh | sh
```

Add this line to the end of your `~/.bashrc`
```bash
eval "$(starship init bash)"
```

## macos using zsh

Install the latest version
```bash
curl -sS https://starship.rs/install.sh | sh
```

Add this line to the end of your `~/.zshrc` file
- **Mine didn't exist so I had to create it**
```bash
eval "$(starship init zsh)"
```

# Change default config file location
Configuration changes are normally applied to the `~/.config/starship.toml` file, but since I have my file in github, I changed the default config file so that I can easily clone the repo to a new machine

I'll keep all my github repos in the `github` repo so I can just clone stuff in there. After cloning the repo there just run the following command so that the starship points to the cloned configuration
```apacheconf
export STARSHIP_CONFIG=~/github/starship-config/starship.toml
```