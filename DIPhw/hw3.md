---
layout: research
---

# 数字图像处理实验作业三　图像的直方图变换 

<p align="center"> 赵子瑞 </p>
<p align="center"> 自动化钱61  2160405068 </p>
<p align="center"> 2019年3月12日 </p>

### 摘要 
　　本文通过直方图变换的基本方法，实现了图像的直方图统计，图像的直方图均衡，图像的直方图匹配，局部直方图均衡和图像的直方图分割。本次试验加深了我利用直方图完成相应的图像增强的理解，让我对直方图处理图像的知识有了更深刻的理解。
  
## 项目任务

本次实验的任务分为以下几点：
* 1 将附件中所有图像的直方图画出
* 2 把所有图像进行直方图均衡，输出均衡后的图像和原图像进行对比，分析改善内容
* 3 进一步把图像按照对原图像直方图的观察，各自指定不同的原图像的直方图，进行直方图匹配，进行图像增强
* 4 对elain和lena图像进行7×7的局部直方图增强
* 5 利用直方图对图像elain和woman进行分割


## 图像的直方图表示 
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/project3/lena.bmp" height="20%" width="20%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/project3/elain.bmp" height="20%" width="20%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/project3/woman.bmp" height="20%" width="20%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/project3/citywall.bmp" height="20%" width="20%" /></p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/project3/lena_hist.png" height="20%" width="20%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/project3/elain_hist.png" height="20%" width="20%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/project3/woman_hist.png" height="20%" width="20%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/project3/citywall_hist.png" height="20%" width="20%" /></p>

## 直方图均衡 

直方图均衡的结果如下图所示。

<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_lena.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_elain.bmp" height="40%" width="40%" />　</p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_lena_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_elain_hist.png" height="40%" width="40%" />　</p>
<p align="center"><img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_woman.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_citywall.bmp" height="40%" width="40%" /></p>
<p align="center"><img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_woman_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_citywall_hist.png" height="40%" width="40%" /></p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_lena1.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_elain1.bmp" height="40%" width="40%" />　</p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_lena1_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_elain1_hist.png" height="40%" width="40%" />　</p>
<p align="center"><img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_woman1.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_citywall1.bmp" height="40%" width="40%" /></p>
<p align="center"><img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_woman1_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_citywall1_hist.png" height="40%" width="40%" /></p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_lena2.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_elain2.bmp" height="40%" width="40%" />　</p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_lena2_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_elain2_hist.png" height="40%" width="40%" />　</p>
<p align="center"><img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_woman2.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_citywall2.bmp" height="40%" width="40%" /></p>
<p align="center"><img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_woman2_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_citywall2_hist.png" height="40%" width="40%" /></p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_lena2.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_elain2.bmp" height="40%" width="40%" />　</p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_lena2_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_elain2_hist.png" height="40%" width="40%" />　</p>
<p align="center"><img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_woman2.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_citywall2.bmp" height="40%" width="40%" /></p>
<p align="center"><img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_woman2_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_citywall2_hist.png" height="40%" width="40%" /></p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_lena4.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_elain3.bmp" height="40%" width="40%" />　</p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_lena4_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/result_elain3_hist.png" height="40%" width="40%" />　</p>

## 直方图匹配 
通过观察直方图均衡的结果，我们发现直方图均衡可以有效的改善很多图像的状态，但是依然有很多不足。如果按照原图像对这直方图均衡后的图像进一步加强，可以进一步优化这些性质，让图像按照原有的像素分布进行映射，从而还原更多细节，进行有效的变换。

**说明：图像左边为原始图像，中间为均衡化图像，右边为直方图匹配后的图像**

<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_lena1.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_elain1.bmp" height="40%" width="40%" />　</p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_lena1_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_elain1_hist.png" height="40%" width="40%" />　</p>
<p align="center"><img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_woman1.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_citywall1.bmp" height="40%" width="40%" /></p>
<p align="center"><img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_woman1_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_citywall1_hist.png" height="40%" width="40%" /></p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_lena2.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_elain2.bmp" height="40%" width="40%" />　</p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_lena2_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_elain2_hist.png" height="40%" width="40%" />　</p>
<p align="center"><img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_woman2.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_citywall2.bmp" height="40%" width="40%" /></p>
<p align="center"><img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_woman2_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_citywall2_hist.png" height="40%" width="40%" /></p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_lena2.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_elain2.bmp" height="40%" width="40%" />　</p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_lena2_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_elain2_hist.png" height="40%" width="40%" />　</p>
<p align="center"><img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_woman2.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_citywall2.bmp" height="40%" width="40%" /></p>
<p align="center"><img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_woman2_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_citywall2_hist.png" height="40%" width="40%" /></p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_lena4.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_elain3.bmp" height="40%" width="40%" />　</p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_lena4_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/mat_result_elain3_hist.png" height="40%" width="40%" />　</p>

## 局部直方图均衡
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/local_result_lena.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/local_result_elain.bmp" height="40%" width="40%" />　</p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/local_result_lena_hist.png" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/local_result_elain_hist.png" height="40%" width="40%" />　</p>

## 直方图分割

对于直方图分割，我采用了课件中的方法，运用迭代的方法寻找阈值，通过寻找的阈值来实现对图像的分割。但是由于图像的背景和人物的像素特征接近，无法实现完全的分割，基于直方图的图像分割仅适用于背景和目标像素相差较大的图像。

<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/seg_result1_elain.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/seg_result2_elain.bmp" height="40%" width="40%" />　</p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/seg_result_elain_hist.png" height="40%" width="40%" />　</p>

<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/seg_result1_woman.bmp" height="40%" width="40%" />　<img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/seg_result2_woman.bmp" height="40%" width="40%" />　</p>
<p align="center"> <img src="https://raw.githubusercontent.com/1989Ryan/hw3/master/images/seg_result_woman_hist.png" height="40%" width="40%" />　</p>


## 小结

本次作业图像较多，主要运用python opencv的直方图均衡函数的同时，也自行实现了直方图匹配，直方图局部均衡化和直方图分割的基本函数，加深了我对理论知识的理解，也增强了我的代码动手能力。
