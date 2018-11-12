# List panel

Find out more about the list panel component and when to use it in the [NHS Digital service manual](https://beta.nhs.uk/service-manual/patterns/).

To discuss or contribute to this component, visit the [GitHub issue for this component](https://github.com/nhsuk/nhsuk-frontend/issues/173).

## Quick start examples

### List panel

[Preview the list panel component](https://nhsuk.github.io/nhsuk-frontend/components/list-panel.html)

### HTML markup

```html
<div class="nhsuk-list-panel nhsuk-list-panel--mobile">
  <h2 id="A" class="nhsuk-list-panel__label">A</h2>
  <ul class="nhsuk-list-panel__list  nhsuk-list-panel__list--with-label ">
    <li class="nhsuk-list-panel__list-item">
      <a href="/index" class="nhsuk-list-panel__list-item-link">AAA</a>
    </li>
    <li class="nhsuk-list-panel__list-item">
      <a href="/index" class="nhsuk-list-panel__list-item-link">Abdominal aortic aneurysm</a>
    </li>
    <li class="nhsuk-list-panel__list-item">
      <a href="/index" class="nhsuk-list-panel__list-item-link">Abscess</a>
    </li>
  </ul>
  <div class="nhsuk-back-to-top">
    <a class="nhsuk-back-to-top__link" href="#nhsuk-a-z-nav">
      <svg class="nhsuk-icon nhsuk-icon__arrow-right" data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" aria-hidden="true">
        <path d="M19.6 11.66l-2.73-3A.51.51 0 0 0 16 9v2H5a1 1 0 0 0 0 2h11v2a.5.5 0 0 0 .32.46.39.39 0 0 0 .18 0 .52.52 0 0 0 .37-.16l2.73-3a.5.5 0 0 0 0-.64z"></path>
      </svg>
      Back to top
    </a>
  </div>
</div>

<div class="nhsuk-list-panel nhsuk-list-panel--mobile">
  <h2 id="B" class="nhsuk-list-panel__label">B</h2>
  <div class="nhsuk-list-panel__box  nhsuk-list-panel__box--with-label ">
    <p class="nhsuk-list-panel--results-items__no-results">There are currently no medicines listed</p>
  </div>
  <div class="nhsuk-back-to-top">
    <a class="nhsuk-back-to-top__link" href="#nhsuk-a-z-nav">
      <svg class="nhsuk-icon nhsuk-icon__arrow-right" data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" aria-hidden="true">
        <path d="M19.6 11.66l-2.73-3A.51.51 0 0 0 16 9v2H5a1 1 0 0 0 0 2h11v2a.5.5 0 0 0 .32.46.39.39 0 0 0 .18 0 .52.52 0 0 0 .37-.16l2.73-3a.5.5 0 0 0 0-.64z"></path>
      </svg>
      Back to top
    </a>
  </div>

</div>

<div class="nhsuk-list-panel nhsuk-list-panel--mobile">
  <h2 id="C" class="nhsuk-list-panel__label">C</h2>
  <ul class="nhsuk-list-panel__list  nhsuk-list-panel__list--with-label ">
    <li class="nhsuk-list-panel__list-item">
      <a href="/index" class="nhsuk-list-panel__list-item-link">Chest pain</a>
    </li>
    <li class="nhsuk-list-panel__list-item">
      <a href="/index" class="nhsuk-list-panel__list-item-link">Cold sore</a>
    </li>
  </ul>
  <div class="nhsuk-back-to-top">
    <a class="nhsuk-back-to-top__link" href="#nhsuk-a-z-nav">
      <svg class="nhsuk-icon nhsuk-icon__arrow-right" data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" aria-hidden="true">
        <path d="M19.6 11.66l-2.73-3A.51.51 0 0 0 16 9v2H5a1 1 0 0 0 0 2h11v2a.5.5 0 0 0 .32.46.39.39 0 0 0 .18 0 .52.52 0 0 0 .37-.16l2.73-3a.5.5 0 0 0 0-.64z"></path>
      </svg>
      Back to top
    </a>
  </div>
</div>

<div class="nhsuk-list-panel nhsuk-list-panel--mobile">
  <h2 id="D" class="nhsuk-list-panel__label">D</h2>
  <ul class="nhsuk-list-panel__list  nhsuk-list-panel__list--with-label ">
    <li class="nhsuk-list-panel__list-item">
      <a href="/index" class="nhsuk-list-panel__list-item-link">Dandruff</a>
    </li>
    <li class="nhsuk-list-panel__list-item">
      <a href="/index" class="nhsuk-list-panel__list-item-link">Dementia</a>
    </li>
    <li class="nhsuk-list-panel__list-item">
      <a href="/index" class="nhsuk-list-panel__list-item-link">Dental pain</a>
    </li>
  </ul>
  <div class="nhsuk-back-to-top">
    <a class="nhsuk-back-to-top__link" href="#nhsuk-a-z-nav">
      <svg class="nhsuk-icon nhsuk-icon__arrow-right" data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" aria-hidden="true">
        <path d="M19.6 11.66l-2.73-3A.51.51 0 0 0 16 9v2H5a1 1 0 0 0 0 2h11v2a.5.5 0 0 0 .32.46.39.39 0 0 0 .18 0 .52.52 0 0 0 .37-.16l2.73-3a.5.5 0 0 0 0-.64z"></path>
      </svg>
      Back to top
    </a>
  </div>
</div>
```

### Nunjucks macro

If you’re using Nunjucks macros in production be aware that using `html` arguments, or ones ending with `html` can be a [security risk](https://en.wikipedia.org/wiki/Cross-site_scripting). More about it in the [Nunjucks documentation](https://mozilla.github.io/nunjucks/api.html#user-defined-templates-warning).

```
{% from 'components/list-panel/macro.njk' import listPanel %}

{{ listPanel({
  label: "A",
  id: "A",
  items: [
    {
      URL: "/index",
      link: "AAA"
    },
    {
      URL: "/index",
      link: "Abdominal aortic aneurysm"
    },
    {
      URL: "/index",
      link: "Abscess"
    }
  ]
}) }}

{{ listPanel({
  label: "B",
  id: "B",
  disable: "true",
  message: "There are currently no medicines listed"
}) }}

{{ listPanel({
  label: "C",
  id: "C",
  items: [
    {
      URL: "/index",
      link: "Chest pain"
    },
    {
      URL: "/index",
      link: "Cold sore"
    }
  ]
}) }}

{{ listPanel({
  label: "D",
  id: "D",
  items: [
    {
      URL: "/index",
      link: "Dandruff"
    },
    {
      URL: "/index",
      link: "Dementia"
    },
    {
      URL: "/index",
      link: "Dental pain"
    }
  ]
}) }}
```