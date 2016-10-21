# Put logos on your gif the easy way!
=
 go to  https://raphael-abreu.github.io/Gif-bookmarklets !


javascript:(function(s){try{s=document.selection.createRange().text}catch(_){s=document.getSelection()}loadUrl('http://ezgif.com/overlay?url='+location.href)})()

javascript:(function(s){try{s=document.selection.createRange().text}catch(_){s=document.getSelection()}window.location="http://ezgif.com/overlay?url="+location.href+""})()


$.ajax({
    type: 'POST',
    url: 'http://upload.giphy.com/v1/gifs',
    data: {
        api_key: 'dc6zaTOxFJmzC',
        source_image_url: window.location.href,
    },
success: function(data) { prompt('copie esse link' ,"https://media.giphy.com/media/"+data.data.id+"/giphy.gif"); },    error: console.log("algo deu errado")
});



javascript:(function(){function callback(){(function($){var jQuery=$;$.ajax({type: 'POST',url: 'http://upload.giphy.com/v1/gifs',data: {api_key: 'dc6zaTOxFJmzC',source_image_url: 'window.location.href',},success: function(data) { prompt('copie esse link' ,"https://media.giphy.com/media/"+data.data.id+"/giphy.gif"); },})})(jQuery.noConflict(true))}var s=document.createElement("script");s.src="https://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js";if(s.addEventListener){s.addEventListener("load",callback,false)}else if(s.readyState){s.onreadystatechange=callback}document.body.appendChild(s);})()')
