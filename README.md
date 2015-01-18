# hashtags.js
Make hashtags on your site like facebook and twitter
# How To Use It
Simple String Replace Example:
Let's replace hashtag keywords with url :
In this example we replace @@@ in ``` <a href='http://www.site.com/hashtag.php?hashtag=@@@'>@@@</a> ``` with the keyword then 
replace keyword with this link .
```javascript
x = ("I love #javascript and #php").parseHashtag("<a href='http://www.site.com/hashtag.php?hashtag=@@@'>@@@</a>","@@@");
```
Callback function Example:
Let's Count Hashtag keywords :

```javascript
var count=0;
"#hello #word #i'm #very #happy".parseHashtag(function(tag){
    count++
  });
 console.log(count);
 ```
Let's replace keywords with url :

```javascript

"#hello #word #i'm #very #happy".parseHashtag(function(tag){
      return 'http://www.site.com/hashtag.php?hashtag='+tag;
  });

 ```
# Author
Mahdi Jouini
