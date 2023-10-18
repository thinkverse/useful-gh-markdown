# Useful GitHub Flavored Markdown Snippets

## Enhanced Blockquotes

- [ ] Works on GitHub mobile app.

```md
> [!NOTE]
> BLOCKQUOTE_TEXT
```

> [!NOTE]
> This repository does not contain `GitHub Flavored Markdown`.

```md
> [!WARNING]
> BLOCKQUOTE_TEXT
```

> [!WARNING]
> This only works on GitHub, or services where this is supported.

#### 2023 Updates!

As of July 2023, we got a new `IMPORTANT` type and a new `![TYPE]` syntax. You can read more about it in the [discussion](https://github.com/orgs/community/discussions/16925).

```md
> [!IMPORTANT]
> BLOCKQUOTE_TEXT
```

> [!IMPORTANT]
> This became available on 21st July 2023.

The old syntax, `**type**` will be phased out in favor of the new syntax.

```md
> **Note**
> This is the old syntax.
```

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
