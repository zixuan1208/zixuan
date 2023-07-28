---
permalink: /
title: "About "
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

Hello, I'm Zixuan He, a fourth-year student at Nanjing University of Finance and Economics majoring in Computer Science and Technology (B.S.), advised by [Prof. Lei Zhang](https://xueshu.baidu.com/scholarID/CN-BK73TEKJ).  
My research interests are in machine learning, deep learning, computer vision, multimodality, and applications to autonomous driving. Currently, I am doing research on multimodal field of speech-to-motion in terms of 3d. For my CV, please refer to [CV](Zixuan_He_CV.pdf). Free to email me if you would like to work together!  

**I am actively looking for Ph.D./RA position, please contact me if you think I am a good fit.**


Awards
======
<ul>
    <li>2023/1 Won <a href="中国机器人大赛三等奖.jpg">in the 17th Intelligent Vehicle Competition.
      <div class="slideshow-container">
        <input type="radio" name="slide" id="slide1" checked>
        <img src="中国机器人大赛三等奖.jpg" alt="Image 1">
        <input type="radio" name="slide" id="slide2">
        <img src="智能车比赛国家一等奖.jpg" alt="Image 2">
        <input type="radio" name="slide" id="slide3">
        <img src="美赛建模H奖.jpg" alt="Image 3">
        <div class="slideshow-controls">
          <input type="radio" name="slide-dot" id="slide-dot1" checked>
          <label for="slide-dot1"></label>
          <input type="radio" name="slide-dot" id="slide-dot2">
          <label for="slide-dot2"></label>
          <input type="radio" name="slide-dot" id="slide-dot3">
        <label for="slide-dot3"></label>
      </div>
    </div>
    </li>
    <li>2022/8 Won the <a href="智能车比赛国家一等奖.jpg">Third Prize</a> of the China University Student Design Competition.</li>
    <li>2022/2 Participated in MCM/ICM to obtain <a href="美赛建模H奖.jpg">Honorable Mentions</a>.</li>
    <li>Some other modeling competitions such as May Day Modelling, and APMCM.</li>
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






