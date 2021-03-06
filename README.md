Cheat Sheet for Brain
===

Overview


## Motor-Imagery イメージ・トレーニング

### [Left/Right Hand MI](http://gigadb.org/dataset/100295) 両手の運動におけるイメージ・トレーニング

date: 2017/5/05

**1. 概要**  
　52人の被験者（うち女性19人、平均年齢±SD年齢= 24.8±3.86歳）の左手と右手のMI運動についてBCI実験を実施した。これのデータ・セット。

**2. 要件**
- 64のAg / AgClアクティブ電極
- サンプリンググレード：512Hz
- BCI2000システム3.0.2
- 2本のEMG電極を深指屈筋と各腕の伸筋に取り付ける
- バックグラウンドノイズレベル：37~39db
- Matlab

**4. 実験内容**　　
　被験者の前方にスクリーンを用意し、スクリーン上に表示される指示に従って手を動かす

**5. データ形式と構造**  
　各被験者のEEG（1番目から64番目のチャネル）およびEMG（65番目から68番目のチャネル）データ（「* .mat」）のMATLAB構造を以下に示す。
- rest：目を開いた状態での休息状態
- noise：
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


### [Motor Movement/Imagery Dataset](https://www.physionet.org/physiobank/database/eegmmidb/) イメージと運動が脳波に及ぼす影響

date: 2009/9/9

**1. 概要**  
　109人の被験者を対象に、1500を超える1~2分程度の脳波計測データ。

**2. 要件**  
- 64チャンネルの電極
- BCI2000システム
- PhysioToolkit
- PhysioBank  

**3. 実験内容**　　
1. 目を開ける
2. 目を閉じる
3. タスク1　左手または右手の開閉
4. タスク2　左手または右手の開閉を想像する
5. タスク3　両手または両足の開閉
6. タスク4　両手または両足の開閉を想像する
7. タスク1
8. タスク2
9. タスク3
10. タスク4
11. タスク1
12. タスク2
13. タスク3
14. タスク4

**4. データ形式と構造**  
　「*.edf」と「*.edf.event」


### [Grasp and Lift EEG Challenge](https://www.kaggle.com/c/grasp-and-lift-eeg-detection/data)　物体を扱う際の脳と筋肉の関係

date: 2015/8/31

**1. 概要**  
　12人（8人の女性、19~35歳）の被験者に対し、モノを掴む、持ち上げる、移動させるの動作を指示し、その際の脳波を測定する。

**2. 要件**  
- 32 chanelsのEEG
- 5 chanelsのEMG
- 肩、前腕、および手の筋肉、腕、親指、人差し指

**3. 実験内容**  
1. HandStart
2. FirstDigitTouch
3. BouthStartLoadPhase
4. 下げる
5. 移動する
6. 両方とも話す

**4. データ形式と構造**  
　「*_data.csv」と「*_events.csv」
　
　id,HandStart,FirstDigitTouch,BothStartLoadPhase,LiftOff,Replace,BothReleased


### [The largest SCP data of Motor-Imagery](https://doi.org/10.6084/m9.figshare.c.3917698) イメージ・トレーニングのデータセット　　
[[詳細]](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6190745/pdf/sdata2018211.pdf)

date: 2018/10/11

**1. 概要**  
　13人の被験者から201の検出項目を75回測定する。被験者に対し、スクリーン上に指示を表示し、その際の脳波を計測する。 


### [BCI Competition IV-1](http://www.bbci.de/competition/iv/#dataset1)　BCIの発表のデータセット1

date: -

**概要**  
1. 7人の被験者の両手と両足に対して、MIを用意し、その脳波をモニタリングした。　　[64 chanels EEG, classes 2]
2. 9人の被験者の両手に足して、MI画像を見せ、それを実行した際の脳波　[22 chanels EEG, 3 chanels EOG, classes 4]
3. 9人の被験者の両手に足して、運動画像を見せ、それを実行した際の脳波 [3 bipolar chanels EEG, 3 chanels EOG, classes 2]
4. 2人の被験者に対して、手首の動きを行っている際の脳波　[10 chanels MEG, classes 4]
5. 3人の被験者に対して、指の動きを粉ている際の脳波　[48-64 chanels ECoG, classes 5] 


