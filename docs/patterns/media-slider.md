> Media slides are a method to introduce more complex stories without adding extraneous content.

```image|plain
  src: "yalesom/assets/patterns/media-slider__sample.png"
  description: "Rendered example of a media slider"
```
In contrast to [Cards], Media Slides should only be presented in the context of the slider.

# Slide
## Video
Video is preferred for slides as it has greater potential for narrative.
```html|plain,light
<div id="media-slider-2396" class="media-slider media-slider--slideshow sliderLoaded" aria-labelledby="media-slider-2396_title">
  <ul class="media-slider__media-list">
    <li id="media-slot-140797" class="media-slider__media-slot media-slider__media-slot--active" data-type="video" aria-hidden="false">
      <div class="media-slider__media">
        <div class="media-slider__media-wrapper" data-href="http://insights.som.yale.edu/insights/how-fair-is-american-society" data-title="" data-ischrome="true">
          <h2 class="media-slider__title">Economic Inequality</h2>
          <div class="media-slider__object">
            <video class="media-slider__video" data-video-id="5579506689001" data-video-name="Michael Kraus on the Misperception of Racial Economic Equality - Data" data-title="Economic Inequality" poster="/yalesom/assets/patterns/Kraus_titleslide.jpg" src="http://f1.media.brightcove.com/4/1822790495001/1822790495001_5579531340001_5579506689001.mp4?pubId=1822790495001&amp;videoId=5579506689001" autoplay="true"></video>
            <img class="media-slider__video_poster media-slider__video_poster--playing" src="/yalesom/assets/patterns/Kraus_titleslide.jpg">
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
```hint
Video slides are intended to be teasers for other content and **not primary content**. Maximum video length should be around 15 seconds.
```
## Image
When video content is not available, or is otherwise inappropriate, still images are permissible. Apply random transition effects to images to emulate the effect of video content.
```html|plain,light
<div id="media-slider-2396" class="media-slider media-slider--slideshow sliderLoaded" aria-labelledby="media-slider-2396_title">
  <ul class="media-slider__media-list">
    <li id="media-slot-158828" class="media-slider__media-slot media-slider__media-slot--active" data-type="image" aria-hidden="true">
      <div class="media-slider__media">
        <div class="media-slider__media-wrapper" data-href="https://som.yale.edu/mission-objectives/interests-industries/finance" data-title="" data-ischrome="true">
          <h2 class="media-slider__title">Interests and Industries: Finance</h2>
          <div class="media-slider__object">
          <figure class="media-slider__figure"><img src="/yalesom/assets/patterns/_DSC0185.jpg" class="media-slider__image media-slider__kb-pan-right"></figure>
          </div>
        </div>
        <div class="media-slider__meta-data">
          <span class="media-slider__meta-data__caption">Today’s leaders rely on a deep understanding of financial tools to solve complex problems in an increasingly global context.
        </span>
        </div>
      </div>
    </li>
  </ul>
