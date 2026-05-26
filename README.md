# [YzのRepositories](https://github.com/Yz-Filer)  

> [!NOTE]  
> `https://yz-filer.github.io/Yz-Filer/`のURLが表示されていて表示が崩れてる場合は、上記リンクからオリジナルページ`https://github.com/Yz-Filer`にアクセスして下さい。  

## 1. Yz-Filer  

### 1. [Yz-Filer Ver.2](https://github.com/Yz-Filer/Yz-Filer/blob/master/Yz-Filer.md)  

![](image/DarkNavy2.png)  

キー操作系ファイラーのFD、FILMTN、WinFMっぽいSFTP/SCP対応のタブ型ファイラーです。  
C#言語で作成したWindows対応版となります。  

### 2. Yz-Filer Ver.3  

キー操作系ファイラーのFD、FILMTN、WinFMっぽいSMB/SCP対応のタブ型ファイラーです。  
Go言語 + GTK3で作成したLinux対応版となります。  

> [!NOTE]  
> Windows版も同梱してますが、gtk3の制約でDrag & Dropが出来ないなどの機能制限があります。  

[ここ](bin/Yz-Filer_3.0.zip)
に置いてます。 

### 3. Yz-Filer Ver.3.1

キー操作系ファイラーのFD、FILMTN、WinFMっぽいSMB/SCP対応のタブ型ファイラーです。  

- [vector](https://www.vector.co.jp/soft/data/util/se523591.html)
- [GitHub Releases](https://github.com/Yz-Filer/Yz-Filer/releases)  

Go言語 + GTK3で作成したLinux/Windows対応版となります。  
[go言語 & gotk3をちょっとやり直してみたい](https://github.com/Yz-Filer/golang)  で確認した内容を取り込んで、Windows版もDrag & Dropに対応しました。

<img src="image/yz3.1_window1.png" width="40%" /> <img src="image/yz3.1_window2.png" width="40%" />  

gtk3を使ってるため、Ver.3から上図のように、テーマをカスタマイズすることで、半透明や背景画像の指定も出来るようになりました。  

> [!NOTE]
> 詳細は、[3. テーマを使いたい](https://github.com/Yz-Filer/golang/tree/main/Contents/03)を参照

Ver.3からVer.3.1への主な変更点は以下の通りです。

- Window環境でファイルエクスプローラーとのDnDおよびクリップボード経由でのファイルのコピー&ペーストに対応しました。
（DnDは「Shiftキー + Drop」でMove、「Ctrlキー + Drop」でCopyとなります）

- Windows環境でローカルファイルの右クリックメニューにエクスプローラーの右クリックメニューを表示するように変更しました。（一部表示されないサブメニューがあります）

- 機能には関係ないですが、リソースを埋め込んだのでgladeファイルが不要になりました。

- 機能的には大きく変わってませんが、文字コード変換、USBディスク監視、ディレクトリ監視を「[go言語 & gotk3をちょっとやり直してみたい](https://github.com/Yz-Filer/golang)」の内容に変更しました。  

- 画像ビューアは、範囲指定、コピー(Ctrl + C)、ペースト(Ctrl + V)、背景色の変更に対応しました  
<img src="image/yz3.1_ImageViewer.png" width="40%" />  

- USBディスクを使用不可にしている端末では起動出来なかったため、USBディスク監視をOFFにするコマンドラインオプションを追加しました。起動時に「--no-usb-watcher」を引数に指定すると、ドライブスキャンおよびUSBディスク監視が行われなくなります。
（「C:\」などが初期表示されないため、必要に応じて「F7キーコマンド」で登録して下さい）


## 2. [go言語 & gotk3をちょっとやり直してみたい](https://github.com/Yz-Filer/golang)  

![](image/window.jpg)  

Yz-Filer作成時に調べきれなかった事とかがあったので、GeminiとWEB検索を利用して調べ直したメモです。  

- 他のPCで動作させる方法、テーマを使う方法  
- タスクトレイ常駐、いくつかのコントロール、カスタムシグナル、書式設定、クリップボード、USBドライブイジェクト、ディレクトリ監視、Drag and Drop、文字コード判定  
- 付箋アプリ、簡易メモ帳アプリ、画像ビューアアプリ  

などを記載してます。  

## 3. [Yz-VideoEffect / Yz-ImageEffect](https://github.com/Yz-Filer/Yz-VideoEffect)  

<img src="image/sk_kanazawa_org.jpg" width="40%" /> <img src="image/sk_kanazawa.jpg" width="40%" />  

写真や動画をエッジ、2値化、3値化、水彩画風、黒板アート風、スケッチ風、アニメ風に変換するツールです。  

## 4. [OfficeShapeTool](https://github.com/Yz-Filer/OfficeShapeTool)  

![](image/hdl6.gif)  

Microsoft OfficeのPowerPoint形式（Office Open XMLのプレゼンテーション形式）で保存された図形に「接続ポイント」と「調整ハンドル」を追加するツールです。  
「図形の結合」機能とあわせて使うとオリジナルの図形が作成できます。  

[1. はじめに](https://github.com/Yz-Filer/OfficeShapeTool#1-%E3%81%AF%E3%81%98%E3%82%81%E3%81%AB)  
[2. 作成例](https://github.com/Yz-Filer/OfficeShapeTool#2-%E4%BD%9C%E6%88%90%E4%BE%8B)  
[3. インストール・設定](https://github.com/Yz-Filer/OfficeShapeTool#3-%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB%E8%A8%AD%E5%AE%9A)  
[4. カスタム図形への接続ポイントと調整ハンドル追加](https://github.com/Yz-Filer/OfficeShapeTool#4-%E3%82%AB%E3%82%B9%E3%82%BF%E3%83%A0%E5%9B%B3%E5%BD%A2%E3%81%B8%E3%81%AE%E6%8E%A5%E7%B6%9A%E3%83%9D%E3%82%A4%E3%83%B3%E3%83%88%E3%81%A8%E8%AA%BF%E6%95%B4%E3%83%8F%E3%83%B3%E3%83%89%E3%83%AB%E8%BF%BD%E5%8A%A0)  
[5. 画像への接続ポイント追加](https://github.com/Yz-Filer/OfficeShapeTool#5-%E7%94%BB%E5%83%8F%E3%81%B8%E3%81%AE%E6%8E%A5%E7%B6%9A%E3%83%9D%E3%82%A4%E3%83%B3%E3%83%88%E8%BF%BD%E5%8A%A0)  
[6. 回転移動と放射移動（polar調整ハンドル）](https://github.com/Yz-Filer/OfficeShapeTool#6-%E5%9B%9E%E8%BB%A2%E7%A7%BB%E5%8B%95%E3%81%A8%E6%94%BE%E5%B0%84%E7%A7%BB%E5%8B%95polar%E8%AA%BF%E6%95%B4%E3%83%8F%E3%83%B3%E3%83%89%E3%83%AB)  