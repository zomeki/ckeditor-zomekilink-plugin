# ckeditor-zomekilink-plugin

CKEditor 4.3.0のlinkプラグインをカスタマイズしています。

## リポジトリ作成手順

ckeditor4をクローンします。

    $ git clone https://github.com/ckeditor/ckeditor4
    $ cd ckeditor4

4.3.0タグをmasterブランチにします。

    $ git pull --tags
    $ git checkout 4.3.0
    $ git branch -m master master.bk
    $ git checkout -b master

linkプラグインのみを残します。

    $ git filter-branch --subdirectory-filter plugins/link -- --all
