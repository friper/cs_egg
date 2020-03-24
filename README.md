Cheat Sheet for Brain
===

Overview

## Motor-Imagery イメージ・トレーニング

### [Left/Right Hand MI](http://gigadb.org/dataset/100295) 両手の運動におけるイメージ・トレーニング
1. 概要

　52人の被験者（うち女性19人、平均年齢±SD年齢= 24.8±3.86歳）の左手と右手のMI運動についてBCI実験を実施した。これのデータ・セット。

2. 要件
- 64のAg / AgClアクティブ電極
- サンプリンググレード：512Hz
- BCI2000システム3.0.2
- 2本のEMG電極を深指屈筋と各腕の伸筋に取り付ける
- バックグラウンドノイズレベル：37〜39db

3. データ形式と構造

　各被験者のEEG（1番目から64番目のチャネル）およびEMG（65番目から68番目のチャネル）データ（「* .mat」）のMATLAB構造を以下に示す。
- 休息：目を開いた状態での休息状態
- ノイズ：
    - 瞬き、5秒×2
    - 眼球の上下運動、5秒×2
    - 眼球運動の左右、5秒×2
    - 顎噛み、5秒×2
    - 頭の動きを左右に、5秒×2
- imagery_left：左手MIの100または120試行
- imagery_right：右手のMIの100回または120回の試行
- n_imagery_trials：MIクラスごとに100または120回の試行
- imagery_event：値「1」は各MIトライアルの開始を表します
- movement_left：実際の左手の動きの20回の試行
- Movement_right：実際の右手の動きの20回の試行
- n_movement_trials：実際の手の動きのクラスごとに20回の試行
- movement_event：値「1」は、各運動試行の開始を表します
- frame：ミリ秒単位の試行の時間範囲
- srate：サンプリングレート
- senloc：3Dセンサーの位置
- psenloc：単位球に投影されたセンサー位置
- subject：件名の2桁のID-「s＃」
- comment：件名に対するコメント
- bad_trial_indices
    - 電圧の大きさによって決まる悪い試行
    - EMGの活動と相関する悪い試験

### [Motor Movement/Imagery Dataset](https://www.physionet.org/physiobank/database/eegmmidb/)
1. 概要
2. 要件
3. データ形式と構造

### [Grasp and Lift EEG Challenge](https://www.kaggle.com/c/grasp-and-lift-eeg-detection/data)
1. 概要
2. 要件
3. データ形式と構造

### [The largest SCP data of Motor-Imagery](https://doi.org/10.6084/m9.figshare.c.3917698)
1. 概要
2. 要件
3. データ形式と構造

### [BCI Competition IV-1](http://www.bbci.de/competition/iv/#dataset1)


### [BCI Competition IV-2a](http://www.bbci.de/competition/iv/#dataset2a)


### [BCI Competition IV-2b](http://www.bbci.de/competition/iv/#dataset2b)


### [High-Gamma Dataset](https://github.com/robintibor/high-gamma-dataset)


### [Left/Right Hand 1D/2D movements](https://sites.google.com/site/projectbci/)


### [Imagination of Right-hand Thumb Movement](https://archive.ics.uci.edu/ml/datasets/Planning+Relax)



## Emotion-Recognition 感情認識



## Error-Related Potentials (ErrP) エラー関連陰性電位
- **エラー関連陰性電位**･･･
脳波計測中において、被験者が何かしらの想定とは違う行為を認知した際に発生する陰性の事象関連電位のこと

###



## Visually Evoked Potentials (VEPs) 視覚誘発電位



## Event Related Potentials [ERPs] 事象関連電位



## Resting State 安静時の自発性能活動



## Music and EEG 聴覚刺激における脳波 



## Eye-blinks/movements 瞬きと動作が脳波に与える影響



## Miscellaneous 多方面の研究



## Clinical EEG 疾病者の脳波



## Others [Unfiltered]