</div>
```
# Grid
Media sliders should have a navigational component that allows users to select specific slides and to pause the animation. Because the visual elements in media slides are a mix of video and photographic content, the "pause" in this case is an overview grid of all the items in the slider. Users should be able to toggle back to the slide view.
```hint|warning
Navigation in carousel/slider elements are **critical for web accessibility requirements**.
```
```html|plain,light
<div id="media-slider-2396" class="media-slider sliderLoaded media-slider--grid" aria-labelledby="media-slider-2396_title" data-pid="2396">
  <div class="media-slider__toggle icon-linearicon icon--focus"></div>
  <ul class="media-slider__media-list">
    <li id="media-slot-158828" class="media-slider__media-slot media-slider__media-slot--animate-in-complete" data-type="image" aria-hidden="true">
      <div class="media-slider__media">
        <div class="media-slider__media-wrapper" data-href="https://som.yale.edu/mission-objectives/interests-industries/finance" data-title="" data-ischrome="true">
          <h2 class="media-slider__title">Interests and Industries: Finance</h2>
          <div class="media-slider__object">
            <figure class="media-slider__figure"><img src="/yalesom/assets/patterns/_DSC0185.jpg" class="media-slider__image"></figure>
          </div>
        </div>
        <div class="media-slider__meta-data">
          <span class="media-slider__meta-data__caption">Today’s leaders rely on a deep understanding of financial tools to solve complex problems in an increasingly global context.</span>
        </div>
      </div>
    </li>
    <li id="media-slot-140797" class="media-slider__media-slot media-slider__media-slot--animate-in-complete" data-type="video" aria-hidden="true">
      <div class="media-slider__media">
        <div class="media-slider__media-wrapper" data-href="https://som.yale.edu/news/2018/01/yale-som-entrepreneurs-arix-technologies" data-title="" data-ischrome="true">
          <h2 class="media-slider__title">Yale SOM Entrepreneurs: Dianna Liu ’18</h2>
          <div class="media-slider__object">
            <video class="media-slider__video" data-video-id="5749758390001" data-video-name="ARIX_Dianna Liu_Homepage_REV2" data-title="Yale SOM Entrepreneurs: Dianna Liu ’18" poster="/yalesom/assets/patterns/dianna_liu.jpg" src="http://f1.media.brightcove.com/4/1822790495001/1822790495001_5756355879001_5749758390001.mp4?pubId=1822790495001&amp;videoId=5749758390001"></video>
            <img class="media-slider__video_poster" src="/yalesom/assets/patterns/dianna_liu.jpg">
            </div>
        </div>
        <div class="media-slider__meta-data">
          <span class="media-slider__meta-data__caption">Dianna Liu ’18, an oil and gas engineer before coming to Yale SOM, launched Arix Technologies, which is creating pipe crawling robots that can detect corrosion on pipelines, potentially saving millions in broken pipes and spills for the energy industry alone.</span>
        </div>
      </div>
    </li>
    <li id="media-slot-131529" class="media-slider__media-slot media-slider__media-slot--animate-in-complete" data-type="video" aria-hidden="false">
      <div class="media-slider__media">
        <div class="media-slider__media-wrapper" data-href="http://insights.som.yale.edu/insights/how-fair-is-american-society" data-title="" data-ischrome="true">
          <h2 class="media-slider__title">Economic Inequality</h2>
          <div class="media-slider__object">
            <video class="media-slider__video" data-video-id="5579506689001" data-video-name="Michael Kraus on the Misperception of Racial Economic Equality - Data" data-title="Economic Inequality" poster="/yalesom/assets/patterns/Kraus_titleslide.jpg" src="http://f1.media.brightcove.com/4/1822790495001/1822790495001_5579531340001_5579506689001.mp4?pubId=1822790495001&amp;videoId=5579506689001"></video>
            <img class="media-slider__video_poster media-slider__video_poster--playing" src="/yalesom/assets/patterns/Kraus_titleslide.jpg">
            </div>
        </div>
        <div class="media-slider__meta-data">
          <span class="media-slider__meta-data__caption">Americans tend to be overly optimistic about economic equality between white and black citizens, according to a new study by Yale researchers.</span>
        </div>
      </div>
    </li>
    <li id="media-slot-106025" class="media-slider__media-slot media-slider__media-slot--animate-in-complete" data-type="video" aria-hidden="true">
      <div class="media-slider__media">
        <div class="media-slider__media-wrapper" data-href="https://som.yale.edu/news/2016/07/inside-global-virtual-teams-course" data-title="" data-ischrome="true">
          <h2 class="media-slider__title">Why Global Virtual Teams?</h2>
          <div class="media-slider__object">
            <video class="media-slider__video" data-video-id="4968493136001" data-video-name="GVT Homepage Slider" data-title="Why Global Virtual Teams?" poster="http://f1.media.brightcove.com/8/1822790495001/1822790495001_4968781374001_4968493136001-vs.jpg?pubId=1822790495001&amp;videoId=4968493136001" src="http://f1.media.brightcove.com/4/1822790495001/1822790495001_4973329115001_4968493136001.mp4?pubId=1822790495001&amp;videoId=4968493136001"></video>
            <img class="media-slider__video_poster media-slider__video_poster--playing" src="http://f1.media.brightcove.com/8/1822790495001/1822790495001_4968781374001_4968493136001-vs.jpg?pubId=1822790495001&amp;videoId=4968493136001">
          </div>
        </div>
        <div class="media-slider__meta-data">
          <span class="media-slider__meta-data__caption">The Global Virtual Teams course helps students develop the tools they need to successfully work across cultural and geographic barriers.</span>
        </div>
      </div>
    </li>
  </ul>
</div>
```

[cards]: /patterns/cards
