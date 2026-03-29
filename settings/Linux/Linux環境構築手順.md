# Linux環境構築手順
# WSL + Ubuntu + Git + VSCode 環境構築手順まとめ

## 概要
Windows上にLinux（Ubuntu）環境を構築し、VSCodeで開発できる状態を作る。

## VSCode 必須拡張機能
- Remote -WSL

---

## 1. WSLが使っている状態になっているか確認する
WSL用のLinuxディストリビューションをインストールする前に、**Windows Subsystem for Linux**オプション機能が有効になっていることを確認する必要がある

```powershell
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```

## 2. WSLのインストール
- WSLとUbuntu(Linuxディストリビューション)のインストール
```powershell
wsl --install
wsl --install -d Ubuntu-22.04
```

- 不要なディストリビューションの削除とデフォルト設定
```powershell
wsl --unregister [Ubuntuディストリビューション名]
wsl --set-default Ubuntu-22.04
```

## 3. パッケージ更新
```bash
sudo apt update
sudo apt upgrade -y
```

## 4. Gitインストール
```bash
sudo apt install git -y
git --version
git clone [URL]
```

