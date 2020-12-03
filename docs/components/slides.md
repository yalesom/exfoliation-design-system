> **Slides** introduce more complex stories through rich media. Slides are defined by dynamic movement and are typically self-contained content elements, although linking to deeper content is permissible.

# Anatomy

```image|plain,span-6
src: "/exfoliation-design-system/assets/components/slide-anatomy.png"
```

## Elements

**Headline**
_(required)_ Headlines should be concise so as not to conflict with media content. Text always is animated, overlaps the media region and is most commonly is aligned to the left and bottom of the container.

**Media**
_(required)_ Video is preferred, as it has greater potential for narrative, but static images are permissible.

**Description/byline**
_(optional)_ Provides additional context to a slide.

**Pagination**
_(required for multiple)_ Sliders with multiple slides should have a non-numeric pagination. Remove pagination for single slide instances.

**Controls**
_(required for video)_ Required [success criterion] for WCAG 2.0 Level A

# Specimens

```html|plain,light
<section id="ysm-slider-15139" class="ysm-slider ysm-slider--marquee ysm-slider--media entity-paragraphs-item ysm-slider--has-pager ysm-slider--marquee--slideshow sliderLoaded" aria-labelledby="ysm-slider-15139_title" data-pid="15139">
      <h2 id="paragraphs-item--title-15139" class="paragraphs-item__title  gamma">Highlights from Yale SOM</h2>
      <div class="ysm-slider__bx-wrapper" style="max-width: 100%;">
      <div class="bx-viewport" aria-live="polite">
      <ul class="ysm-slider__list">
          <li id="ysm-slider__slot-227745-4" class="ysm-slider__slot" aria-hidden="true">
    <article class="ysm-slider__media" data-type="video">
    <div class="ysm-slider__wrapper" data-href="https://som.yale.edu/news/2020/05/faculty-describe-challenges-and-lessons-learned-in-the-virtual-classroom" data-title="" tabindex="0">
    <h2 class="ysm-slider__title ysm-slider__title--media">#VirtualYale Connections</h2>
    <div class="ysm-slider__object">
              <video class="ysm-slider__video" data-title="#VirtualYale Connections" src="https://player.vimeo.com/external/425602187.sd.mp4?s=7db4b52e28c3dfd9111839381a75c5080c68188e&amp;profile_id=165&amp;oauth2_token_id=1248300143" poster="https://i.vimeocdn.com/video/904315878_1280x720.jpg?r=pad"></video>
        <img class="ysm-slider__video_poster" aria-role="presentation" alt="" src="https://i.vimeocdn.com/video/904315878_1280x720.jpg?r=pad">
          </div>
  </div>
  <footer class="ysm-slider__meta-data">
    <span class="ysm-slider__meta-data__caption"><p>Professor Rodrigo Canales and other faculty members discuss their experiences teaching online.&nbsp;</p>
</span>
  </footer>
</article>
  </li>
    </ul></div><div class="bx-controls bx-has-pager has-controls"><div class="bx-pager bx-default-pager"><div class="bx-pager-item"><a href="" data-slide-index="0" class="bx-pager-link">1</a></div><div class="bx-pager-item"><a href="" data-slide-index="1" class="bx-pager-link active">2</a></div><div class="bx-pager-item"><a href="" data-slide-index="2" class="bx-pager-link">3</a></div><div class="bx-pager-item"><a href="" data-slide-index="3" class="bx-pager-link">4</a></div></div><button class="ysm-slider__toggle icon-linearicon icon--border-outer" aria-label="Toggle presentation view"></button><button class="ysm-slider__playstate ysm-slider__playstate--play" aria-label="Pause playback"></button></div></div>
    </section>
```

```hint|neutral
**Video slide**
Video slides are intended to summarize a topic and **not** be full length videos. Maximum video length should be around 15 seconds.
```

## Variants

```html|plain,light
<div id="media-slider-2396" class="ysm-slider ysm-slider--marquee ysm-slider--profile entity-paragraphs-item ysm-slider--marquee--slideshow sliderLoaded" aria-labelledby="media-slider-2396_title">
<ul class="ysm-slider__list">
<li id="media-slot-140797" class="ysm-slider__slot ysm-slider__slot--active" data-type="video" aria-hidden="false">
<article class="ysm-slider__media" data-type="image">
<div class="ysm-slider__wrapper" data-href="https://som.yale.edu/profile/xerxes-mullan-02" data-title="" tabindex="0">
<h2 class="ysm-slider__title ysm-slider__title--profile"><span class="ysm-slider__title--overlay">SOM really has that right balance of business and society. It really is one of those unique institutions that shows you both sides of the coin. </span></h2>          <div class="ysm-slider__object">
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
