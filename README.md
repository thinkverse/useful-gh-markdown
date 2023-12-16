# Useful GitHub Flavored Markdown Snippets

## Alerts

> Previously knows as "*Enhanced Blockquotes*."

You can read about Alerts in the [documentation](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#alerts).

- [x] Works on GitHub mobile app.

```md
> [!NOTE]
> BLOCKQUOTE_TEXT
```

> [!NOTE]
> This repository contains `GitHub Flavored Markdown`.

```md
> [!WARNING]
> BLOCKQUOTE_TEXT
```

> [!WARNING]
> This only works on GitHub, or services where this is supported.

#### July 2023 Update!

As of July 2023, we got a new `IMPORTANT` type and a new `![TYPE]` syntax. You can read more about it in the [discussion](https://github.com/orgs/community/discussions/16925).

```md
> [!IMPORTANT]
> BLOCKQUOTE_TEXT
```

#### November 2023 Update!

As of November 2023, we have two more types: `TIP` and `CAUTION`.


```md
> [!TIP]
> BLOCKQUOTE_TEXT
```

> [!TIP]
> This became available on 14th November 2023.

```md
> [!CAUTION]
> BLOCKQUOTE_TEXT
```

> [!CAUTION]
> Might not be supported on other platforms.

## Context-based images

### HTML version

- [x] Works on GitHub mobile app.

Specify an image to display based on the preferred color scheme. Change your color scheme from light to dark or vice-versa to see the image change.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/3369400/139447912-e0f43f33-6d9f-45f8-be46-2df5bbc91289.png">
  <img alt="GitHub logomark." src="https://user-images.githubusercontent.com/3369400/139448065-39a229ba-4b06-434b-bc67-616e2ed80c8f.png">
</picture>

```md
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="IMAGE_URL">
  <img alt="IMAGE_ALT" src="IMAGE_URL">
</picture>
```

Source: [Specify theme context for images in Markdown GA](https://github.blog/changelog/2022-08-15-specify-theme-context-for-images-in-markdown-ga/)

### Markdown version

- [x] Works on GitHub mobile app.

GitHub also supports themed images in Markdown, by appending `#gh-dark-mode-only` or `#gh-light-mode-only` at the end of an image url.

![GitHub-Mark-Light](https://user-images.githubusercontent.com/3369400/139447912-e0f43f33-6d9f-45f8-be46-2df5bbc91289.png#gh-dark-mode-only)
![GitHub-Mark-Dark](https://user-images.githubusercontent.com/3369400/139448065-39a229ba-4b06-434b-bc67-616e2ed80c8f.png#gh-light-mode-only)

```md
![IMAGE_ALT](IMAGE_URL#gh-dark-mode-only)
![IMAGE_ALT](IMAGE_URL#gh-light-mode-only)
```

Source: [Specify theme context for images in Markdown](https://github.blog/changelog/2021-11-24-specify-theme-context-for-images-in-markdown/)


## Fence blocks for Math

- [ ] Works on GitHub mobile app.

You can specify a math-specific fence block with ` ```math `, it even supports LaTeX expressions, read more about it in the [documentation](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions). 

````md
```math
\sqrt{3}
```
````

```math
\sqrt{3}
```

Source: [Fenced block syntax for mathematical expressions](https://github.blog/changelog/2022-06-28-fenced-block-syntax-for-mathematical-expressions/)
