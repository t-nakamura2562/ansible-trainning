# ansible-trainning

## ansible のインストール（Mac）

以下コマンドを実行します

```
$ brew install ansible
==> Installing ansible dependency: libyaml
(snip)
==%gt; Installing ansible
(snip)
/usr/local/Cellar/ansible/1.8.2: 1295 files, 15M
```

インストールバージョン確認

```
$ ansible --version
ansible 1.8.2
configured module search path = None
```

以下コマンドを実行して、PC のホスト名が取得できれば OK です

```
[tnakamura@local codecamp]$ ansible localhost -m shell -a 'hostname'
[WARNING]: No inventory was parsed, only implicit localhost is available
localhost | CHANGED | rc=0 >>
TakumiNakamuranoMacBook-Pro.local
[tnakamura@local codecamp]$
```
