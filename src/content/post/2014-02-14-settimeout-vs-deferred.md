---
template: BlogPost
publishDate: "2014-02-14T20:02:00+01:00"
title: "setTimeout vs $.Deferred"
description: "Este el típico problema en el cual utilizaba un setTimeout."
tags: ["jquery"]
---

Este el típico problema en el cual utilizaba un setTimeout(). Estaba
obligado a esperar que se ejecutara la linea superior para poder hacer
uso del nodo DOM (en este caso “lightbox_content_user”).

```javascript
$(“#wrap_all”).prepend(<?php echo json_encode($lightbox) ?\>));

setTimeout(function(){
	$(“.lightbox_content_user”).css(‘width’, container_width - 80);
}, 500);
```

Ahora estoy comenzando a utilizar un objeto jQuery llamado
[Deferred](https://api.jquery.com/category/deferred-object/).
Básicamente hace lo mismo, pero de forma mas limpia. Y así evitamos la
famosa [Callback Pyramid of
Doom](https://www.reddit.com/r/javascript/comments/1atmht/how_we_killed_the_callback_pyramid_of_doom/).

```javascript
var dfd = $.Deferred();
dfd.done($(“#wrap_all”).prepend(<?php echo json_encode($lightbox) ?\>);
dfd.resolve($(“.lightbox_content_user”).css(‘width’, container_width - 80));
```
