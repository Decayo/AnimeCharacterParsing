# AnimeCharacterParsing

[繁體中文](#繁體中文) |English


#### [繁體中文](#繁體中文)

## 動漫人物人體解析 使用半監督協同訓練  


### 簡介
&nbsp; &nbsp; &nbsp;&nbsp;一個使用半監督語意分割的動漫人物解析方法，由於標註成本較高，因此我們採用半監督學習，我們的資料集僅1153張圖片，並使用1017張使用於訓練136張用於驗證下圖為本資料集的預覽。
![](https://i.imgur.com/o8V06jK.png)  
&nbsp; &nbsp; &nbsp;&nbsp;產生的分割圖可以後續做任何應用，最常見的是使用GAN的動漫人物生成和自動上色，相關工作如DanbooRegion提供了無語意的實力分割，他的相關研究在平塗自動上色表現十分優異，而這篇論文使用了tag2pix和DanbooRegion，進行標籤自動上色也有很好的著色效果。我們的分割塗可以說是更細緻的語義關係，由於目前並沒有成套的資料集和可直接使用的動漫分割，這正是本篇工作的動機所在。Github社群也有兩個關於動漫的語義分割：AniSeg和Anime-Semantic-Segmentation-GAN，較於這兩個我們的類別有16個和13個，並且能夠分割得更好更細緻。
  
&nbsp; &nbsp; &nbsp;&nbsp;



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
- 彩圖與線稿
- 任何畫風 (厚塗、賽璐璐皆可)
- 任何背景  
- 多個人物  
- 任何遮擋(文字，花，樹枝，特效等)  
- 範例圖片-12個類別(驗證集輸出，依序為輸入、輸出、GroundTruth)：
![](https://i.imgur.com/PEnYlG3.png)
![](https://i.imgur.com/s4USR73.png)
![](https://i.imgur.com/Mq5LAUc.png)
![](https://i.imgur.com/T2jxWuP.png)
![](https://i.imgur.com/PfMmq3Z.png)
![](https://i.imgur.com/DbTuj8K.png)
![](https://i.imgur.com/fYfNrLt.png)
![](https://i.imgur.com/VFUhHlV.png)
![](https://i.imgur.com/V6cAHSj.png)
![](https://i.imgur.com/DlWLP8I.png)
![](https://i.imgur.com/jP3c6gT.png)  
  
**不適用場景：**  

- 人物太小
- 非典型動漫人物 (如福瑞等其他非人)
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


