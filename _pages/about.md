---
permalink: /
title: "About"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
<style>
  .slideshow-container {
    width: 500px;
    height: 300px;
    position: relative;
    overflow: hidden;
  }
        
  .slideshow-container input {
    display: none;
  }
  
  .slideshow-container img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    position: absolute;
    top: 0;
    left: 0;
    opacity: 0;
    transition: opacity 0.5s ease-in-out;
  }
  
  .slideshow-container input:checked + img {
      opacity: 1;
  }
  
  .slideshow-controls {
      position: absolute;
      bottom: 10px;
      left: 50%;
      transform: translateX(-50%);
      z-index: 1;
  }
  
  .slideshow-controls label {
      display: inline-block;
      width: 10px;
      height: 10px;
      border-radius: 50%;
      background-color: #999;
      margin: 0 5px;
      cursor: pointer;
  }
  
  .slideshow-controls label:hover {
      background-color: #333;
  }
  
  .slideshow-controls input:checked + label {
      background-color: #333;
  }
</style>

Hello, I am Xiaochuan Ai（艾小川）, a fourth-year student majoring in Computer Science and Technology at Xi'an Technological University. My research interests lie in Machine Learning, Deep Learning, Computer Vision, Generative Modeling, and Multimodality. Recently, I focus on doing research in the field of speech generation motion in 3d human reconstruction, focusing on improving the model computing speed and running efficiency.For my CV,please refer.[CV](assets/Curriculum Vitae.pdf).<br>


**I am actively seeking a Ph.D./RA position**.<br>

If you think I would be a good fit or would like to work with me, please feel free to contact me via email to further explore potential collaboration opportunities. Thanks!




Awards
======


* 2022/06   Won [Third prize](images/微信图片_202307192028502.jpg) of China Undergraduate Mathematical Contest in Modeling.
* 2022/11   Awarded as a [Merit student](images/微信图片_20230719202850.jpg) for the 2021-2022 school year.
* 2022/11   Awarded Second Class[Academic Scholarship](images/微信图片_202307192028501.jpg) for the 2021- 2022 academic year.
* 2022/11   Won [First prize](images/微信图片_202307192028511.jpg) of ICT competition.
* 2022/12   Won [Second prize](images/微信图片_20230719202851.jpg) of 2022-2023  ICT Competition Shaanxi Division.<br>
 
<img src="assets/ICT获奖.PNG" alt="ICT获奖" width="400" height="300"/>
<br>

<ul>
      <div class="slideshow-container">
        <input type="radio" name="slide" id="slide1" checked>
        <img src="images/微信图片_202307192028502.jpg" alt="Image 1">
        <input type="radio" name="slide" id="slide2">
        <img src="images/微信图片_20230719202850.jpg" alt="Image 2">
        <input type="radio" name="slide" id="slide3">
        <img src="images/微信图片_202307192028501.jpg" alt="Image 3">
        <input type="radio" name="slide" id="slide3">
        <img src="images/微信图片_202307192028511.jpg" alt="Image 4">
        <input type="radio" name="slide" id="slide3">
        <img src="images/微信图片_20230719202851.jpg" alt="Image 5">        
        <div class="slideshow-controls">
          <input type="radio" name="slide-dot" id="slide-dot1" checked>
          <label for="slide-dot1"></label>
          <input type="radio" name="slide-dot" id="slide-dot2">
          <label for="slide-dot2"></label>
          <input type="radio" name="slide-dot" id="slide-dot3">
          <label for="slide-dot3"></label>
          <input type="radio" name="slide-dot" id="slide-dot4">
          <label for="slide-dot4"></label>
          <input type="radio" name="slide-dot" id="slide-dot5">
          <label for="slide-dot5"></label>
      </div>
    </div>
</ul>

<script>
  // 在页面加载完毕后执行
  document.addEventListener('DOMContentLoaded', function() {
    // 获取轮播容器和轮播图片数量
    var slideshowContainer = document.querySelector('.slideshow-container');
    var slideshowImages = slideshowContainer.querySelectorAll('img');
    var numImages = slideshowImages.length;
    
    // 定义初始显示的图片索引
    var currentImageIndex = 0;
    
    // 自动切换图片的间隔时间（单位：毫秒）
    var interval = 2000;
    
    // 切换图片的函数
    function changeImage() {
      // 隐藏当前显示的图片
      slideshowImages[currentImageIndex].style.opacity = 0;
      
      // 计算下一张图片的索引
      currentImageIndex = (currentImageIndex + 1) % numImages;
      
      // 显示下一张图片
      slideshowImages[currentImageIndex].style.opacity = 1;
      
      // 设置定时器，延迟切换下一张图片
      setTimeout(changeImage, interval);
    }
    
    // 执行切换图片函数
    setTimeout(changeImage, interval);
  });
</script>



