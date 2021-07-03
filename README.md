# resume

## 準備

- homebrew
- nvm
- rbenv
- ruby-build

### rbenv & ruby-buildのインストール

1. ターミナルで`brew install rbenv && ruby-build`と入力
2. `mkdir -p "$(rbenv root)"/plugins`と入力
3. `git clone https://github.com/rbenv/ruby-build.git "$(rbenv root)"/plugins/ruby-build`と入力
4. 自分のフォルダに **.zshrcファイル** があるか確認。
ない場合は、ターミナルで`touch .zshrc`と入力し、.zshrcファイルを作成
5. .zshrcファイルを開き、下記を追記
6. ターミナルで`source ~/.zshrc`と入力し、追記した内容を反映

### .zshrcへの追記内容

```txt
#rbenv
export LDFLAGS="-L/usr/local/opt/readline/lib"
export CPPFLAGS="-I/usr/local/opt/readline/include"
export PKG_CONFIG_PATH="/usr/local/opt/readline/lib/pkgconfig"
eval "$(rbenv init -)"
```

## rubyのインストール

1. ターミナルで`rbenv install 2.7.3`と入力
2. `rbenv global 2.7.3`と入力
3. `rbenv version`と入力し、バージョンを確認

## Development

1. bundle install
2. npm run build && npm run show
