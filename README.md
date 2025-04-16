# emotion

## 项目介绍
基于多模态情感分析大模型算法

## 环境部署

python3.8.2+cpu/gpu+CUDA11.8

## 数据集

-IEMOCAP数据集: 描述交互式情绪二元运动捕捉（iemocap）数据库是一个动作、多模式和多峰值的数据库，在南加州大学的Sail实验室收集。它包含大约12小时的视听数据，包括视频、语音、面部运动捕捉、文本转录。

6 classes: happy/sad/neutral/angry/excited/frustrated<br>
Raw Features: dataset/iemocap/raw/IEMOCAP_features_raw.pkl (Pickle files) <br>
The file contains:  
videoIDs[vid] = List of utterance IDs in this video in the order of occurance <br>
videoSpeakers[vid] = List of speaker turns. e.g. [M, M, F, M, F]. here M = Male, F = Female <br>
videoText[vid] = List of textual features for each utterance in video vid. <br>
videoAudio[vid] = List of audio features for each utterance in video vid. <br>
videoVisual[vid] = List of visual features for each utterance in video vid. <br>
videoLabels[vid] = List of label indices for each utterance in video vid. <br>
videoSentence[vid] = List of sentences for each utterance in video vid. <br>
trainVid =  List of videos (videos IDs) in train set. <br>
testVid =  List of videos (videos IDs) in test set. <br>

-MOSEI数据集: 由来自1000多个YouTube身份和200个主题的23500句话组成。

3 classes: positive/negative/neutral <br>
Raw Features: (Pickle files) <br>
Audio: dataset/mosei/raw/audio_3way.pickle <br>
Text: dataset/mosei/raw/text_3way.pickle <br>
Video: dataset/mosei/raw/video_3way.pickle <br>

-MOSI数据集:英文的多模态情感数据集，数据集中含有文本、语音和视频三种模态的信息，有2199个样本

2 classes: Positive/Negative <br>
Raw Features: (Pickle files) <br>
Audio: dataset/mosi/raw/audio_2way.pickle <br>
Text: dataset/mosi/raw/text_2way.pickle <br>
Video: dataset/mosi/raw/video_2way.pickle <br>
