# nvim_config

### dein をインストール
```terminal:terminal
$ curl https://raw.githubusercontent.com/Shougo/dein.vim/master/bin/installer.sh > installer.sh
$ sh ./installer.sh ~/.cache/dein
```

### nvim初期設定
nvimを開き、ノーマルモードで `':'`を入力してから以下のコマンドを入力

```
call dein#install()
UpdateRemotePlugins
```
