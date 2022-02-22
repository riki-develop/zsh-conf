## ■概要  

### ・zshのカスタマイズ

①Homebrewでzshをインストール

```
/bin/zsh --version # デフォルトで入っているzshのバージョン
brew info zsh # Homebrewでインストールできるzshのバージョン

# Homebrewで入れる
brew install zsh

# 補完を強力にしてくれてるプラグインも
brew install zsh-completions zsh-autosuggestions zsh-syntax-highlighting
```

②ログインシェルをzshにする

```
# 現在のログインシェルを確認
echo $SHELL
```

↓

```
sudo vi /etc/shells
↓
# 下記を追記
/usr/local/bin/zsh
```

↓

```
# ログインシェル変更
chsh -s /usr/local/bin/zsh
```

③設定ファイルの作成

```
vi ~/.zshrc
```

↓

**zsh-confの設定を書き込む**

↓

```
source ~/.zshrc
```

で設定を反映させて完成！
