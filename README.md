# この開発コンテナの作り方

1. 適当なフォルダを作成

```
mkdir ubuntu-go
```

2. vscode でフォルダを開く

3. `F1` でコマンドパレットを開く
 
4. 「add dev container」と入力し、 [Dev Containers: Add Development Container Configuration Files] (Dev Containers: 開発コンテナー構成ファイルの追加)を選ぶ。

5. Select a container configuration template から [Ubuntu] を選択する。

6. Ubuntu version で [jammy (default)] を選択。

7. Select additional features to install で [Go devcontainers] の チェックボックスをオンにして `OK`

-> devcontainer.json が作成される。

8. `F1` でコマンドパレットを開き、 [Reopen in Container] を選択する。

9. go がインストールされていることを確認

```
# go version
go version go1.19.4 linux/arm64
```

10. hello.go ファイルを作成して、実行してみる。

```go
package main

import "fmt"

func main() {
	fmt.Println("Hello, 世界")
}
```

```bash
# go run hello.go
```
