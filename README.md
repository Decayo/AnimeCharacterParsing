# AnimeCharacterParsing

[繁體中文](#繁體中文) |[English](#English)
#### [English](#English)

## A Semi-Supervised Deep Co-Training Approach to Anime Character Parsing  


### Introduction
&nbsp; &nbsp; &nbsp;&nbsp;A method for parsing anime characters using semi-supervised semantic segmentation. Due to the high cost of labeling, we adopt semi-supervised learning. Our data set has only 1,153 images, and 1,017 images are used for training and 136 images are used for verification. A preview of the dataset is below.  
![](https://i.imgur.com/o8V06jK.png)  
&nbsp; &nbsp; &nbsp;&nbsp;The generated segmentation map can be used in any  application which needs semantic map. The most common one is the face generation and automatic coloring of anime characters using GAN. Related work such as [DanbooRegion](https://github.com/lllyasviel/DanbooRegion) provides non-semantic instance segmentation and it performs very good on flatten coloring.  
&nbsp; &nbsp; &nbsp;&nbsp; This [paper](https://www.sysu-imsl.com/files/PG2021/line_art_colorization_pg2021_main.pdf) uses [tag2pix](https://github.com/blandocs/Tag2Pix) and 
[DanbooRegion](https://github.com/lllyasviel/DanbooRegion), the instance segmentation with tags also has a good coloring effect. Our segmentation can offered more detailed semantic relationship. Since there is no complete datasets of animation segmentation, so we provide the dataset and the parsing method, and this is the motivation of this work.   
&nbsp; &nbsp; &nbsp;&nbsp; The Github community also has two semantic segmentations for anime: [AniSeg](https://github.com/jerryli27/AniSeg) and [Anime-Semantic-Segmentation-GAN](https://github.com/pit-ray/Anime-Semantic-Segmentation-GAN), compared to these two projects, we can apply to more complex scene. The above two have many limit to usage, but we have almost none, as long as it is an illustration, we can output segmentation maps, and can generate more detailed segmentation.
  
&nbsp; &nbsp; &nbsp;&nbsp;

## Approach

- Wait for update

## Dataset and model download
- Wait for update

## Class Definition  
 ![](https://i.imgur.com/XQCPWCs.png)


## Experimental Results
&nbsp; &nbsp; &nbsp;&nbsp; We divide the experimental set into easy, medium and hard, and progress in order according to the degree of complexity, as defined in the following table:
![](https://i.imgur.com/4dHkzNE.png)
- 13-class experimental result
     ![](https://i.imgur.com/PCAjdYY.png)
- 16-class experimental result
     ![](https://i.imgur.com/7cdKW2S.png)

## Segmentation output
**Can perform well in：**
- Easy and medium difficulty in validation set
- Any colored illustrution or sketch
- Any artist style
- Any background (no matter whit or complex background)  
- Many people in one illustration 
- Any occulusion  
- Example reulsts of 13 classes (Input, Predict map, Ground Truth)：
![](https://i.imgur.com/PEnYlG3.png)
![](https://i.imgur.com/s4USR73.png)
![](https://i.imgur.com/Mq5LAUc.png)
![](https://i.imgur.com/T2jxWuP.png)
![](https://i.imgur.com/PfMmq3Z.png)
![](https://i.imgur.com/DbTuj8K.png)
![](https://i.imgur.com/WKK75cJ.png)
![](https://i.imgur.com/P7BFCTW.png)
![](https://i.imgur.com/VFUhHlV.png)
![](https://i.imgur.com/V6cAHSj.png)
![](https://i.imgur.com/DlWLP8I.png)
![](https://i.imgur.com/jP3c6gT.png)  
  
**Cannot perform well in：**  
- Hard difficulty in validation set
- Too small human body part or person
- Non-human character
- Complex light source
- Example reulsts of 13 classes (Input, Predict map, Ground Truth)：
![](https://i.imgur.com/ce8hz41.png)
![](https://i.imgur.com/K6uJmqQ.png)
![](https://i.imgur.com/MnOineG.jpg)
![](https://i.imgur.com/MLIyVm8.png)
![](https://i.imgur.com/XPuVD6F.jpg)
![](https://i.imgur.com/zSE4vny.png)  

 
TODO List
- [ ] Upload training and validation dataset
- [ ] Upload source code
- [ ] Upload trained model


#### [繁體中文](#繁體中文)

## 動漫人物人體解析 使用半監督協同訓練  


### 簡介
&nbsp; &nbsp; &nbsp;&nbsp;一個使用半監督語意分割的動漫人物解析方法，由於標註成本較高，因此我們採用半監督學習，我們的資料集僅1153張圖片，並使用1017張使用於訓練136張用於驗證下圖為本資料集的預覽。
![](https://i.imgur.com/o8V06jK.png)  
&nbsp; &nbsp; &nbsp;&nbsp;產生的分割圖可以後續做任何應用，最常見的是使用GAN的動漫人物生成和自動上色，相關工作如[DanbooRegion](https://github.com/lllyasviel/DanbooRegion)提供了無語意的實力分割，他的相關研究在平塗自動上色表現十分優異，而這篇[論文](https://www.sysu-imsl.com/files/PG2021/line_art_colorization_pg2021_main.pdf)使用了[tag2pix](https://github.com/blandocs/Tag2Pix)和[DanbooRegion](https://github.com/lllyasviel/DanbooRegion)，進行標籤自動上色也有很好的著色效果。我們的分割塗可以說是更細緻的語義關係，由於目前並沒有成套的資料集和可直接使用的動漫分割，這正是本篇工作的動機所在。Github社群也有兩個關於動漫的語義分割：[AniSeg](https://github.com/jerryli27/AniSeg)和[Anime-Semantic-Segmentation-GAN](https://github.com/pit-ray/Anime-Semantic-Segmentation-GAN)，較於這兩個專案，我們能適用的範圍更廣，上述這兩個多有使用限制，而我們幾乎沒有，只要是插圖就能輸出分割圖，並且能夠分割得更好更細緻。
  
&nbsp; &nbsp; &nbsp;&nbsp;

## 方法

- 待更新

## 資料集和訓練模型下載
- 待更新

## 類別定義  
 ![](https://i.imgur.com/XQCPWCs.png)


## 實驗數據
&nbsp; &nbsp; &nbsp;&nbsp; 我們將實驗集分為簡單、中等和困難，根據複雜程度依序遞進，定義如下表：
![](https://i.imgur.com/4dHkzNE.png)
- 類別13的實驗數據
     ![](https://i.imgur.com/PCAjdYY.png)
- 類別16的實驗數據
     ![](https://i.imgur.com/7cdKW2S.png)

## 結果和適用場景
**適用場景：**
- 驗證集中的簡單和中等難度
- 彩圖與線稿
- 任何畫風 (厚塗、賽璐璐皆可)
- 任何背景  
- 多個人物  
- 任何遮擋(文字，花，樹枝，特效等)  
- 範例圖片-12個類別(依序為輸入、輸出、GroundTruth)：
![](https://i.imgur.com/PEnYlG3.png)
![](https://i.imgur.com/s4USR73.png)
![](https://i.imgur.com/Mq5LAUc.png)
![](https://i.imgur.com/T2jxWuP.png)
![](https://i.imgur.com/PfMmq3Z.png)
![](https://i.imgur.com/DbTuj8K.png)
![](https://i.imgur.com/WKK75cJ.png)
![](https://i.imgur.com/P7BFCTW.png)
![](https://i.imgur.com/VFUhHlV.png)
![](https://i.imgur.com/V6cAHSj.png)
![](https://i.imgur.com/DlWLP8I.png)
![](https://i.imgur.com/jP3c6gT.png)  
  
**不適用場景：**  
- 驗證集中的困難難度
- 人物太小
- 非典型動漫人物
- 過於複雜的光影
- 範例圖片-12個類別(驗證集輸出，依序為輸入、輸出、GroundTruth)：
![](https://i.imgur.com/ce8hz41.png)
![](https://i.imgur.com/K6uJmqQ.png)
![](https://i.imgur.com/MnOineG.jpg)
![](https://i.imgur.com/MLIyVm8.png)
![](https://i.imgur.com/XPuVD6F.jpg)
![](https://i.imgur.com/zSE4vny.png)  

 
TODO List
- [ ] 上傳訓練用和驗證資料集
- [ ] 上傳源碼
- [ ] 上傳訓練完成模型檔案
--------------------------------------
--------------------------------------


