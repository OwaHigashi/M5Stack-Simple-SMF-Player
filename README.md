# M5Stack Simple SMF Player

こちらは、非常にシンプルなSMFプレーヤで、特に画面表示は何も行いません。

#include "MD_MIDIFile.h"

とあるように、MD_MIDIFileライブラリを利用します。このライブラリは、smfファイルを解析し、シリアルポートにMIDI信号を送信するために必要な全ての前処理を行うことができます。

再生したいファイルの一覧をプログラム中で指定することで再生できます。
