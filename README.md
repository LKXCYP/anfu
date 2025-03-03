<!doctype html>
<html lang="zh-CN">
  <head>
    <meta charset="UTF-8" />
    <title>福州安复安全咨询服务有限公司</title>
    <style>
      body {
          background-color: #e8f5e9; /* 浅绿色背景 */
          color: #2e7d32; /* 深绿色文本 */
          font-family: Arial, sans-serif;
      }

      h1, h2 {
          color: #1b5e20; /* 更深的绿色标题 */
      }

      a {
          color: #388e3c; /* 绿色链接 */
          text-decoration: none;
      }

      a:hover {
          text-decoration: underline;
      }

      #centered-div {
          border: 2px solid #2e7d32; /* 深绿色边框 */
          padding: 10px; /* 内边距，使内容与边框有一定距离 */
          border-radius: 5px; /* 圆角边框 */
          margin: 0; /* 将外边距设置为0，使div左对齐 */
          text-align: center; /* 将文本内容居中 */
      }

      nav ul {
          list-style-type: none; /* 去除列表项的默认标记 */
          padding: 0;
      }

      nav ul span {
          display: inline-block;
          margin-right: 20px;
      }

      nav ul span a {
          border: 2px solid #2e7d32; /* 深绿色边框 */
          padding: 5px 10px; /* 内边距 */
          text-decoration: none; /* 去掉下划线 */
          color: #2e7d32; /* 链接颜色 */
      }

      .dropdown {
          position: relative;
          display: inline-block;
          overflow: visible; /* 根据需要调整，确保子元素不会被裁剪 */
      }

      #dropdown-arrow {
          margin-right: 0px; /* 根据需要调整 */
      }

      .dropdown-content {
          display: none;
          position: absolute;
          background-color: #f9f9f9;
          min-width: 160px;
          box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
          z-index: 1;
      }

      .dropdown-content a {
          color: black;
          padding: 12px 16px;
          text-decoration: none;
          display: block;
      }

      .dropdown-content a:hover {
          background-color: #f1f1f1;
      }

      h4 {
          margin-top: 0; /* 去除h4元素的顶部外边距，使它更贴近边框 */
      }

      li {
          list-style-type: none; /* 去除列表项的默认标记 */
          margin: 5px 0; /* 为每个列表项添加上下外边距，使其间隔开 */
      }

      table {
          width: 100%;
          border-collapse: collapse; /* 合并表格边框 */
          margin: 0; /* 表格左对齐 */
      }

      th, td {
          border: 1px solid #2e7d32; /* 深绿色单元格边框 */
          padding: 10px; /* 单元格内边距 */
          text-align: center; /* 单元格文本居中 */
      }

      th {
          background-color: #c8e6c9; /* 浅绿色表头背景色 */
      }

      /* 设置特定段落中的链接颜色 */
      .no-color a {
          color: inherit; /* 继承父元素的颜色 */
          text-decoration: none; /* 去掉下划线 */
      }

      /* 设置 logo 图片的圆角边框 */
      img {
          border-radius: 15px; /* 圆角边框 */
          border: 3px solid #2e7d32; /* 深绿色边框 */
      }

      /* 居中显示 logo */
      .logo-container {
          text-align: center; /* 居中对齐 */
      }

      .logo-container span {
          display: inline-block; /* 使 span 元素并排显示 */
          margin: 0 10px; /* 添加左右外边距 */
      }

      /* 返回顶部按钮样式 */
      #back-to-top {
          display: none; /* 默认隐藏 */
          position: fixed; /* 固定位置 */
          bottom: 20px; /* 距离底部20px */
          right: 20px; /* 距离右侧20px */
          z-index: 99; /* 确保按钮在最上层 */
          border: none; /* 无边框 */
          outline: none; /* 无轮廓 */
          background-color: #2e7d32; /* 按钮背景色 */
          color: white; /* 按钮文字颜色 */
          cursor: pointer; /* 鼠标指针样式 */
          padding: 15px; /* 内边距 */
          border-radius: 10px; /* 圆角边框 */
          font-size: 18px; /* 字体大小 */
      }

      #back-to-top:hover {
          background-color: #1b5e20; /* 悬停时的背景色 */
      }

      /* 轮播容器样式 */
      #slider {
          position: relative;
          width: 600px;
          height: 600px;
          overflow: hidden;
          margin: 0; /* 左对齐 */
      }

      /* 图片列表样式 */
      #slider ul {
          list-style-type: none;
          margin: 0;
          padding: 0;
          position: absolute;
          width: 80%;
          height: 80%;
      }

      /* 单个图片样式 */
      #slider ul li {
          position: absolute;
          width: 80%;
          height: 80%;
          opacity: 0;
          transition: opacity 1s;
      }

      /* 图片样式 */
      #slider ul li img {
          width: 80%;
          height: 80%;
          object-fit: cover;
      }

      /* 显示当前图片 */
      #slider ul li.active {
          opacity: 1;
      }
    </style>
    <script>
      function toggleDropdown() {
          var dropdownContent = document.getElementById("dropdown-content");
          var dropdownArrow = document.getElementById("dropdown-arrow");
          if (dropdownContent.style.display === "block") {
              dropdownContent.style.display = "none";
              dropdownArrow.innerHTML = "▲";
          } else {
              dropdownContent.style.display = "block";
              dropdownArrow.innerHTML = "▼";
          }
      }

      // 显示或隐藏返回顶部按钮
      window.onscroll = function() {
          var backToTopButton = document.getElementById("back-to-top");
          if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
              backToTopButton.style.display = "block";
          } else {
              backToTopButton.style.display = "none";
          }
      };

      // 返回顶部
      function backToTop() {
          document.body.scrollTop = 0;
          document.documentElement.scrollTop = 0;
      }

      // 图片轮播
      document.addEventListener("DOMContentLoaded", function() {
          var slides = document.querySelectorAll("#slider ul li");
          var currentIndex = 0;

          function showSlide(index) {
              slides.forEach(function(slide, i) {
                  slide.classList.remove("active");
                  if (i === index) {
                      slide.classList.add("active");
                  }
              });
          }

          function nextSlide() {
              currentIndex = (currentIndex + 1) % slides.length;
              showSlide(currentIndex);
          }

          showSlide(currentIndex);
          setInterval(nextSlide, 3000); // 每3秒切换一次图片
      });
    </script>
  </head>

  <body>
    <div id="centered-div">
      <img src="images/安复安全logo.png" alt="安复logo" title="至诚学院logo和安复logo" width="400" height="120"/>
      <!-- logo栏 -->
      <h1 id="home">福州安复安全咨询服务有限公司</h1>
      <!-- 公司名称 -->
      <nav>
        <ul>
          <span><a href="安复首页.html" target="_self">首页</a></span>
          <span><a href="技术支持.html" target="_self">技术支持</a></span>
          <span><a href="经营范围.html" target="_self">经营范围</a></span>
          <span><a href="经营范围.html" target="_self">涉及业务</a></span>
          <span><a href="业务介绍.html" target="_self">业务介绍</a></span>
          <span class="dropdown">
            <a href="javascript:void(0);" onclick="toggleDropdown()">
                <span id="dropdown-arrow">▲</span>
                <a href="项目展示.html" target="_self">项目展示
            </a>
            <div id="dropdown-content" class="dropdown-content">
                <a href="信息化项目展示.html" target="_self">信息化项目展示</a>
                <a href="应急预案编制项目展示.html" target="_self">应急预案编制</a>
                <a href="风险评估.html" target="_self">风险评估</a>
                <a href="隐患排查.html" target="_self">应急预案编制</a>
            </div>
        </span>
          <span><a href="关于我们.html" target="_self">关于我们</a></span>
          <span><a href="联系我们.html" target="_self">联系我们</a></span>
        </ul>
      </nav>
    </div>
    <div id="slider">
        <ul>
            <li class="active"><img src="images/1.png" alt="图片1"></li>
            <li><img src="images/2.png" alt="图片2"></li>
            <li><img src="images/3.png" alt="图片3"></li>
            <li><img src="images/4.png" alt="图片4"></li>
            <li><img src="images/5.png" alt="图片5"></li>
            <li><img src="images/6.png" alt="图片6"></li>
            <li><img src="images/7.png" alt="图片7"></li>
            <li><img src="images/8.png" alt="图片8"></li>
            <li><img src="images/9.png" alt="图片9"></li>
            <li><img src="images/10.png" alt="图片10"></li>
            <li><img src="images/11.png" alt="图片11"></li>
            <li><img src="images/12.png" alt="图片12"></li>
            <li><img src="images/13.png" alt="图片13"></li>
            <li><img src="images/14.png" alt="图片14"></li>
            <li><img src="images/15.png" alt="图片15"></li>
            <li><img src="images/16.png" alt="图片16"></li>
            <li><img src="images/17.png" alt="图片17"></li>
            <li><img src="images/18.png" alt="图片18"></li>
            <li><img src="images/19.png" alt="图片19"></li>
            <li><img src="images/20.png" alt="图片20"></li>
            <li><img src="images/21.png" alt="图片21"></li>
            <li><img src="images/22.png" alt="图片22"></li>
            <li><img src="images/23.png" alt="图片23"></li>
            <li><img src="images/24.png" alt="图片24"></li>
            <li><img src="images/25.png" alt="图片25"></li>
            <li><img src="images/26.png" alt="图片26"></li>
            <li><img src="images/27.png" alt="图片27"></li>
            <li><img src="images/28.png" alt="图片28"></li>
            <li><img src="images/安复logo.png" alt="图片29"></li>
            <li><img src="images/福建蓬希logo.png"alt=图片30"></li>
            <li><img src="images/福州大学logo.jpg" alt="图片31"></li>
        </ul>
    </div>
    <button id="back-to-top" onclick="backToTop()">返回顶部</button>
  </body>
</html>

<style>
  /* 返回顶部按钮样式 */
  #back-to-top {
      display: none; /* 默认隐藏 */
      position: fixed; /* 固定位置 */
      bottom: 20px; /* 距离底部20px */
      right: 20px; /* 距离右侧20px */
      z-index: 99; /* 确保按钮在最上层 */
      border: none; /* 无边框 */
      outline: none; /* 无轮廓 */
      background-color: #2e7d32; /* 按钮背景色 */
      color: white; /* 按钮文字颜色 */
      cursor: pointer; /* 鼠标指针样式 */
      padding: 15px; /* 内边距 */
      border-radius: 10px; /* 圆角边框 */
      font-size: 18px; /* 字体大小 */
  }

  #back-to-top:hover {
      background-color: #1b5e20; /* 悬停时的背景色 */
  }
</style>

<script>
  // 显示或隐藏返回顶部按钮
  window.onscroll = function() {
      var backToTopButton = document.getElementById("back-to-top");
      if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
          backToTopButton.style.display = "block";
      } else {
          backToTopButton.style.display = "none";
      }
  };

  // 返回顶部
  function backToTop() {
      document.body.scrollTop = 0;
      document.documentElement.scrollTop = 0;
  }
</script>
