<html>
<head>
<meta charset="utf-8">
<title>网传小官网</title>
<link rel="stylesheet" type="text/css" href="style.css" />
<link rel="stylesheet" type="text/css" href="swiper-3.4.0.min.css" />
</head>
<body>
<div class="content">
   <div class="header">
     <img src="logo.png">
        <div class="quickLink">
            <a href="#">教师进入</a>
            <a href="#">教师进入</a>
            <a href="#">教师进入</a>
        </div>
   </div>
</div>
<div class="nav">
      <ul>
         <a href="#"><li>首页</li> </a>
         <a href="#"><li>首页</li> </a> 
         <a href="#"><li>首页</li> </a>
         <a href="#"><li>首页</li> </a>
         <a href="#"><li>首页</li> </a>
         <a href="#"><li>首页</li> </a>
         <a href="#"><li>首页</li> </a>
         <a href="#"><li>首页</li> </a>
      </ul>
</div>

<div class="swiper-container" id="bannerSilde">
    <div class="swiper-wrapper">
        <div class=" banner swiper-slide"><img src="banner1.jpg"></div>
        <div class=" banner swiper-slide"><img src="banner2.jpg"></div>
        <div class="swiper-slide">Slide 3</div>
    </div>
       <div class="swiper-button-prev"></div>
       <div class="swiper-button-next"></div>
</div>

<div class="container">

         <div class="row">
              <div class="cols" id="cols1-1">
                 <div class="swiper-container" id="newSwiper">
                    <div class="swiper-wrapper">
                          <div class="swiper-slide"><img src="01.jpg" width="300" height="250"></div>
                          <div class="swiper-slide"><img src="02.jpg" width="300" height="250"></div>
                          <div class="swiper-slide"><img src="03.jpg" width="300" height="250"></div>
                    </div>
                          <div class="swiper-pagination"></div>
                          <div class="newTitle">标题</div>
              </div>
          </div>
              <div class="cols" id="cols1-2">
                 <ul>
        <li><span class="channel">[栏目]</span>&nbsp;&nbsp;&nbsp;<a href="#">标题</a><span class="datetime">2017/3/31</span></li>
        <li><span class="channel">[栏目]</span>&nbsp;&nbsp;&nbsp;<a href="#">标题</a><span class="datetime">2017/3/31</span></li>
        <li><span class="channel">[栏目]</span>&nbsp;&nbsp;&nbsp;<a href="#">标题</a><span class="datetime">2017/3/31</span></li>
        <li><span class="channel">[栏目]</span>&nbsp;&nbsp;&nbsp;<a href="#">标题</a><span class="datetime">2017/3/31</span></li>
        <li><span class="channel">[栏目]</span>&nbsp;&nbsp;&nbsp;<a href="#">标题</a><span class="datetime">2017/3/31</span></li>
        <li><span class="channel">[栏目]</span>&nbsp;&nbsp;&nbsp;<a href="#">标题</a><span class="datetime">2017/3/31</span></li>
        <li><span class="channel">[栏目]</span>&nbsp;&nbsp;&nbsp;<a href="#">标题</a><span class="datetime">2017/3/31</span></li>
                 </ul>
               </div>
              <div class="cols" id="cols1-3">
                   <span class="titleColor">学院概况</span>
                   <p>
                   网络传播学院是中国互联网新闻中心与浙江越秀外国语学院合办的中国互联网人才培养的重要基地，其培养目标是:为中国互联网行业培养高素质、高层次的互联网媒体新闻、经营、技术和管理人才。学院现有编辑出版学、传播学、新闻学、网络与新媒体和数字媒体艺术五个本科专业。
                   </p>
              </div>    
           </div>  
         <div class="row"></div>
         <div class="row"></div>
   </div> 
</body>

<script src="jquery-3.1.1.min.js"></script>
<script src="swiper.jquery.min.js"></script>
<script>        
  var mySlide = new Swiper ('#bannerSilde', {
    loop: true,
    nextButton: '.swiper-button-next',
    prevButton: '.swiper-button-prev',
  })        
    var width = $(document).width();
    var height = width *300/2000;
    $('#bannerSilde').css('height',height+'px');
	
 var newSwiper = new Swiper ('#newSwiper', {
       autoplay: 4000,//可选选项，自动滑动
       pagination : '.swiper-pagination',
       paginationType : 'progress',
       effect : 'fade'
   })

var swiperChildren =  $('#newSwiper .swiper-wrapper').children();
       swiperChildren.each(function () {
          $(this).children().attr({
                   "width":"300",
                   "height":"220"
           });
       })

</script>
</html>
