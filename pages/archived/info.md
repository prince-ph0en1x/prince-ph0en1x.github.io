---
layout: page
title: "Last update"
subheadline: "Housekeeping info"
teaser: "when was this website last updated"
permalink: "/info/"
header:
    image_fullwidth: "header_drop.jpg"
---

<div id='commits' data-path='master'></div>
<script src='https://code.jquery.com/jquery-2.2.1.min.js'></script>
<script>
var path = $('#commits').data('path');
var url = 'https://api.github.com/repos/prince-ph0en1x/prince-ph0en1x.github.io/commits?path='+path;
        url:url,
        success: function(data){
    var str="<table class='docutils'><thead><tr><th>message</th><th>date</th><th>author</th><th>link</th></tr></thead><tbody>";
    for(var idx=0;idx<data.length && idx<10;idx++){
      var one = data[idx];
      var d = one.commit.author.date.substr(0,10);
      var t = one.commit.author.date.substr(11,10);
      str+="<tr><td>"+one.commit.message+"</td><td>"
          +d+" "+t+"</td><td>"
          +one.commit.author.name+"</td><td>"
          +"<a href='"+one.html_url+"'>"+one.sha.substr(0,7)+"</a></td></tr>";
    }
    str+="</tbody></table>";
    $('#commits').html(str);
}});
</script>

