# Day 2: HTML Attributes, Links and Images

## Attributes

Attributes provide **additional information** about HTML elements.

```html
<a href="https://example.com">Example</a>
```

## Links

|Attribute|Purpose|
|---|---|
|`href`|Specifies the hyperlink destination|
|`target="_blank"`|Opens the link in a new tab/window|
|`rel="noopener noreferrer"`|Opener isolation and referrer privacy|

```html
<a href="https://example.com" target="_blank" rel="noopener noreferrer">Example</a>
```

## Absolute vs Relative URLs

|Type|Example|
|---|---|
|Absolute URL|`https://example.com/about.html`|
|Relative URL|`about.html`|

## Images

`<img>` embeds an image and is a **void element** (no closing tag, no content).

|Attribute|Purpose|
|---|---|
|`src`|Location of the image|
|`alt`|Text alternative|
|`width`|Width of the image|
|`height`|Height of the image|

```html
<img src="images/profile.jpg" alt="Profile photo" width="200" height="200">
```

## Relative Paths

|Path|Meaning|
|---|---|
|`images/profile.jpg`|Points into a subfolder|
|`./`|Current directory|
|`../`|Parent directory|

## Inline vs Block Elements

| Display                  | Elements             |
| ------------------------ | -------------------- |
| Inline (by default)      | `<a>`, `<img>`       |
| Block-level (by default) | Headings, paragraphs |
