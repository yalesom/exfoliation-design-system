> Cards visually articulate an element of content in a compact space.

# Card elements
## Primary content
All card types should, whenever possible, highlight a compelling image and a concise headline. Headlines and images should scale to fill the available space and be contextually sensitive to screen size.

## Metadata
Metadata represents the critical details necessary to give context to an individual card. Commonly:   
- *Date* — **when** was the content published
- *Author* — **who** authored to the content
- *Source* — **where** was the content published

While each metadatum should be visually distinct, sizes and styles should remain consistent to the parent application.

```hint
Although cards are typically displayed in the context of a slider, single card instances are permissible.
```
```image|plain
  src: "/exfoliation-design-system/assets/patterns/card-slider__sample.png"
  description: "Rendered example of a card slider"
```

# Card types
## Content cards
Most cards will be content cards. External sources should include a small, branded identifier from that source.
```html|span-3,plain,light
<ul class="card-slider__card-slot-list" data-min-height="true">
  <li class="card-slider__card-slot">
    <article id="card-id-941535" class="card-slider__card card-slider__card--internal_reference">
      <div class="card-slider__media" data-href="http://insights.som.yale.edu/insights/can-we-secure-online-identities" data-title="Can We Secure Online Identities? " data-main-image="https://som.yale.edu/sites/default/files/styles/yale_large_square_tile/public/insights/background/fingerprints.jpg?itok=vIUL6tht" data-target="_blank">
          <h2 class="card-slider__title" data-title="Can We Secure Online Identities? ">Can We Secure Online Identities? </h2>
          <img class="card-slider__badge-image" alt="Publication logo" src="https://som.yale.edu/sites/all/themes/common_assets/img/YaleInsights_bug.svg">
          <a class="no-icon" href="https://insights.som.yale.edu/insights/can-we-secure-online-identities"><img src="/exfoliation-design-system/assets/patterns/fingerprints.jpg" class="card-slider__media-image" alt="Can We Secure Online Identities?  card image" target="_blank"></a>
      </div>
      <div class="card-slider__meta-data">
        <span class="card-slider__meta-data__date">January 12, 2018</span>
        <span class="card-slider__meta-data__authors"><a href="//insights.som.yale.edu/single-contributor/24015">Sunil Madhu</a></span>
        <span class="card-slider__meta-data__source"><a href="http://insights.som.yale.edu" target="_blank">Yale Insights</a></span>
      </div>
    </article>
  </li>
</ul>
```
```html|span-3,plain,light
<ul class="card-slider__card-slot-list" data-min-height="true">
  <li class="card-slider__card-slot">
    <article id="card-id-942176" class="card-slider__card card-slider__card--internal_reference">
      <div class="card-slider__media card-slider__media--no-image" data-href="http://insights.som.yale.edu/insights/departing-pepsico-ceo-indra-nooyi-did-it-her-way" data-title="Prof. Jeffrey Sonnenfeld: PepsiCo CEO Indra Nooyi ’80 Did It Her Way" data-main-image="" data-target="_blank">
        <h2 class="card-slider__title" data-title="Prof. Jeffrey Sonnenfeld: PepsiCo CEO Indra Nooyi ’80 Did It Her Way">Prof. Jeffrey Sonnenfeld: PepsiCo CEO Indra Nooyi ’80 Did It Her Way</h2>
      </div>
      <div class="card-slider__meta-data">
        <span class="card-slider__meta-data__date">August 7, 2018</span>
        <span class="card-slider__meta-data__authors"><a href="//insights.som.yale.edu/single-contributor/8268">Jeffrey A. Sonnenfeld</a></span>
        <span class="card-slider__meta-data__source"><a href="https://som.yale.edu/about/recent-news" target="_blank">News</a></span>
      </div>
    </article>
  </li>
</ul>
```

