# nethack-sandbox

nethackのsandboxです。

# sandbox構築方法

## 前提

* gitクライアントをインストールしておく
* dockerをインストールしておく

## gitまわり

```
git clone https://github.com/ino9dev/nethack.git
cd nethack
``` 

## dockerまわり

```
docker-compose up -d #しばらく待つ
docker exec -it nethack /bin/bash
root@baad54b18285:~# /usr/games/nethack
```

# その他

saveファイルはcloneのフォルダのsaveフォルダに保存されます。
docker-composeは既存のローカル環境を意識せずに書いているので、競合、不都合あれば適宜修正ください。

# 何かあれば

pull requestかissueでお知らせいただけると幸いです。
