# nvim_config

### config ファイルを作成
```
mkdir -p ~/.config/
cd ~/.config/
git clone https://github.com/ekrecker/nvim_config.git
mv nvim_config/ nvim
```

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
