# Ruby

Ruby programming Language

## Installation

Ruby comes pre-installed in macOS, but this version of Ruby is outdated. It's necessary for Apple system Ruby scripts.

It's [advised to use Ruby version managers](https://snyk.io/blog/how-to-install-ruby-in-mac-os/).

### Versions

Recommended: [rbenv](https://github.com/nvm-sh/nvm#intro)

Other: rvm

Have (the `RUBY` and `RBENV` portions of my [.zshrc](https://github.com/NdagiStanley/dotfiles/blob/main/.zshrc)):

```sh
...
## RUBY
# Sets the Homebrew-installed Ruby to a higher priority than the system Ruby and adds the directory used for Ruby gems
...
## RBENV
if [ -d "/opt/homebrew/opt/rbenv/bin" ]; then
...
```

in your `.zshrc` or `.bashrc` (or equivalent) then install `rbenv`:

```bash
brew install rbenv ruby-build
```

Common commands:

```bash
rbenv versions
rbenv install 3.2.1
rbenv global 3.2.1
```

Further: running `rbenv local 3.0.5` creates a `.ruby-version` file specifying the default ruby version when you _cd_ into the directory.

## Implementation

Run:

```bash
ruby hello-world.rb
```

---
Ref:

- https://www.ruby-lang.org/en/
