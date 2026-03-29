# Linux環境構築
# Linux環境構築する意味
**実際の開発・運用環境に近い状態で作業するため**
## 1. 本番環境がほぼLinux
- Webサーバー
- クラウド（AWS / Azure / GCP）
- Dockerコンテナ

ほぼ全部Linuxで動いている  
→**本番と同じ環境で開発できる**

## 2. コマンド・ツールが標準
Linuxでは以下が当たり前に使える：

- bash
- ssh
- apt
- grep / sed / awk

開発・インフラ・セキュリティすべてで使う

## 3. 開発ツールがLinux前提
代表例：

- Node.js
- Python
- Docker

Linuxの方がトラブルが少なく、動作が安定する

## 4. Windowsとの環境差異を減らせる
Windowsのみだと：

- パスの違い（\ と /）
- 改行コードの違い
- 権限管理の違い

バグの原因になる

## 5. WSLの強み
Windows + Linuxのハイブリッド環境：

- Windows：使いやすいUI
- Linux：開発環境

VSCode + WSL は現在の主流構成