## Social cards
Source provides slightly more context for this card type, so source metadata should be moved to the beginning of the stack. In addition, headlines are optional for this card type, especially when an visual is a self-contained context (i.e., Instagram).
#### Visual
```html|span-3,plain,light
<ul class="card-slider__card-slot-list" data-min-height="true">
  <li class="card-slider__card-slot">
    <article id="card-id-942198" class="card-slider__card card-slider__card--social card-slider__card--instagram">
        <div class="card-slider__media
        " data-href="https://www.instagram.com/p/BjX1hkHFMZ-" data-main-image="https://instagram.fphl2-4.fna.fbcdn.net/vp/5deaa50e54d6c4d1c3d5e0ac62fd9657/5C152D6A/t51.2885-15/sh0.08/e35/s640x640/33627109_216557572275428_1368073815376003072_n.jpg" data-title="instagram" data-main-image-source="external" data-target="_blank">
          <h2 class="card-slider__title"></h2>
          <a style="background-image:url(https://instagram.fphl2-4.fna.fbcdn.net/vp/5deaa50e54d6c4d1c3d5e0ac62fd9657/5C152D6A/t51.2885-15/sh0.08/e35/s640x640/33627109_216557572275428_1368073815376003072_n.jpg);" class="no-icon card-slider__media-image external" href="https://www.instagram.com/p/BjX1hkHFMZ-" target="_blank"></a>
        </div>
      <div class="card-slider__meta-data icon-instagram">
        <span class="card-slider__meta-data__authors"><a href="https://www.instagram.com/yalesom" target="_blank">yalesom</a></span>
        <span class="card-slider__meta-data__date">May 29, 2018</span>
      </div>
    </article>
  </li>
</ul>
```
```html|span-3,plain,light
<ul class="card-slider__card-slot-list" data-min-height="true">
  <li class="card-slider__card-slot">
    <article id="card-id-942200" class="card-slider__card card-slider__card--social card-slider__card--youtube">
      <div class="card-slider__media
      " data-href="http://youtu.be/-wnRNbNW4kg" data-main-image="https://i.ytimg.com/vi/-wnRNbNW4kg/hqdefault.jpg" data-title="youtube" data-main-image-source="external" data-target="_blank">
        <h2 class="card-slider__title">Meet the Full-time MBA Class of 2019</h2>
        <a style="background-image:url(https://i.ytimg.com/vi/-wnRNbNW4kg/hqdefault.jpg);" class="no-icon card-slider__media-image external" href="http://youtu.be/-wnRNbNW4kg" target="_blank"></a>
      </div>
      <div class="card-slider__meta-data icon-youtube-play">
        <span class="card-slider__meta-data__authors"><a href="http://www.youtube.com/channel/UC-NVYNjSpxgnZorM1t2TF1w" target="_blank">Yale School of Management</a></span>
        <span class="card-slider__meta-data__date">September 13, 2017</span>
      </div>
    </article>
  </li>
</ul>
```

#### Non-visual
Twitter represents a unique type of social card in that the primary visual is text. For non-visual cards, we transform the text into the visual element.
```html|span-3,plain,light
<ul class="card-slider__card-slot-list" data-min-height="true">
  <li class="card-slider__card-slot">
    <article id="card-id-942196" class="card-slider__card card-slider__card--social card-slider__card--twitter">
      <div class="card-slider__media
     card-slider__media--no-image" data-href="https://twitter.com/exfoliation-design-system/status/1031559786419154944" data-main-image="" data-title="twitter" data-target="_blank">
        <h2 class="card-slider__title">RT <a target="_blank" rel="nofollow" class="twitter-timeline-link" href="http://twitter.com/DBachGlobal">@DBachGlobal</a>: And we’re off! Dean <a target="_blank" rel="nofollow" class="twitter-timeline-link" href="http://twitter.com/EdwardASnyder">@EdwardASnyder</a> welcomes 70 new MAMs, 11 Systemic Risk students and the 32 members of our first… <a href="https://t.co/v0nS98XkiY">https://t.co/v0nS98XkiY</a></h2>
        <div class="card-slider__author-block">
          <a href="http://twitter.com/YaleSOM" target="_blank"><img class="card-slider__author-block__avatar" src="//pbs.twimg.com/profile_images/877910548100329472/ENIm5pUS_normal.jpg"></a> 								
          <div class="card-slider__author-block__name"><a href="http://twitter.com/YaleSOM" class="no-icon" target="_blank">Yale SOM</a></div>
          <div class="card-slider__author-block__handle"><a href="http://twitter.com/YaleSOM" class="no-icon" target="_blank">@YaleSOM</a></div> 		
        </div>
        <div class="card-slider__timestamp"><em class="placeholder">2 weeks 1 day</em> ago</div>
        <a class="no-icon" href="https://twitter.com/exfoliation-design-system/status/1031559786419154944" target="_blank"></a>
      </div>
      <ul class="card-slider__meta-data__social-share icon-linearicon social-share--list">
        <li><a href="http://twitter.com/intent/tweet?in_reply_to=1031559786419154944" target="_blank" class="icon--reply no-icon"></a></li>
        <li><a href="http://twitter.com/intent/retweet?tweet_id=1031559786419154944" target="_blank" class="icon--repeat no-icon"></a></li>
        <li><a href="http://twitter.com/intent/favorite?tweet_id=1031559786419154944" target="_blank" class="icon--star no-icon"></a></li>
      </ul>
      <div class="card-slider__meta-data icon-twitter">
        <span class="card-slider__meta-data__authors"><a href="http://twitter.com/YaleSOM" class="no-icon" target="_blank">@YaleSOM</a></span>
      </div>
    </article>
  </li>
</ul>
```
