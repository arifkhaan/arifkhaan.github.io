---
layout: page
title: Gallery
subtitle: 
---



<blockquote class="instagram-media" data-instgrm-permalink="https://www.instagram.com/p/BmeNh7wAddr/?utm_source=ig_embed" data-instgrm-version="9" style=" background:#FFF; border:0; border-radius:3px; box-shadow:0 0 1px 0 rgba(0,0,0,0.5),0 1px 10px 0 rgba(0,0,0,0.15); margin: 1px; max-width:540px; min-width:326px; padding:0; width:99.375%; width:-webkit-calc(100% - 2px); width:calc(100% - 2px);"><div style="padding:8px;"> <div style=" background:#F8F8F8; line-height:0; margin-top:40px; padding:50% 0; text-align:center; width:100%;"> <div style=" background:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACwAAAAsCAMAAAApWqozAAAABGdBTUEAALGPC/xhBQAAAAFzUkdCAK7OHOkAAAAMUExURczMzPf399fX1+bm5mzY9AMAAADiSURBVDjLvZXbEsMgCES5/P8/t9FuRVCRmU73JWlzosgSIIZURCjo/ad+EQJJB4Hv8BFt+IDpQoCx1wjOSBFhh2XssxEIYn3ulI/6MNReE07UIWJEv8UEOWDS88LY97kqyTliJKKtuYBbruAyVh5wOHiXmpi5we58Ek028czwyuQdLKPG1Bkb4NnM+VeAnfHqn1k4+GPT6uGQcvu2h2OVuIf/gWUFyy8OWEpdyZSa3aVCqpVoVvzZZ2VTnn2wU8qzVjDDetO90GSy9mVLqtgYSy231MxrY6I2gGqjrTY0L8fxCxfCBbhWrsYYAAAAAElFTkSuQmCC); display:block; height:44px; margin:0 auto -44px; position:relative; top:-22px; width:44px;"></div></div><p style=" color:#c9c8cd; font-family:Arial,sans-serif; font-size:14px; line-height:17px; margin-bottom:0; margin-top:8px; overflow:hidden; padding:8px 0 7px; text-align:center; text-overflow:ellipsis; white-space:nowrap;"><a href="https://www.instagram.com/p/26Mu24mhCa/?utm_source=ig_embed" style=" color:#c9c8cd; font-family:Arial,sans-serif; font-size:14px; font-style:normal; font-weight:normal; line-height:17px; text-decoration:none;" target="_blank">A post shared by Arif Ullah Khan (@aarif_ullah_khan)</a> on <time style=" font-family:Arial,sans-serif; font-size:14px; line-height:17px;" datetime="2015-05-20T15:49:31+00:00">May 20, 2015 at 8:49am PDT</time></p></div></blockquote> <script async defer src="//www.instagram.com/embed.js"></script>

<div class="myExMul" >
    <a href="image1_b.jpg" rel="myExMul-1">
        <img alt="title 1" src="img/photos/arif3.jpg" />
    </a>
    <a href="image2_b.jpg" rel="myExMul-1">
        <img alt="title 2" src="img/photos/10437437_1237194076308109_352005160891353053_n.jpg" />
    </a>
    ...
</div>
<div class="myExMul" >
    <a href="image3_b.jpg" rel="myExMul-2">
        <img alt="title 3" src="img/photos/group1.jpg" />
    </a>
    <a href="image4_b.jpg" rel="myExMul-2">
        <img alt="title 4" src="img/photos/group1.jpg" />
    </a>
    ...
</div>
<div class="myExMul" >
    <a href="image5_b.jpg" rel="myExMul-3">
        <img alt="title 5" src="img/photos/group1.jpg" />
    </a>
    <a href="image6_b.jpg" rel="myExMul-3">
        <img alt="title 6" src="img/photos/group1.jpg" />
    </a>
    ...
</div>

$('.myExMul').justifiedGallery({
    rowHeight : 50 
}).on('jg.complete', function () {
    $(this).find('a').colorbox({
        maxWidth : '80%',
        maxHeight : '80%',
        opacity : 0.8,
        transition : 'elastic',
        current : ''
    });
});
$('.myExMul').each(function (i, el) {
    $(el).justifiedGallery({rel: 'myExMul-' + i}).on('jg.complete', function () {
        $(this).find('a').colorbox({
            maxWidth : '80%',
            maxHeight : '80%',
            opacity : 0.8,
            transition : 'elastic',
            current : ''
        });
    });
});
