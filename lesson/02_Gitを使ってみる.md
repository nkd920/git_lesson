# Gitを使ってみよう！
## この章でやること
GitHubを利用して実際にGitを使ってみましょう

### Gitのインストール、Githubアカウントの作成
#### 1.Gitのインストールしよう
本日はMacを利用するためすでにインストールされていますので、

Windowsにインストールする方法を記載しておきます。

##### Gitをインストールする
<span style="color:red">後ほどURLを記載します</span>

#### 2.GitHubのアカウントを作成しよう
<span style="color:red">後ほどURLを記載します</span>


### git helpでコマンドが引ける
以下のコマンドを打ってみましょう

    git help

利用できるオプション、機能が表示されます。

普段開発で利用する際は大体ここに載っているコマンドですので、
困ったら見てみると良いでしょう

    usage: git [--version] [--help] [-C <path>] [-c name=value]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p|--paginate|--no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

    The most commonly used git commands are:
       add        Add file contents to the index
       bisect     Find by binary search the change that introduced a bug
       branch     List, create, or delete branches
       checkout   Checkout a branch or paths to the working tree
       clone      Clone a repository into a new directory
       commit     Record changes to the repository
       diff       Show changes between commits, commit and working tree, etc
       fetch      Download objects and refs from another repository
       grep       Print lines matching a pattern
       init       Create an empty Git repository or reinitialize an existing one
       log        Show commit logs
       merge      Join two or more development histories together
       mv         Move or rename a file, a directory, or a symlink
       pull       Fetch from and integrate with another repository or a local branch
       push       Update remote refs along with associated objects
       rebase     Forward-port local commits to the updated upstream head
       reset      Reset current HEAD to the specified state
       rm         Remove files from the working tree and from the index
       show       Show various types of objects
       status     Show the working tree status
       tag        Create, list, delete or verify a tag object signed with GPG

    'git help -a' and 'git help -g' list available subcommands and some
    concept guides. See 'git help <command>' or 'git help <concept>'
    to read about a specific subcommand or concept.

もっと細かくHELP一覧がみたい！という方は以下のコマンドを叩いてみましょう

    git help config

vimで開くので、qキーで閉じましょう

それぞれの機能の詳細が知りたい！という方は、以下のコマンドを実行してみましょう

（add　の部分は詳細を知りたいコマンドに変更してみてください）

    git help -w add

### Gitの設定
#### 1. Gitの初期設定を行いましょう
    git config --global（user.nameとuser.emailを設定）
#### 2. メッセージカラーリングをつけよう
    git config --global color.ui true
#### 3. 設定を確認してみよう
    git config -l

### 各コマンドを使ってGitの設定から、GitHubにアップまでやってみよう
#### 1. gitで管理するフォルダの作成
    mkdir myproj
#### 2. 管理するフォルダへ移動
    cd myproj
#### 3. gitをつかいますよという設定
    git init
#### 4. コミットするファイルを作成
    vim index.html
#### 5. ファイルをgitの管理に追加する
    git add index.html
#### 6. ファイルが追加されていることを確認する
    git status
#### 7. コミットする
    git commit -m 'initial commit'
#### 8. コミットされたことを確認する
    git log
#### 9. GitHubにPushしてみよう
    git push

### 演習問題

1. myprojフォルダのgitへ、2nd.htmlを作成しコミット・プッシュしよう
* index.htmlフィアルを編集し、変更をコミット・プッシュしよう

