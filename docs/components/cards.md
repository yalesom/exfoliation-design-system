> **Cards** visually articulate a single topic with a minimum of information. They should be simple, actionable and easy to scan.

# Anatomy
```image|plain,span-4
src: "/exfoliation-design-system/assets/components/card-anatomy.png"
```

## Elements

**Headline**
*(required)* Header text is the only required element of a card. Headlines should scale to fill the available container space and be concise so as not to conflict with image content. Text always is contained inside the image region and is most commonly is aligned to the left and bottom of the container. 

**Image**
*(preferred)* All card types should, whenever possible, highlight a compelling image. 

**Metadata**
*(optional)* Metadata represents the critical details necessary to give context to an individual card. Commonly:   
- *Date* — when was the content published
- *Author* — who authored to the content
- *Source* — where was the content published

While each metadatum should be visually distinct, sizes and styles should remain consistent to the parent application.

**Description**
*(optional)*  Provides additional context to a card where the headline/image is insufficient. Descriptions should be brief (maximum of 4 lines). Desrciptions should not be used in conjuction with Metadata.

**Source logo**
*(optional)*  External sources may be called out by a small, branded identifier in the upper right of the card.

# Specimens

```html|span-4,plain,light,no-source
<ul class="card-slider__card-slot-list" data-min-height="true">
<li class="card-slider__card-slot">
<article id="card-id-941535" class="card-slider__card card-slider__card--internal_reference">
<div class="card-slider__media" data-href="http://insights.som.yale.edu/insights/can-we-secure-online-identities" data-title="Can We Secure Online Identities? " data-main-image="/exfoliation-design-system/assets/components/fingerprints.jpg" data-target="_blank">
<h2 class="card-slider__title" data-title="Can We Secure Online Identities? ">Can We Secure Online Identities? </h2>
<img class="card-slider__badge-image" alt="Publication logo" src="https://som.yale.edu/sites/all/themes/common_assets/img/YaleInsights_bug.svg">
<a class="no-icon" href="https://insights.som.yale.edu/insights/can-we-secure-online-identities"><img src="/exfoliation-design-system/assets/components/fingerprints.jpg" class="card-slider__media-image" alt="Can We Secure Online Identities?  card image" target="_blank"></a>
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
```hint|neutral,span-2
**Content card**
Most cards will be content cards and link to another page. Images should darken and blur on interactions to improve headline legibility for the focused element.
```
```html|span-4,plain,light,no-source
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
```hint|neutral,span-2
**Non-image content card**
Cards without associated visual media should reverse the contrast relationship of headline to background to put greater emphasis on text. Cards of this type should also have an alternate hover/focus effect.
```
## Variants
```html|span-4,plain,light
<ul class="card-slider__card-slot-list" data-min-height="true">
<li class="card-slider__card-slot">
<article id="card-id-942198" class="card-slider__card card-slider__card--social card-slider__card--instagram">
<div class="card-slider__media
" data-href="https://www.instagram.com/p/BjX1hkHFMZ-" data-main-image="/exfoliation-design-system/assets/components/33627109_216557572275428_1368073815376003072_n.jpg" data-title="instagram" data-main-image-source="external" data-target="_blank">
<h2 class="card-slider__title"></h2>
<a style="background-image:url(/exfoliation-design-system/assets/components/33627109_216557572275428_1368073815376003072_n.jpg);" class="no-icon card-slider__media-image external" href="https://www.instagram.com/p/BjX1hkHFMZ-" target="_blank"></a>
</div>
<div class="card-slider__meta-data icon-instagram">
<span class="card-slider__meta-data__authors"><a href="https://www.instagram.com/yalesom" target="_blank">yalesom</a></span>
<span class="card-slider__meta-data__date">May 29, 2018</span>
</div>
</article>
</li>
</ul>
```
```hint|neutral,span-2
**Image-only social card**
Source provides slightly more context for this card type, so source metadata should be moved to the beginning of the stack. In addition, headlines are optional for this card type, especially when an visual is a self-contained context (i.e., Instagram).
```
```html|span-4,plain,light,no-source
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
```hint|neutral,span-2
**Non-image social card**
Twitter represents a unique type of social card in that the primary visual is text. For non-visual cards, we transform the text into the visual element.
```
## Markup
Import the following components to use the preferred markup pattern for content cards:
`@import "~yale-som-theme/scss/components/_cards";`
`@import "~yale-som-theme/scss/components/_metadata";`
```code|lang-html
<article class="node card">
  <header class="card__object card--has-url" data-dynamic-font-size="true" style="font-size: 301px;">
    <h2 class="card__title">Get connected</h2>
      <div class="card__media">
        <a href="#" class="no-icon" aria-label="Continue reading Get connected">
          <img class="card__image" aria-role="presentation" 
            src="example.jpg" alt="Students around conference table" 
            title="" />
        </a>
      </div>
  </header>
  <div class="card__metadata metadata metadata--flat">
    <span class="card__metadata__date metadata__item">February 25, 2019</span>
    <span class="card__metadata__authors metadata__item">
      <a href="#">Ranji Nagaswami</a>
    </span>
    <span class="card__metadata__source metadata__item">
      <a href="#" target="_blank">Yale Insights</a>
    </span>
  </div>
</article>
```

```code|lang-js,span-4
YaleSOM.dynamicFontSize = function () {
  $('[data-dynamic-font-size=true]').each(function () {
    $(this).css('font-size', $(this).outerWidth());
  });
};
```
```hint|neutral,span-2
**Dynamic font scaling**
In most contexts, card headlines should scale relative to the containing element. This can be accomplished with the provided JavaScript function, which will change the font-size methodology from breakpoints to inherited font size.  
```
# Usage
## Card slider
```image|plain
src: "/exfoliation-design-system/assets/components/card-slider__sample.png"
```

## Card stack
```image|plain
src: "/exfoliation-design-system/assets/components/image2019-1-17_15-5-8.png"
```
## Card teaser
```image|plain
src: "/exfoliation-design-system/assets/components/image2019-1-17_14-59-43.png"
```
## Card grid
```image|plain
src: "/exfoliation-design-system/assets/components/card-grid.png"
```
