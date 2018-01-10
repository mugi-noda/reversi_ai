# reversi_ai
Artifical Intelligence of Reversi (Othello)

How to compile the Reversi_AI
-
※GUIがWindowsにしか対応していないため、ここではWindowsでのコンパイル方法のみを解説します。（ほかのOS、環境でもほぼ同じですが。）
※コンパイルにはC++11以上に対応したコンパイラが必要です。（私はMinGW(https://sourceforge.net/projects/mingw-w64/)を使っています。）
※最適化オプションについては、デバッグの目的がない限り、すべて記載することをお勧めします。

手順
-
1. "Revrsi_AI"のディレクトリでターミナル（cmd.exeなど）を開きます。
2. "g++ main.cpp -std=c++17 -O3 -mtune=native -march=native -flto -o a.exe"でコンパイルします。

AIはGUIでの使用を前提としてIOが設計されています。CUIで使いたい場合（おもにLINUXで使いたい場合）、以下のようにmain.cppを変更してください。

Line9: game.showBoard();    -->       game.show();

Line22: game.showBoard();   -->       game.show();


How to build the Reversi_GUI
-
"visualstudio2017"か"build tools for visualstudio2017"を使ってビルドしてください。

How to run Reversi_AI on Reversi_GUI
-
 Reversi_AIをコンパイルして生成されたexeファイルをRevresi_GUI.exeがあるディレクトリにコピーし、Reversi_GUI.exeを実行してください。
 Reversi_AIを実行して生成されたa.exeは単独でも実行可能です。コマンドラインから呼び出してください。
