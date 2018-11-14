> Teasers are abridged versions of content items containing the minimum viable information necessary to convey context.

# Articles and Events
Dated content are commonly displayed chronologically in a list.
## Full
Use where the display mode is the primary content of the page. For example, a blog overview page would have the posts in that blog as primary content. Author and timestamp are contained in the header with this pattern. Metadata are typically content tags.
```image|span-4
  src: "yalesom/assets/patterns/teasers-article-full.png"
  description: "Rendered example"
```
```html|plain,light
<article class="node-teaser" role="article">
  <header>
    <h2><a href="#">From the Assistant Dean for Admissions: Meet the MBA Class of 2020</a></h2>
      <span class="node-teaser__author">
  	    <a href="#">Bruce DelMonico</a>
      </span>
      <span class="timestamp">August 24, 2018</span>
  </header>
  <div class="node-teaser__main">
    <figure class="node-teaser__image"><img src="/yalesom/assets/core/image-300x300.gif" alt="Class of 2020"></figure>
    <div class="node-teaser__body">
      <p>The 347 new members of the Yale SOM community are as diverse and accomplished as any we have welcomed to New Haven.</p>

      <a href="#" class="node-teaser__continue">Continue reading “From the Assistant Dean for Admissions: Meet the MBA Class of 2020”</a>
    </div>
  </div>
  <footer class="node-teaser__metadata metadata metadata--flat">
    <span class="metadata__item"><a href="#" class="icon--tags--right">Admissions</a></span>
    <span class="metadata__item"><a href="#" class="icon--tags--right">Student Life</a></span>
  </footer>
</article>
```

## Minimal
Use where the display mode is a supporting element on a page. For example, a landing page may contain a list of events or articles that are not the primary focus of the page. Author and timestamp are collected with the content source in the metadata area.

Selected sources include a "bug" icon to indicate content external to the current site.

```image|span-2
  src: "yalesom/assets/patterns/teasers-article-minimal.png"
  description: "Rendered example"
```
```code|collapsed
<article class="node-teaser node-teaser--minimal" role="article">
  <header>
    <h2><a href="#">Can Organized Labor Come Back?</a></h2>
  </header>
  <footer class="node-teaser__metadata metadata metadata--flat">
    <span class="metadata__item metadata__item__date timestamp">August 28, 2018</span>
    <span class="metadata__item metadata__item__authors"><a href="#">Richard L. Trumka</a></span>
    <span class="metadata__item metadata__item__source icon--insights"><a href="http://insights.som.yale.edu" aria-label="Visit Yale Insights" target="blank">Yale Insights</a></span>
  </footer>
</article>
```
```hint|warning
**Important:** Class structures in sample markup not yet added to Main SOM theme. See [Node Teaser](https://bitbucket.org/sq360_sysadmin/yale-som-theme/src/master/scss/parts/_node-teaser.scss)
```

# Pages
Non-dated content use a more generic teaser structure, commonly featuring only a title, key image and excerpt.
## Large
```image|span-5
  src: "yalesom/assets/patterns/teasers-page-large.png"
  description: "Rendered example"
```
## Detail
Detail teasers are defined by their list of section links.
```image|span-3
  src: "yalesom/assets/patterns/teasers-page-detail.png"
  description: "Rendered example"
```
## Small
```image|span-3
  src: "yalesom/assets/patterns/teasers-page-small.png"
  description: "Rendered example"
```

# People
## Full
```image|span-4
  src: "yalesom/assets/patterns/teasers-person-full.png"
  description: "Rendered example"
```
## Minimal
```image|span-2
  src: "yalesom/assets/patterns/teasers-person-minimal.png"
  description: "Rendered example"
```
## Profiles
```image|span-2
  src: "yalesom/assets/patterns/teasers-person-profile.png"
  description: "Rendered example"
```
