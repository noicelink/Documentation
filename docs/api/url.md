---
layout: default
title: Register a URL
parent: API
nav_order: 1
---

# Register a URL

`POST` https://noice.link/api/url\
Creates a new short URL\
Required parameters:

- `slug` (string): The link's slug
- `url` (string): The unshortified URL

Optional parameters:

- `title` (string): The preview's title
- `description` (string): The preview's description
- `image` (string): The preview's image

Example payload:

<!-- prettier-ignore -->
{% highlight JS %}
{
    description: "poggers",
    image: "https://d33wubrfki0l68.cloudfront.net/f9876141461caf644453abcc5918309b95b135f7/ace2a/assets/classic.png"
    slug: "free-nitro",
    title: "Yes free nitro",
    url: "https://www.youtube.com/watch?v=dQw4w9WgXcQ",
}
{% endhighlight %}

Example response:

<!-- prettier-ignore -->
{% highlight JS %}
{
    description: "poggers",
    image: "https://d33wubrfki0l68.cloudfront.net/f9876141461caf644453abcc5918309b95b135f7/ace2a/assets/classic.png",
    slug: "qixof",
    title: "Yes free nitro",
    url: "https://www.youtube.com/watch?v=dQw4w9WgXcQ",
    token: "eyASNOnjds...",
    \_id: "6052093f64e617001508c07a"
}
{% endhighlight %}

Possible error codes:\
[Here](https://docs.noice.link/errors)
