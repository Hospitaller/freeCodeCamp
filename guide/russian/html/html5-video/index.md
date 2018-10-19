
---
title: HTML5 Video
localeTitle: Видео HTML5
---
## Видео HTML5

До появления HTML5, чтобы отобразить игру или видео на веб-странице, вам нужно было использовать плагин, например Adobe Flash Player. С введением HTML5 вы можете разместить его непосредственно на самой странице. HTML-код тег используется для встраивания видео в веб-документы. Он может содержать один или несколько источников видео, представленных с использованием атрибута src или [исходного](source) элемента.

Чтобы вставить видеофайл в веб-страницу, просто добавьте этот фрагмент кода и измените src аудиофайла.
```
<video controls width="400" height="300">
  <source src="video.mp4" type="video/mp4"><!-- MP4 для Safari, IE9, iPhone, iPad, Android, и Windows Phone 7 -->
  <source src="video.webm" type="video/webm"><!-- WebM/VP8 для Firefox4, Opera, и Chrome -->
  <source src="video.ogv" type="video/ogg"><!-- Ogg/Vorbis для старых версий браузеров Firefox и Opera -->
  <object data="video.swf" type="application/x-shockwave-flash"><!-- добавляем видеоконтент для устаревших браузеров, в которых нет поддержки элемента video -->
    <param name="movie" value="video.swf">
  </object>
</video>
```
 Html 5 video поддерживают все современные браузеры, однако стоит учитывать формат видео.
 Существует три самых распространенных формата -  MP4, WebM, и Ogg.
 
 Тэг **`<source>`** используется для указания нескольких источников видео и аудио. Браузер автоматически определяет поддерживаемые типы носителей или кодеков



 
 #### autoplay 
 
 "autoplay" может принимать два значения - *true* и *false*. По умолчанию принимает значение *false*. Значение *true* заставляет видео запускаться автоматически, при достижении определенного порога кэширования. Многие считают автозапуск видео на странице раздражающим, поэтому рекомендуем не злоупотреблять им. Стоит заметить, что некоторые мобильные браузеры, такие как Safari для iOS, и вовсе игнорируют этот атрибут.
```

<video src="pr6.webm" width="320" height="240" autoplay></video>

  
```
#### poster 
 
 Атрибут "poster" принимает URL изображения, которое будет отображаться во время загрузки видеофайла или до тех пор, пока пользователь не нажмет на кнопку PLAY. Если атрибут не задан, то будет отображаться первый кадр видеофайла.
 
 #### controls 
 
 Атрибут "controls" указывает браузеру, что нужно отобразить базовые элементы управления воспроизведением (воспроизведение, пауза, громкость).
```

<video width="400" height="300" controls poster="video/duel.jpg">
	<source src="video/duel.ogv" type='video/ogg; codecs="theora, vorbis"'>
	<source src="video/duel.mp4" type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"'>
	<source src="video/duel.webm" type='video/webm; codecs="vp8, vorbis"'>
Тег video не поддерживается вашим браузером. <a href="video/duel.mp4">Скачайте видео</a>. </video>
```




Есть много других атрибутов, которые можно добавить, которые необязательны для настройки видеоплеера на странице. Чтобы узнать больше, нажмите на ссылки ниже.

## Дополнительная информация:

*   [W3Schools - HTML5 Видео](https://www.w3schools.com/html/html5_video.asp)
*   [Веб-документы Mozilla - Видео](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/video)
*   [Википедия - HTML5 Видео](https://en.wikipedia.org/wiki/HTML5_video)
*   [HTML5 Rocks - HTML5 Video](https://www.html5rocks.com/en/tutorials/video/basics/)
*   [Могу ли я использовать видео?](https://caniuse.com/#search=video)
*   [Как использовать HTML5 для воспроизведения видеофайлов на своей веб-странице](https://docs.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/samples/hh924821(v=vs.85))
