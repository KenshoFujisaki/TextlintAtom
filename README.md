# TextlintAtom
[Atom]("https://atom.io/")で[textlint]("https://github.com/textlint/textlint")を使うためのインストール手順です。プラグインに[linter-textlint]("https://github.com/1000ch/linter-textlint")を用います。

## インストール手順
#### 1. `Node.js`および`npm`のインストール
* Windowsの場合
    1. [chocolatey]("https://chocolatey.org/")で`Node.js`をインストールします。
```sh
choco install nodejs.install
```
* Mac OS Xの場合  
    1.  [anyenvで開発環境を整える]("http://qiita.com/luckypool/items/f1e756e9d3e9786ad9ea")にしたがって`ndenv`をインストールします。
    2. 以下を実行し、`Node.js`のバージョンを`v5.0.0`に変更します。
```sh
ndenv install v5.0.0
ndenv global v5.0.0
ndenv rehash
```

#### 2. `textlint`および`textlint-rule-*`のインストール
```sh
cd [本READMEがあるディレクトリ]
npm install -g textlint
npm install
```
[!] Windowsの場合は`PowerShell`、Mac OS Xの場合は`Bash`で実行してください。

#### 3. `linter-textlint`のインストール
```sh
apm install linter-textlint # Atom内からのpackage installでもOK
```
[!] Windowsの場合は`PowerShell`、Mac OS Xの場合は`Bash`で実行してください。

## インストール確認
1. atomで本READMEを開く
```
cd [本READMEがあるディレクトリ]
atom .
```
[!] プロジェクトとして開く必要があるのでご注意ください。

2. エラー確認  
正しくインストールができた場合、この行でエラーメッセージ、「一つの文で"、"を3つ以上使用しています」が表示されます。
![インストール確認](./img/check_install.png)
