---
layout: default
title: Edit a URL
parent: API
nav_order: 2
---

# Edit a URL

`POST` https://noice.link/api/url\
Edits a short URL\
Required parameters:

- `slug` (string): The link's slug
- `url` (string): The unshortified URL
- `token` (string): The link token

Optional parameters:

- `title` (string): The preview's title
- `description` (string): The preview's description
- `image` (string): The preview's image
- `domain` (string): Custom domain name ([more info here](/custom-domains))

Example payload:

<!-- prettier-ignore -->
{% highlight JS %}
{
    description: "poggers",
    image: "https://d33wubrfki0l68.cloudfront.net/f9876141461caf644453abcc5918309b95b135f7/ace2a/assets/classic.png"
    slug: "free-nitro",
    title: "Yes free nitro",
    domain: "go.macedon.ga",
    url: "https://www.youtube.com/watch?v=dQw4w9WgXcQ",
    token: "eyASNOnjds..."
}
{% endhighlight %}

Example response:

<!-- prettier-ignore -->
{% highlight JS %}
{
    success: true
}

{% endhighlight %}

Possible error codes:\
[Here](https://docs.noice.link/errors)
