---
title: Tiny Core Linux用のJDK11 TCZパッケージを作る
---

# Tiny Core Linux用のJDK11 TCZパッケージを作る

Tiny Coreは正式のJDKビルドを提供しません。Tiny Core 10用のjava-installer.tczはOpenJDK 11で使いません。Tiny Coreの過去バージョンも同じです。下記のGibHubリポジトリのDockerスクリプトを利用しOpenJDK tar.gz パッケージからjdk11.tcz作るこたができます。

1) hpmtissera/tinycore-jdk11-tcz リポジトリをクローンする。

   https://github.com/hpmtissera/tinycore-jdk11-tcz.git

2) OpenJDK11のtar.gzファイルをhttps://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases　からダウンロドしtinycore-jdk11-tczフォルダ中にコピーします。

```
ex. OpenJDK11U-jdk_aarch64_linux_11.0.4_11.tar.gz
```

3) build.sh スクリプトを実行します。 

```bash
./build.sh
```

4) スクリプトでjdk11.tczパッケージを作成されます。
