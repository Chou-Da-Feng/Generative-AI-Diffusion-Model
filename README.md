# Generative-AI-Diffusion-Model

## 摘要
擴散模型是一種生成式模型，通過在訓練過程中逐步向數據中添加噪聲，並學習如何消除噪聲來生成新的樣本。  
[Diffusion Model](https://drive.google.com/file/d/1HYHCSSGOMlvG8oImZfKS_Odp4kLCQ_o6/view?usp=sharing)<---此連結的pdf為參考台灣大學[李宏毅](https://www.youtube.com/@HungyiLeeNTU)老師的擴散模型影片與2022年8月出版的[Understanding Diffusion Models: A Unified Perspective](https://arxiv.org/abs/2208.11970)此篇論文製作而成，裡面包含了所有擴散模型數學原理的理解，再把數學轉換成程式碼的實現，還有模型的架構([Unet](https://arxiv.org/abs/1505.04597))。

## 實作

本專案的實作分為無條件式生成與有條件式生成兩部分。由於生成式模型需要大量的訓練時間與強大的計算資源，我使用 Google Colab 提供的 T4 GPU 來進行訓練。數據集方面，為了簡化實作流程，選擇了較簡單的數據集。

在無條件生成部分，我選用了 Kaggle 上的 Catface 數據集。由於無條件生成需要數據集的變異性較小，因此確保數據集中的樣本盡量一致，這樣生成結果才能清楚顯示為貓臉圖像。在有條件生成部分，我選用了 MNIST 手寫數字數據集，進行不同條件下的生成實驗。 

### 生成過程:

![cat gif](/README_resource/cat.gif)

### 無條件式生成結果:

![cat sampling](/README_resource/cat_sampling.png)

### 有條件式生成結果:

![mnist smapling](/README_resource/mnist_sampling.png)




