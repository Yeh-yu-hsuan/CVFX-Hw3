# homework3-GAN-Dissection

## Assign

1.  10% (Generate images with GANPaint)
2.  20% (Dissect any GAN model and analyze what you find)
3.  20% (Compare with other method)
4.  30% (Assistant) 
5.  20% (Mutual evaluation)

## 1. Generate images with GANPaint
|GANPaint|Before|After|
|--------|------|-----|
|**Example 1**|<img src='fig1/1-1.png'>|<img src='fig1/1-2.png'>|
|**Example 2**|<img src='fig1/2-1.png'>|<img src='fig1/2-2.png'>|
|**Example 3**|<img src='fig1/3-1.png'>|<img src='fig1/3-2.png'>|

## 2. Dissect GAN model and analyze
We dissect our GAN model which is trained on LSUN livingroom dataset. Here we show some dissecting examples:

### Ceiling 
<img src='fig2/hw3-1.png'>

### Sofa
<img src='fig2/hw3-2.png'>

### Window
<img src='fig2/hw3-3.png'>

GAN dissection can automatically find the corresponding feature maps of certain labels. The area of yellow circles indicates that the feature maps are similar.

However, failures also happen frequently. We also show some failure case as the following figures:

### Chair
<img src='fig2/hw3-fail.png'>

## 3. Compare with other method 

* Globally and Locally Consistent Image Completion [method1]

* EdgeConnect: Generative Image Inpainting with Adversarial Edge Learning [method2]

* Generative Image Inpainting with Contextual Attention [method3]

We compare three generative inpaiting methods. For each image, we crop a rectangle and fill it with white color. For clearer visualization, we compress the results as gif animation. The display order is the original image, cropped image, and inpainted image, respectively.

In general, the three methods can perform well on the grass

|Method|Globally and Locally Consistent Image Completion|EdgeConnect: Generative Image Inpainting with Adversarial Edge Learning|Generative Image Inpainting with Contextual Attention|
|-----------|------------|-----------|--------------|
|**Sample_1**|<img src='fig_gif/method1/cat.gif' width="600">|<img src='fig_gif/method2/cat.gif' width="600">|<img src='fig_gif/method3/new_cat.gif' width="600">|
|**Sample_2**|<img src='fig_gif/method1/g.gif' width="600">|<img src='fig_gif/method2/g.gif' width="600">|<img src='fig_gif/method3/g.gif' width="600">|
|**Sample_3**|<img src='fig_gif/method1/m.gif' width="600">|<img src='fig_gif/method2/m.gif' width="600">|<img src='fig_gif/method3/m.gif' width="600">|
|**Sample_4**|<img src='fig_gif/method1/re_f.gif' width="600">|<img src='fig_gif/method2/re_f.gif' width="600">|<img src='fig_gif/method3/re_f_1.gif' width="600">|
|**Sample_5**|<img src='fig_gif/method1/re_f2.gif' width="600">|<img src='fig_gif/method2/re_f2.gif' width="600">|<img src='fig_gif/method3/re_f_2.gif' width="600">|
|**Sample_6**|<img src='fig_gif/method1/re_f3.gif' width="600">|<img src='fig_gif/method2/re_f3.gif' width="600">|<img src='fig_gif/method3/re_f_3.gif' width="600">|
|**Sample_7**|<img src='fig_gif/method1/re_f4.gif' width="600">|<img src='fig_gif/method2/re_f4.gif' width="600">|<img src='fig_gif/method3/re_f_4.gif' width="600">|

