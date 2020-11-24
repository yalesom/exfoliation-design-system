> Teasers are abridged versions of content items containing the minimum viable information necessary to convey context.

# Articles and Events

Dated content are commonly displayed chronologically in a list.

## Full

Use where the display mode is the primary content of the page. For example, a blog overview page would have the posts in that blog as primary content. Author and timestamp are contained in the header with this pattern. Metadata are typically content tags.

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
    <figure class="node-teaser__image"><img src="/exfoliation-design-system/assets/core/image-300x300.gif" alt="Class of 2020"></figure>
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

```image|span-4
  src: "/exfoliation-design-system/assets/components/teasers-article-full.png"
  description: "Rendered example"
```

## Minimal

Use where the display mode is a supporting element on a page. For example, a landing page may contain a list of events or articles that are not the primary focus of the page. Author and timestamp are collected with the content source in the metadata area.

Selected sources include a "bug" icon to indicate content external to the current site.

```html|span-4
<article
	class="node node-teaser node-teaser--minimal node-type-insights_article"
>
	<h2 class="node-teaser__title">
		<a
			href="https://dev-insights-d8.pantheonsite.io/insights/the-art-world-in-the-age-of-covid"
			>The Art World in the Age of COVID</a
		>
	</h2>
	<footer class="metadata metadata--flat metadata--submitted">
		<span class="metadata__item metadata__timestamp timestamp"
			>October 15, 2020</span
		>
		<span
			class="metadata__item metadata__source metadata__source--insights_article"
			><a href="https://dev-insights-d8.pantheonsite.io">Yale Insights</a></span
		>
	</footer>
</article>
```

```hint|neutral,span-2
See [Node Teaser](https://bitbucket.org/sq360_sysadmin/yale-som-theme/src/master/scss/components/_node-teaser.scss)
```

```image|span-2
  src: "/exfoliation-design-system/assets/components/teasers-article-minimal.png"
  description: "Rendered example"
```

# Pages

Non-dated content use a more generic teaser structure, commonly featuring only a title, key image and excerpt.

## Large

```image|span-5
  src: "/exfoliation-design-system/assets/components/teasers-page-large.png"
  description: "Rendered example"
```

## Detail

Detail teasers are defined by their list of section links.

```image|span-3
  src: "/exfoliation-design-system/assets/components/teasers-page-detail.png"
  description: "Rendered example"
```

## Small

```image|span-3
  src: "/exfoliation-design-system/assets/components/teasers-page-small.png"
  description: "Rendered example"
```

# People

## Full

```image|span-4
  src: "/exfoliation-design-system/assets/components/teasers-person-full.png"
  description: "Rendered example"
```

## Minimal

```image|span-2
  src: "/exfoliation-design-system/assets/components/teasers-person-minimal.png"
  description: "Rendered example"
```

## Profiles

```image|span-2
  src: "/exfoliation-design-system/assets/components/teasers-person-profile.png"
  description: "Rendered example"
```
