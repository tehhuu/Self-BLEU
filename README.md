Self-BLEU

## Description

SacreBLEUを利用して、テキストファイル中の文の平均Self-BLEUスコアを求めます。

モデルの生成文の多様性の評価などに利用できます。

プログラムの動作手順は以下の通りです。

1. 全文から1文を選び，その文と残りの文のBLEUスコアを計算する。
1. 取り出す文を変えて，選ばれたことのない文がなくなるまで1を繰り返す。
1. 手順1，2で求まった値の平均を取る．

Calculating the average Self-BLEU Score in a text file by using 'SacreBLEU'.

You can use this to evaluate diversity of generated sentences from a model.

The process of the program is as follows
1. Choose one sentence and calculate the BLEU score between the sentence and remain sentenses.
1. Change the sentence and return to step-1 untill there are no sentence you can choose. 
1. take the average of the scores calculated in step1-2

## Requirement

・Python 3.x

・sacrebleu

https://github.com/mjpost/sacrebleu

(You can get by 'pip3 install sacrebleu')
