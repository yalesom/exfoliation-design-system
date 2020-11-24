> **Cards** visually articulate a single topic with a minimum of information. They should be simple, actionable and easy to scan.

# Anatomy

```image|plain,span-4
src: "/exfoliation-design-system/assets/components/card-anatomy.png"
```

## Elements

**Headline**
_(required)_ Header text is the only required element of a card. Headlines should scale to fill the available container space and be concise so as not to conflict with image content. Text always is contained inside the image region and is most commonly is aligned to the left and bottom of the container.

**Image**
_(preferred)_ All card types should, whenever possible, highlight a compelling image.

**Metadata**
_(optional)_ Metadata represents the critical details necessary to give context to an individual card. Commonly:

- _Date_ — when was the content published
- _Author_ — who authored to the content
- _Source_ — where was the content published

While each metadatum should be visually distinct, sizes and styles should remain consistent to the parent application.

**Description**
_(optional)_ Provides additional context to a card where the headline/image is insufficient. Descriptions should be brief (maximum of 4 lines). Desrciptions should not be used in conjuction with Metadata.

**Source logo**
_(optional)_ External sources may be called out by a small, branded identifier in the upper right of the card.

# Specimens

```html|span-4,plain,light
<ul class="ysm-slider__list" data-min-height="true">
<li class="ysm-slider__slot">
<article id="paragraph-19116" class="node-teaser card">
  <header class="card__object card--has-url card--insights_article" data-dynamic-font-size="true" style="--dynamic-font-size:486px">
    <h2 class="card__title">
      Study Finds Hospital Desegregation Didn’t Improve Mortality Rate for Black Infants    </h2>
    <div class="card__media">
            <a href="https://insights.som.yale.edu/insights/study-finds-hospital-desegregation-didnt-improve-mortality-rate-for-black-infants" class="no-icon" aria-label="Continue reading Study Finds Hospital Desegregation Didn’t Improve Mortality Rate for Black Infants">
                          <picture><source media="all and (min-width: 851px)" type="image/webp" srcset="https://insights.som.yale.edu/sites/default/files/styles/square_sm/public/2020-10/desegregation%20of%20hospitals%20infant%20mortality.webp?h=63566863&amp;itok=pzhsmQVr 1x,https://insights.som.yale.edu/sites/default/files/styles/square/public/2020-10/desegregation%20of%20hospitals%20infant%20mortality.webp?h=63566863&amp;itok=kKmxyVTh 2x"><source media="all and (min-width: 851px)" type="image/jpeg" srcset="https://insights.som.yale.edu/sites/default/files/styles/square_sm/public/2020-10/desegregation%20of%20hospitals%20infant%20mortality.jpg?h=63566863&amp;itok=pzhsmQVr 1x, https://insights.som.yale.edu/sites/default/files/styles/square/public/2020-10/desegregation%20of%20hospitals%20infant%20mortality.jpg?h=63566863&amp;itok=kKmxyVTh 2x"><source type="image/webp" srcset="https://insights.som.yale.edu/sites/default/files/styles/square_sm/public/2020-10/desegregation%20of%20hospitals%20infant%20mortality.webp?h=63566863&amp;itok=pzhsmQVr"><source type="image/jpeg" srcset="https://insights.som.yale.edu/sites/default/files/styles/square_sm/public/2020-10/desegregation%20of%20hospitals%20infant%20mortality.jpg?h=63566863&amp;itok=pzhsmQVr"><img src="https://insights.som.yale.edu/sites/default/files/styles/square_sm/public/2020-10/desegregation%20of%20hospitals%20infant%20mortality.jpg?h=63566863&amp;itok=pzhsmQVr" alt="A black and white photo of a Black woman holding a newborn baby in a hospital ed" class="card__image" aria-role="presentation"></picture>                      </a>
        </div>
  </header>
      <footer class="metadata metadata--flat metadata--submitted">
      <span class="metadata__item metadata__timestamp timestamp">October 26, 2020</span>                        <span class="metadata__item metadata__author"><a href="https://insights.som.yale.edu/researchers/kerwin-k-charles">Kerwin K. Charles</a></span>


      <span class="metadata__item metadata__source metadata__source--insights_article"><a href="https://insights.som.yale.edu">Yale Insights</a></span>    </footer>
    </article>
</li>
</ul>
```

```hint|neutral,span-2
**Content card**
Most cards will be content cards and link to another page. Images should darken and blur on interactions to improve headline legibility for the focused element.
```

