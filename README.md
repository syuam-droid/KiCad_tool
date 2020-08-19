# KiCad_tool


## ファイルの種類
>NUCLEO-F303K8.zip
    NUCLEO-F303K8のシンボルとフットプリントが入ったフォルダ

>NUCLEO-F446RE.zip
    NUCLEO-F446REのシンボルとフットプリントが入ったフォルダ

>freeroute.zip
    KiCadの自動配線ツール


## 使い方
>NUCLEO-F303K8.zip

    適当な場所にPCB_Libraryというフォルダを作成し、その中に解凍する

    フォルダの名前をNUCLEO-F303K8.prettyに変更する

    フォルダの中に3つファイルがあるが、htmlファイルは必要ないので消してもよい

    KiCadを起動 > シンボルエディター > ファイル > ライブラリーを追加 > 先ほど解凍した中の.libファイルを選択 > 保存して終了

    シンボルについてはこれで完了

>NUCLEO-F446RE.zip

>freeroute.zip

    デスクトップに解凍し、freeroute.jarがあることを確認

    KiCadのPCBレイアウトエディター > ファイル > エクスポート > Specctra(DSN)で配線するファイルを出力

    このとき、作業フォルダにファイル名.dsnがあることを確認

    デスクトップに解凍したfreeroute.jarを起動 > Open Your Own Design > 先ほど出力したファイル名.dsnを選択

    Autorouterで自動配線開始 > 終了すると下のバーに文字が表示されるので確認 > File > Export Specctra Session Fileを選択し、データを出力する

    freeroute.jarはこれで終了

    再びKiCadを起動し、PCBレイアウトエディター > ファイル インポート > Specctraセッションを選択して自動配線データを読み込む

    これで自動配線は完了


## 参照URL
>NUCLEO-F303K8.zip

    https://www.snapeda.com/parts/NUCLEO-F303K8/STMicroelectronics/view-part/?ref=search&t=NUCLEO-F303K8

>NUCLEO-F446RE.zip

    https://www.snapeda.com/parts/NUCLEO-F446RE/STMicroelectronics/view-part/?ref=search&t=NUCLEO-F446RE

>freeroute.zip

    配布終了