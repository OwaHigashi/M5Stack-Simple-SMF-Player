# M5Stack Simple SMF Player

## どんなプログラム？

こちらは、UNIT-SYNTHに対応した非常にシンプルなSMFプレーヤで、特に画面表示は何も行いません。

#include "MD_MIDIFile.h"

とあるように、MD_MIDIFileライブラリを利用します。このライブラリは、smfファイルを解析し、シリアルポートにMIDI信号を送信するために必要な全ての前処理を行うことができます。

再生したいファイルの一覧をプログラム中で指定することで再生できます。

- M5Stack Basic (CORE) を対象としていますが、Core2も含めて、出力先ポートを修正することで容易に対応可能です
- 音源は、UNIT-SYNTHを利用します
- プレイリストはプログラムに埋め込む形ですので、柔軟性はありません（画面表示もないため）

## ちょっと変わった使い方

大規模言語モデルの中には、仕様を与えるとその仕様に従ったプログラムを自動で生成する能力を持つモデルもｗります。こちらのコードを基本として入力し、追加の機能を文章であたえることで、より正確・簡単に狙ったコードが生成できるようになります。

プレイリストを自由にする、ボタンでプレイリスト番号を選ぶなど、容易にプレイリストを編集するなどの指示を与えることで、対応させることができます。
- 従って、極力シンプルにしています。
