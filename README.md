# 爱奇异商城常用代码

## 一键拉扯图片
对于爱奇异的发布商品页面的反人类设计。调用CONSOLE模式，可以自动拉扯图片

    var jq = document.createElement('script');
    jq.src = "http://cdn.bootcss.com/jquery/1.11.1/jquery.min.js";
    document.getElementsByTagName('head')[0].appendChild(jq);
    jQuery.noConflict();
    $(function(){
        $('#ueditor_0').contents().find("img").css("width","100%");
        $('#ueditor_0').contents().find("img").css("height","100%");
    });
