# 『PythonでPLCとつなぐ 現場データの読み書き入門』の教材

西城戸 亮 著『PythonでPLCとつなぐ 現場データの読み書き入門：MCプロトコル・Modbus・OPC UA　練習用PLCでPC1台から試せる』の実習教材です。

PLCの代わりに動く「練習用PLC」と、各章のプログラムが入っています。実機のPLCがなくても、PC1台でMCプロトコル（3Eフレーム）、Modbus TCP、OPC UAを試せます。

## 書籍（Amazon）

著者の他の本（製造業の技術書）：

- [『図解で学ぶ PLCプログラミング入門』](https://www.amazon.co.jp/dp/B0HMPS4P4M)：ラダーの基本から搬送・位置決め・PID・通信・異常復帰まで
- [『現場で使える製造業の画像検査自動化 第2版』](https://www.amazon.co.jp/dp/B0HJYJNHS6)：Python／OpenCVで、照明・判定・検証まで
- [『ラズパイとPythonでつくる 製造業の画像検査』](https://www.amazon.co.jp/dp/B0HKSGDZF2)：カメラ接続からOK／NG判定、記録・運用まで
- [『Claude Codeでつくる 製造業の画像検査システム』](https://www.amazon.co.jp/dp/B0HKSG1LWF)：AIに書かせたコードを、テストと実測で確かめる
- [『Pythonで始める 製造DXの実践』](https://www.amazon.co.jp/dp/B0HL5RK5H9)：現場データの収集・見える化から、管理図・異常検知まで

## 教材ZIPをダウンロードする

**[教材ZIPをダウンロード（約50 KB）](https://github.com/sunnishi/plc-python-book-materials/releases/download/v1.0.0/plc_python_code.zip)**

- 最新の教材：v1.0.0（2026年11月20日）
- ファイル名：`plc_python_code.zip`
- [この版の配布ページ](https://github.com/sunnishi/plc-python-book-materials/releases/tag/v1.0.0)

ダウンロードにGitHubアカウントは不要です。配布ページの「Assets」から取得する場合は、`plc_python_code.zip`を選んでください。自動表示される「Source code (zip)」「Source code (tar.gz)」には、教材は入っていません。

ZIPを展開すると`code`フォルダーができます。書籍の第4章の手順で準備してから始めてください。

## 収録内容

| 学ぶ内容 | 教材内の場所 | 章 |
| --- | --- | --- |
| 練習用PLC（MC 5000番・Modbus 5020番・OPC UA 4840番で待ち受け） | `run_practice_plc.py`、`practice_plc` | 第4章 |
| 環境の確認、ポートの確認 | `ch02`、`ch04` | 第2章・第4章 |
| Modbus TCPの読み書き・エラー・通信の中身 | `ch05` | 第5章 |
| MCプロトコルの読み書き・電文の組み立て | `ch06` | 第6章 |
| OPC UAのブラウズ・読み書き・購読 | `ch07` | 第7章 |
| 符号・32ビット・小数・文字列への変換 | `plcdata.py`、`ch08` | 第8章 |
| CSVへの記録とグラフ（サンプルデータ付き） | `ch09`、`ch10` | 第9章・第10章 |
| 切断に強い読み取り、やりとりの手順（ハンドシェイク） | `ch11`、`ch12` | 第11章・第12章 |
| 画像検査とPLCの連携、稼働モニター | `ch13`、`ch14` | 第13章・第14章 |
| 安全に書き込むための確かめ方 | `ch15` | 第15章 |

## 実行環境と検証範囲

Python 3.12以降で使ってください。制作時の環境はmacOSとPython 3.12、ライブラリの版は`requirements.txt`のとおりです。WindowsやLinuxでも動くように書いていますが、すべての環境では確かめていません。

練習用PLCは学習用の最小限の実装です。実機のPLC・実I/O・生産設備での動作は確かめていません。実機につなぐときは、書籍の「実機につなぐとき」の確かめ方に沿ってください。動いている設備のPLCに、確かめずに書き込まないでください。

## 正誤表

現時点で、報告された誤りはありません。

## 質問・不具合の報告

本文の誤りや、教材が動かない場合は、[Issues](https://github.com/sunnishi/plc-python-book-materials/issues)から報告してください。OS、Pythonの版、実行したコマンド、表示されたメッセージを添えると状況を確認しやすくなります。設備の図面や社内の情報は書き込まないでください。個別の設備への導入支援は対象外です。

## 利用条件

収録コードは、学習と自分の試作に改変・利用できます（LICENSEを参照）。PLCメーカーの機器・開発ソフトの利用条件は、それぞれの提供元に従います。三菱電機、MELSECは三菱電機株式会社の、Modbusは Schneider Electric USA Inc. の、OPC UAは OPC Foundation の商標または登録商標です。

## ダウンロードしたファイルを確認する

[SHA256SUMS.txt](SHA256SUMS.txt)の値と照合できます。
