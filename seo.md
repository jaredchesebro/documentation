# SEO Features and Requirements
This document outlines all SEO requirements for websites developed by and for Lone Fir Creative.

## Table Of Contents
1. [For Browsers](#for-browsers)
2. [Favicon](#favicon)
3. [For Search Engines](#for-search-engines)
4. [For Social Media](#for-social-media)
5. [Images](#images)
6. [Headings](#headings)

## Meta Tags
### For Browsers
```
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
```

### Favicon
Favicons have many uses across browsers and devices. It is reccomended to have about 5 different favicons to optimize display for all devices.

```
<link rel="apple-touch-icon" sizes="180x180" href="/assets/images/apple-touch-icon.png">
<link rel="icon" type="image/png" sizes="32x32" href="/assets/images/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/assets/images/favicon-16x16.png">
<link rel="manifest" href="/assets/site.webmanifest">
```

### For Search Engines
```
<title>Page Title | Site Name</title>
<meta name="description" content="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.">
<meta name="author" content="Jeff Goldblum" />
<link rel="canonical" href="https://example.com/" />
<meta name="robots" content="INDEX, FOLLOW" />
```

### For Social Media
These tags are primarily to help with the display of content within social media platforms. This includes services like facebook, twitter, linkedIn, and even slack. While there are many types of tags available I would reccomend having the Open Graph tags at a minimum as many websites use or will fallback to those.

**Note:** Images should be either 1200px x 1200px or 630px by 1200px. 1200px by 1200px images will automatically cropped depending on the context they are being used.

#### Open Graph
```
<!-- Open Graph -->
<meta property="og:title" content="Page Title | Site Name" />
<meta property="og:description" content="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua." />
<meta property="og:type" content="website" />
<meta property="og:url" content="https://example.com/" />
<meta property="og:image" content="https://example.com/uploads/images/meta-img.jpg" />
```

#### Twitter Card
```
<!-- Twitter Card -->
<meta property="twitter:card" content="summary_large_image" />
<meta property="twitter:title" content="Page Title | Site Name" />
<meta property="twitter:domain" content="example.com">
<meta property="twitter:url" content="https://example.com/">
<meta property="twitter:description" content="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua." />
<meta property="twitter:image" content="https://example.com/uploads/images/meta-img.jpg" />
```

## Images
### Decorative Images
An image used for decorative purposes only should have a blank alt attribute.

```
<img src="/uploads/images/example.jpg" alt="">
```

### Contextual Images
Images that help illustrate a concept related to page content should have the alt text attribute filled out. Try to describe the image so a user may understand how it fits into the context of the page content; be concise.
```
<img src="/uploads/images/example.jpg" alt="Describe the image">
```

## Headings
Headings must appear in hierarchal order. Typically a page will only have one `<h1>` tag.

```
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

You cannot skip from an `<h1>` to an `<h3>` for design concerns; You must use css to style the specific instance. In the example we use a css utility class to style the `<h2>` tag to look like an `<h3>`. This a common pattern for the css frameworks we use.

```
<h1>Heading 1</h1>
<h2 class="h3">Heading 2</h2>
```
