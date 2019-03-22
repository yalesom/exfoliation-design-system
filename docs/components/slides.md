> **Slides** introduce more complex stories through rich media. Slides are defined by dynamic movement and are typically self-contained content elements, although linking to deeper content is permissible.

# Anatomy
```image|plain,span-6
src: "/exfoliation-design-system/assets/components/slide-anatomy.png"
```
## Elements

**Headline**
*(required)* Headlines should be concise so as not to conflict with media content. Text always is animated, overlaps the media region and is most commonly is aligned to the left and bottom of the container. 

**Media**
*(required)* Video is preferred, as it has greater potential for narrative, but static images are permissible. 

**Description/byline**
*(optional)*  Provides additional context to a slide.

**Pagination**
*(required for multiple)* Sliders with multiple slides should have a non-numeric pagination. Remove pagination for single slide instances.

**Controls**
*(required for video)*  Required [success criterion] for WCAG 2.0 Level A


# Specimens
```html|plain,light,no-source
<div id="media-slider-2396" class="media-slider media-slider--slideshow sliderLoaded" aria-labelledby="media-slider-2396_title">
<ul class="media-slider__media-list">
<li id="media-slot-140797" class="media-slider__media-slot media-slider__media-slot--active" data-type="video" aria-hidden="false">
<div class="media-slider__media">
<div class="media-slider__media-wrapper" data-href="http://insights.som.yale.edu/insights/how-fair-is-american-society" data-title="" data-ischrome="true">
<h2 class="media-slider__title">Economic Inequality</h2>
<div class="media-slider__object">
<video class="media-slider__video" data-video-id="5579506689001" data-video-name="Michael Kraus on the Misperception of Racial Economic Equality - Data" data-title="Economic Inequality" poster="/exfoliation-design-system/assets/components/Kraus_titleslide.jpg" src="/exfoliation-design-system/assets/components/1822790495001_5579531340001_5579506689001.mp4" autoplay="true"></video>
<img class="media-slider__video_poster media-slider__video_poster--playing" src="/exfoliation-design-system/assets/components/Kraus_titleslide.jpg">
</div>
</div>
<div class="media-slider__meta-data">
<span class="media-slider__meta-data__caption">Americans tend to be overly optimistic about economic equality between white and black citizens, according to a new study by Yale researchers.
</span>
</div>
</div>
</li>
</ul>
</div>
```
```hint|neutral
**Video slide**
Video slides are intended to summarize a topic and **not** be full length videos. Maximum video length should be around 15 seconds.
```

## Variants
```html|plain,light,no-source
<div id="media-slider-2396" class="ysm-slider slider-marquee slider-profile entity-paragraphs-item ysm-slider--has-pager slider-marquee--slideshow sliderLoaded" aria-labelledby="media-slider-2396_title">
<ul class=""ysm-slider__list">
<li id="media-slot-140797" class="ysm-slider__slot ysm-slider__slot--active" data-type="video" aria-hidden="false">
<article class="ysm-slider__media" data-type="image">
<div class="ysm-slider__wrapper" data-href="https://som.yale.edu/profile/xerxes-mullan-02" data-title="" tabindex="0">
<h2 class="ysm-slider__title slider-profile__title"><span class="slider-profile__title-overlay">SOM really has that right balance of business and society. It really is one of those unique institutions that shows you both sides of the coin. </span></h2>          <div class="ysm-slider__object">
<figure class="ysm-slider__figure"><img src="/exfoliation-design-system/assets/components/XerxesMullan.jpg" width="1280" height="720" alt="" title="" class="ysm-slider__image"></figure>
</div>
</div>
<footer class="ysm-slider__meta-data">
<figcaption class="ysm-slider__meta-data__byline"><a href="https://som.yale.edu/profile/xerxes-mullan-02" tabindex="0" aria-hidden="false">Xerxes Mullan '02 on societal impact</a></figcaption>
</footer>
</article>
</li>
</ul>
</div>
```

```hint|neutral
**Profile slide**
Profile slides are less animated because of a greater focus on reading longer quotation. Headline style is updated to reflect the shift in priority between headline and media.
```
## Markup
Import the following components to use the preferred markup pattern for slides:
`@import "~yale-som-theme/scss/components/ysm-slider/ysm-slider-config";`
`@import "~yale-som-theme/scss/components/ysm-slider/ysm-slider";`
```code|lang-html
<article class="ysm-slider__media" data-type="video">
  <button class="ysm-slider__audio ysm-slider__audio--muted" 
    tabindex="0" aria-hidden="false"></button>
  <div class="ysm-slider__wrapper" data-href="#" data-title="" tabindex="0">
    <h2 class="ysm-slider__title slider-media__title">Careers</h2>
    <div class="ysm-slider__object">
      <video class="ysm-slider__video" data-video-id="5668698051001" 
        data-title="Slide headline" src="example.mp4" 
        data-video-name="Video title" poster=""></video>
      <img class="ysm-slider__video_poster" 
        aria-role="presentation" src="example.jpg">
    </div>
  </div>
  <footer class="ysm-slider__meta-data">
    <span class="ysm-slider__meta-data__caption">
    Americans tend to be overly optimistic about economic equality 
    between white and black citizens, according to a new study 
    by Yale researchers.
    </span>
  </footer>
</article>
```
# Usage

## Media slider
In contrast to [Cards], Media slides should only be presented in the context of a slider.
```image|plain
src: "/exfoliation-design-system/assets/components/media-slider__sample.png"
```
## Profile slide
Profile slides can be displayed individually, or as a slide grouping.
```image|plain
src: "/exfoliation-design-system/assets/components/profile-slider__sample.png"
```

[cards]: /components/cards
[success criterion]: https://www.w3.org/TR/UNDERSTANDING-WCAG20/time-limits-pause.html
