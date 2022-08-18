# Useful GitHub Flavored Markdown

## Enhanced Blockquotes

> **Note** this repository does not contain `GitHub Flavored Markdown`.

```md
> **Note** BLOCKQUOTE_TEXT
```
> **Warning** this only works on GitHub, or services where this is supported.

```md
> **Warning** BLOCKQUOTE_TEXT
```

## Context-based images

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/25423296/163456776-7f95b81a-f1ed-45f7-b7ab-8fa810d529fa.png">
  <img alt="Shows an illustrated sun in light color mode and a moon with stars in dark color mode." src="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
</picture>

```md
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="IMAGE_URL">
  <img alt="IMAGE_ALT" src="IMAGE_URL">
</picture>
```
