> Icons are primarily used in Exfoliation for UI enhancement and to promote clarity on action items.  

Icon fonts can be downloaded in the [resources] section. Most icon instances are applied via CSS with the following [mixin].

# Linearicons

[Linearicons] is the default icon library for all UI.

```image|plain,dark
src: "/exfoliation-design-system/assets/brand/linearicons-sample.svg"
title: "Sample of library"
```

```hint
Many of the icons in the full set are impractical for general use so Exfoliation uses a custom repackaging of the original webfont (via [IcoMoon](https://linearicons.com/) app) to exclude unnecessary glyphs.
```

## Available icon classes
Selected icons can be applied inline by including a class on an element:
```html|plain,dark
<div style="color:#fff; font-size:2rem;">
  <span class="icon-video"/>  
  <span class="icon-network"/>  
  <span class="icon-linearicon icon--magnifier"/>  
  <span class="icon--reply"/>  
  <span class="icon--repeat"/>  
  <span class="icon--star"/>  
  <span class="icon-linearicon icon--mic"/>  
  <span class="icon-linearicon icon--check"/>  
  <span class="icon-linearicon icon--earth"/>  
  <span class="icon-linearicon icon--papers"/>  
  <span class="icon-linearicon icon--arrow-left-circle"/>  
  <span class="icon-linearicon icon--arrow-right-circle"/>  
  <span class="icon-linearicon icon--border-outer"/>  
</div>
```
**Sample of icons via class**

# Fontello
Social icons are single webfont generated via [Fontello] that combines icons from different libraries. The custom library contains specific social channels where Yale SOM participates as well as other common channels.
```html|dark,plain
<div style="color:#fff; font-size:2rem;">
  <span class="icon-facebook"/>  
  <span class="icon-facebook-official"/>  
  <span class="icon-flickr"/>  
  <span class="icon-gplus"/>  
  <span class="icon-linkedin"/>  
  <span class="icon-pinterest-circled"/>  
  <span class="icon-tencent-weibo"/>  
  <span class="icon-tumblr"/>  
  <span class="icon-twitter"/>  
  <span class="icon-vine"/>  
  <span class="icon-wechat"/>  
  <span class="icon-weibo"/>  
  <span class="icon-xing"/>  
  <span class="icon-youtube-play"/>  
  <span class="icon-share"/>  
  <span class="icon-pinterest"/>  
  <span class="icon-instagram"/>  
  <span class="icon-vimeo"/>  
  <span class="icon-tudou"/>  
  <span class="icon-youku"/>  
  <span class="icon-rss"/>  
  <span class="icon-slack"/>  
  <span class="icon-yahoo"/>  
  <span class="icon-whatsapp"/>  
  <span class="icon-skype"/>  
  <span class="icon-slideshare"/>
</div>
```
**Sample of icons via class**


[linearicons]: https://linearicons.com/
[icomoon]: https://icomoon.io/app/#/select
[fontello]: http://fontello.com/
[mixin]:https://bitbucket.org/sq360_sysadmin/yale-som-theme/src/master/scss/core/mixins/_icon.scss
[resources]: /resources