### [High-Gamma Dataset](https://github.com/robintibor/high-gamma-dataset) EEGの複合化・視覚化の深層学習　in Python

date: 2018/9/17 


### [Left/Right Hand 1D/2D movements](https://sites.google.com/site/projectbci/) 腕の動きとMI運動の脳波

date: -


### [Imagination of Right-hand Thumb Movement](https://archive.ics.uci.edu/ml/datasets/Planning+Relax) 脳波を用いた動作の事前思考とそうでない状態の判別

date: 2012/07/17 


## Emotion-Recognition 感情認識
- **[遺伝的アルゴリズム](https://dic.nicovideo.jp/a/遺伝的アルゴリズム)**

### [DEAP](http://www.eecs.qmul.ac.uk/mmv/datasets/deap/) 遺伝的アルゴリズム in Python

date: 2011

**1. 概要**  
　32人の被験者に対し、1分間のミュージックビデオを40本ずつ視聴した際の脳波と抹消の生理学的信号を測定する。
その際、覚醒度、価数、好き・嫌い、優位性、親しみやすさを評価する。

**2. 要件**  
- 32 chanels EEG
- 12 chanels around
- 3 chanels not use


### [Enterface'06](http://www.enterface.net/results/)　ワークショップのデータ集

date: 2006 - 2019


### [Imagined Emotion](http://headit.ucsd.edu/studies/3316f70e-35ff-11e3-a2a9-0050563f2612) 感情を示唆する音声

date: -

**1. 概要**  
　感情を誘起する音声を聞かせ、その感情の思い出を思い出したりやイメージしてもらう。
 

### [NeuroMarketing](https://link.springer.com/article/10.1007/s11042-017-4580-6) 消費者の好みに関する脳波　　
[データ](https://drive.google.com/open?id=0B2T1rQUvyyWcSGVVaHZBZzRtTms)

date: 2017/3/18
 

### [SEED](http://bcmi.sjtu.edu.cn/~seed/seed.html)　映像刺激による感情と脳波

date: -
 
* [SEED-IV](http://bcmi.sjtu.edu.cn/~seed/seed-iv.html)
* [SEED-VIG](http://bcmi.sjtu.edu.cn/~seed/seed-vig.html) 
 

### [HCI-Tagging](https://mahnob-db.eu/hci-tagging/) Webコンテンツと感情

date: -
 

### [Regulation of Arousal](https://ieee-dataport.org/open-access/regulation-arousal-online-neurofeedback-improves-human-performance-demanding-sensory) 難しい感覚運動に伴う脳波

date: 2019/4/03


## Error-Related Potentials (ErrP) エラー関連陰性電位
- **エラー関連陰性電位**･･･
脳波計測中において、被験者が何かしらの想定とは違う行為を認知した際に発生する陰性の事象関連電位のこと

### [BCI-NER Challenge](https://www.kaggle.com/c/inria-bci-challenge) 表示される文字の正誤を脳波で判断

date: 2015


### [Monitoring ErrP in a target selection task](http://bnci-horizon-2020.eu/database/data-sets) 汎用的な課題のデータセット

date:  -

* **Keywords**  

　MI、暗算、SCPトレーニング、ゲームプレイ、音楽、認知制御、エラーの監視


## Visually Evoked Potentials (VEPs) 視覚誘発電位

### [c-VEP BCI](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0051077)

date: 2012/12/07


### [c-VEP BCI with dry electrodes](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0172400)

date: 


### [SSVEP - Visual Search/Discrimination and Handshake](https://archive.ics.uci.edu/ml/datasets/EEG+Steady-State+Visual+Evoked+Potential+Signals#)

date: 


### [Synchronized Brainwave Dataset](https://www.kaggle.com/berkeley-biosense/synchronized-brainwave-dataset)

date: 


## Event Related Potentials [ERPs] 事象関連電位

### [Pattern Visual Evoked Potentials](https://www2.le.ac.uk/departments/engineering/research/bioengineering/neuroengineering-lab/software)

date:   


### [Face vs. House Discrimination](https://purl.stanford.edu/xd109qh3109)

date:   


### [Target Versus Non-Target](https://zenodo.org/record/2649069)

date:   


### [Target Versus Non-Target](https://zenodo.org/record/2669187)

date:   


### [Target Versus Non-Target](https://zenodo.org/record/3266223)

date:   


### [Target Versus Non-Target](https://zenodo.org/record/3267302)

date:   


### [Target Versus Non-Target](https://zenodo.org/record/3266930)

date:   


### [Target Versus Non-Target](https://zenodo.org/record/3268762)

date:   


### [Impedance Data](https://drive.google.com/drive/folders/0B3jfvN2T6iLMLWJMMVJMSXBqajg)

date:   


### [Sustained-Attention Driving](https://figshare.com/articles/Multi-channel_EEG_recordings_during_a_sustained-attention_driving_task/6427334/5)

date:   


### [Dryad-Speech](https://datadryad.org/stash/dataset/doi:10.5061/dryad.070jc)

date:   


## Resting State 安静時の自発性能活動

### [Resting State EEG Data](https://dataverse.tdl.org/dataverse/txstatecogelectro)

date: 


### [EID-M, EID-S](https://drive.google.com/drive/folders/1t6tL434ZOESb06ZvA4Bw1p9chzxzbRbj)

date: 


## Music and EEG 聴覚刺激における脳波 

### [Music Imagery Information Retrieval](https://github.com/sstober/openmiir)

date:  


## Eye-blinks/movements 瞬きと動作が脳波に与える影響

### [Involuntary Eye Movements during Face Perception](http://www2.hu-berlin.de/eyetracking-eeg/testdata.html)

date: 


### [Voluntary-Involuntary Eye-Blinks](https://drive.google.com/file/d/0By5iwWd39NblS2tRWmVTdmRzZUU/view?usp=sharing)

date: 


### [EEG-eye state](https://archive.ics.uci.edu/ml/datasets/EEG+Eye+State)

date: 


### [EEG-IO](http://gnan.ece.gatech.edu/eeg-eyeblinks/)

date: 


### [EEG-VV, EEG-VR](http://gnan.ece.gatech.edu/eeg-eyeblinks/)

date: 


### [Eye State Prediction](http://suendermann.com/corpus/EEG_Eyes.arff.gz)

date: 


### [Kara-One](http://www.cs.toronto.edu/~complingweb/data/karaOne/karaOne.html)

date: 


## Miscellaneous 多方面の研究

### [MNIST Brain Digits](http://mindbigdata.com/opendb/index.html)

date:  


### [Imagenet Brain](http://www.mindbigdata.com/opendb/imagenet.html)

date:  


### [Working Memory](https://github.com/pbashivan/EEGLearn/tree/master/Sample%20data)

date:  


### [Deep Sleep Slow Osciallation](https://challengedata.ens.fr/challenges/10)

date:  


### [Genetic Predisposition to Alcoholism](https://archive.ics.uci.edu/ml/datasets/EEG+Database)

date:  


## Clinical EEG 疾病者の脳波

### [TUH EEG Resources](https://www.isip.piconepress.com/projects/tuh_eeg/html/downloads.shtml)

date: 


### [Predict-UNM](http://predict.cs.unm.edu/)

date: 


## Others [Unfiltered]

### https://sccn.ucsd.edu/~arno/fam2data/publicly_available_EEG_data.html  
http://headit.ucsd.edu/studies

date: 


### 

date: 

