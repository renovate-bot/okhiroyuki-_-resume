# resume

## 準備

- homebrew
- anyenv(rbenv/nodenv)
- ruby-build
- pre-commit

## Development

### pre-commit

```zsh
pre-commit install
```

### Ruby

```zsh
rbenv install
rbenv exec gem install bundler
rbenv rehash
bundle install
```

### Node.js

```zsh
nodenv install
```

## Build

```zsh
npm run build && npm run show
```
