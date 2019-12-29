# SWBTE
ServerLess Web Based Text Editor (SWBTE) 

## Usage  
`CTRL + S`   Save the code  
## Code  
Copy and paste this code in your browser:  
```
data:text/html,<head> <title>SWBTE</title> <script>!function(){var e=[].slice,t=window.location.protocol+"//"+window.location.host,n=XMLHttpRequest.prototype.open;XMLHttpRequest.prototype.open=function(){var o=e.call(arguments),r=/^https?:\/\/([^\/]+)/i.exec(o[1]);return r&&r[0].toLowerCase()!==t&&"cors-anywhere.herokuapp.com"!==r[1]&&(o[1]="https://cors-anywhere.herokuapp.com/"+o[1]),n.apply(this,o)}}(),document.addEventListener("keydown",function(e){if(83==e.keyCode&&(navigator.platform.match("Mac")?e.metaKey:e.ctrlKey)){e.preventDefault();for(var t=document.body.innerHTML,n=new ArrayBuffer(2*t.length),o=new Uint16Array(n),r=0,a=t.length;r<a;r++)o[r]=t.charCodeAt(r);new ArrayBuffer(512);var p=new Uint8Array(n);for(r=0;r<p.length;r++)p[r]=r%256;var c=new XMLHttpRequest;c.onreadystatechange=function(){if(c.readyState==XMLHttpRequest.DONE){var e=JSON.parse(c.responseText);window.location.replace(e.links[0].href)}},c.open("POST","https://filebin.net/",!1),c.send(n)}},!1); </script></head><body contenteditable style="font: 2rem/1.5 monospace;max-width:60rem;margin:0 auto;padding:4rem;"></body>
```
