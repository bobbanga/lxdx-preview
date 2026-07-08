# lxdx-preview

Public preview pages for Lixu Daixing article reviews.

This repository only stores non-sensitive static preview pages for Bob's review.
It is not the source of truth for article packages, WeChat drafts, or publication status.

## Review Entry

- https://bobbanga.github.io/lxdx-preview/wechat-005-freight-knowledge-base/

Top-level entry:

- https://bobbanga.github.io/lxdx-preview/

## Article Structure

Each article uses one fixed directory:

```text
<article_id>/
  index.html
  images/
    cover.png
```

`index.html` must reference the cover with the relative path:

```text
images/cover.png
```

## Copy Boundary

The WeChat-copyable body area is:

```text
#wechat-copy-content
```

Only content intended for the WeChat editor should be inside that element. Review helper text, buttons, internal status, and private workflow notes must stay outside it.

If a cover image should be copied into the WeChat editor body, the image must be inside `#wechat-copy-content` and still use `images/cover.png`.

## Cover Image Rule

Use the formal generated cover image at:

```text
<article_id>/images/cover.png
```

Do not commit screenshots, thumbnails, low-resolution placeholders, corrupted files, local absolute paths, GPT temporary attachment paths, Google Drive paths, or credential material.
