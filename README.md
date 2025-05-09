# dsbiztiu23150017.github.io

# FIX LOG
-R(Terminal)にて >cp *.* ..\dsbiztiu23150017.github.io\ を実行時、 
　'cp' は、内部コマンドまたは外部コマンド、操作可能なプログラムまたはバッチ ファイルとして認識されていません。

　解決策→
  1.Git Bashを開いて 'which git'と入力
  2.'cygpath -w 1の結果'と入力すると実際の場所が出てくる
  ![1-2](https://github.com/user-attachments/assets/615029ab-2151-4dcd-8fc0-5f261e5540da)
  3.出てきた場所の...\bin\を開いてその中に'cp.exe'というファイルがあるのを確認
  4.検索(三本指でタップ)から環境変数を開く
  5.ユーザーの環境変数内のPathを編集、先ほどの...\binのパスを新規で追加する
  6.Rを再起動したらcpコマンドが使えるようになる
