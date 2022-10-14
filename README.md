# docker-laravel-template

## 開発環境構築

### Windows
#### パッケージマネージャ（Scoop）のインストール
1. Powershellで下記コマンドを実行
```shell
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
irm get.scoop.sh | iex
```

#### git, make のインストール
1. Powershellで下記のコマンドを実行
```shell
scoop install git make
```
#### PHPStorm のインストール
1. 下記のリンクから取得  
   [PhpStorm のダウンロード](https://www.jetbrains.com/ja-jp/phpstorm/download/#section=windows)

### Mac
#### パッケージマネージャ（homebrew） のインストール
1. ターミナルで下記のコマンドを実行
```shell
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
#### git, make のインストール
1. ターミナルで下記のコマンドを実行
```shell
brew install git make
```

#### PHPStorm のインストール
1. 下記のリンクから取得  
   [PhpStorm のダウンロード](https://www.jetbrains.com/ja-jp/phpstorm/download/#section=mac)

### 初回起動時
#### GitHub から Clone する
1. [Get from VCS] ボタンを選択
2. GitHub タブを選択
3. Log In via GitHub ボタンを選択
4. Authorize in GitHubボタンを選択
5. PHPStormに戻る
6. Shimaosを選択
7. Cloneを選択

#### 初回設定作業
1. PHPStrom の下部にある Terminalタブを起動
2. 下記のコマンドを実行する
```
make init
```

3. ブラウザを起動し、http://localhost へアクセスする

### 2回目以降
1. 右上にあるプルダウンから、docker-composeを選択
2. [Run ▶︎] ボタンを選択
3. Services タブにDockerの起動情報が表示されていることを確認
4. ブラウザを起動し、http://localhost へアクセスする