```html|span-4,plain,light
<ul class="ysm-slider__list" data-min-height="true">
<li class="ysm-slider__slot">
<article id="paragraph-19115" class="card node-teaser">
  <header class="card__object card--has-url card--no-media card--individual_profile" data-dynamic-font-size="true" style="--dynamic-font-size:486px">
    <h2 class="card__title">
      Alumni Profile: Developing Skills to Support Educators    </h2>
    <div class="card__media">
            <a href="https://som.yale.edu/profile/morgan-hall-10" class="no-icon" aria-label="Continue reading Alumni Profile: Developing Skills to Support Educators"></a>
        </div>
  </header>
      <footer class="metadata metadata--flat metadata--submitted">
      <span class="metadata__item metadata__timestamp timestamp">August 26, 2020</span>              <span class="metadata__item metadata__author">Morgan Hall ’10</span>


      <span class="metadata__item metadata__source metadata__source--individual_profile"><a href="/community/community-profiles" aria-label="Search all community profiles">Community Profile</a></span>    </footer>
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
<ul class="ysm-slider__list" data-min-height="true">
<li class="ysm-slider__slot">
<article id="card-id-942198" class="card card--social">
<header class="card__object card--has-url card--social--instagram" data-dynamic-font-size="true" style="--dynamic-font-size:486px">
    <div class="card__media">
            <a style="background-image:url(/exfoliation-design-system/assets/components/33627109_216557572275428_1368073815376003072_n.jpg);" class="no-icon external" href="https://www.instagram.com/p/BjX1hkHFMZ-" target="_blank"></a>
        </div>
  </header>
  <footer class="metadata metadata--flat metadata--submitted">
  <span class="metadata__item metadata__timestamp timestamp">May 29, 2018</span>
   <span class="metadata__item metadata__author"><a href="https://www.instagram.com/yalesom" target="_blank">@yalesom</a></span>

   </footer>
</article>
</li>
</ul>
```

```hint|neutral,span-2
**Image-only social card**
Source provides slightly more context for this card type, so source metadata should be moved to the beginning of the stack. In addition, headlines are optional for this card type, especially when an visual is a self-contained context (i.e., Instagram).
```

```html|span-4,plain,light
<ul class="ysm-slider__list" data-min-height="true">
<li class="ysm-slider__slot">
<article id="paragraph-17750" class="card card--social">
  <header class="card__object  card--no-media card--social--twitter" data-dynamic-font-size="true" style="--dynamic-font-size:486px">
          <h2 class="card__title tweet-text">
        Meet the Master’s Degree in Global Business and Society Class of <a target="_blank" rel="nofollow" class="twitter-timeline-link" href="https://twitter.com//search?q=%23Yale2021">#Yale2021</a>. <a href="https://t.co/rqvd5iJbsy">https://t.co/rqvd5iJbsy</a>      </h2>
                  <div class="tweet-author-wrapper">
                <a href="https://twitter.com/YaleSOM" aria-label="Visit Yale SOM on Twitter" rel="nofollow" target="_blank" class="no-icon"><img data-icon="" src="//pbs.twimg.com/profile_images/877910548100329472/ENIm5pUS_normal.jpg" alt="" width="48" height="48"><noscript><img src="//pbs.twimg.com/profile_images/877910548100329472/ENIm5pUS_normal.jpg" width="48" height="48" alt="" /></noscript><span class="tweet-author">Yale SOM</span><span class="tweet-screenname">@YaleSOM</span></a></div>
              <div class="tweet-footer content-group content-group--grid-2up">
                <div class="tweet-time"><a href="http://twitter.com/YaleSOM/status/1308768694768721922" class="no-icon"><em class="placeholder">2 months 2 days</em> ago</a></div>
                <div class="tweet-actions">
                  <a href="https://twitter.com/intent/tweet?in_reply_to=1308768694768721922" class="tweet--reply no-icon"><span>Reply</span></a><a href="https://twitter.com/intent/retweet?tweet_id=1308768694768721922" class="tweet--repeat no-icon"><span>Retweet</span></a><a href="https://twitter.com/intent/favorite?tweet_id=1308768694768721922" class="tweet--star no-icon"><span>Favorite</span></a></div>
              </div>      </header>
      <footer class="metadata metadata--flat metadata--submitted">
      <span class="metadata__item metadata__timestamp timestamp">September 23, 2020</span>      <span class="metadata__item metadata__author"><a href="https://twitter.com/YaleSOM" target="_blank" class="no-icon">@YaleSOM</a></span>          </footer>
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
<article class="node-teaser card">
  <header class="card__object card--has-url card--<card-type>" data-dynamic-font-size="true" style="font-size: 301px;">
    <h2 class="card__title">Get connected</h2>
      <div class="card__media">
        <a href="#" class="no-icon" aria-label="Continue reading Get connected">
          <img class="card__image" aria-role="presentation"
            src="example.jpg" alt="Students around conference table"
            title="" />
        </a>
      </div>
  </header>
  <footer class="metadata metadata--flat metadata--submitted">
    <span class="metadata__item metadata__timestamp timestamp">February 25, 2019</span>
    <span class="metadata__item metadata__author">
      <a href="#">Ranji Nagaswami</a>
    </span>
    <span class="metadata__item metadata__source metadata__source--insights-article">
      <a href="#" target="_blank">Yale Insights</a>
    </span>
  </footer>
</article>
```

```code|lang-js,span-4
YaleSOM.dynamicFontSize = function () {
  $('[data-dynamic-font-size=true]').each(function () {
    $(this).attr(
          "style",
          "--dynamic-font-size:" + $(this).outerWidth() + "px"
        );
  });
};
```

```hint|neutral,span-2
**Dynamic font scaling**
In most contexts, card headlines should scale relative to the containing element. This can be accomplished with the provided JavaScript function, which will change the font-size methodology from breakpoints to a font size CSS variable.
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
