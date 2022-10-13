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
curl https://raw.githubusercontent.com/Shougo/dein.vim/master/bin/installer.sh > installer.sh
sh ./installer.sh ~/.cache/dein
```

### nvim初期設定
nvimを開き、ノーマルモードで `':'`を入力してから以下のコマンドを入力

```
call dein#install()
UpdateRemotePlugins
```

### エラーが出る場合
```
sudo apt install python3-pip
pip3でpython3-neovimをインストールする場合は次のようにする。
$ pip3 install neovim
```

# Zsh設定
- Zinit
  - https://github.com/zdharma-continuum/zinit#automatic-installation-recommended

### 補完
```
zinit light zsh-users/zsh-autosuggestions

zinit ice wait'0'; zinit light zsh-users/zsh-completions
autoload -Uz compinit && compinit

### 補完で小文字でも大文字にマッチさせる
zstyle ':completion:*' matcher-list 'm:{a-z}={A-Z}'

### 補完候補を一覧表示したとき、Tabや矢印で選択できるようにする
zstyle ':completion:*:default' menu select=1 
```

### シンタックスハイライト
```
zinit light zsh-users/zsh-syntax-highlighting
```

### 履歴
```
zinit load zdharma/history-search-multi-word
```

### Color Theme
```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
```
