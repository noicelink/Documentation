---
layout: default
title: Register a URL
parent: API
nav_order: 1
---

# Register a URL

`POST` https://noice.link/api/url\
Creates a new short URL\

### Required payload parameters:

- `url` (string): The unshortified URL

### Optional payload parameters:

- `slug` (string): A custom slug
- `title` (string): The preview's title
- `description` (string): The preview's description
- `image` (string): The preview's image
- `color` (string): The embed color in HEX format (e.g.: "#ff00ff")

### Example payload:

<!-- prettier-ignore -->
{% highlight JS %}
{
    description: "poggers",
    image: "https://cdn.macedon.ga/image.png"
    slug: "free-nitro",
    title: "Yes free nitro",
    url: "https://www.youtube.com/watch?v=dQw4w9WgXcQ",
    color: "#ffffff"
}
{% endhighlight %}

### cURL request example

<!-- prettier-ignore -->
{% highlight %}
curl --request POST \
 --url https://noice.link/api/url \
 --header 'Authorization: YOUR_LINK_TOKEN' \
 --header 'Content-Type: application/json'
 --data '{"url": "https://macedon.ga"}'
{% endhighlight %}

### Example response:

<!-- prettier-ignore -->
{% highlight JS %}
{
    description: "poggers",
    image: "https://cdn.macedon.ga/image.png",
    slug: "qixof",
    title: "Yes free nitro",
    url: "https://www.youtube.com/watch?v=dQw4w9WgXcQ",
    token: "eyASNOnjds...",
    color: "#ffffff"
}
{% endhighlight %}

### Possible error codes:\

[Here](https://docs.noice.link/errors)
