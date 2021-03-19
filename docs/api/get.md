---
layout: default
title: Get URL info
parent: API
nav_order: 3
---

# Get URL info

`GET` https://noice.link/api/url\
Gets a short URL info\

There are 2 ways to use this endpoint:

- By using the link token;
- By using the "slug" query.

### Link token

#### Required header

- `Authorization` (string): The link token

#### cURL request example

{% highlight sh %}
curl --request GET \
 --url https://noice.link/api/url \
 --header 'Authorization: YOUR_LINK_TOKEN' \
{% endhighlight %}

### Slug query

#### Required query parameter

- `slug` (string): The link's slug

#### cURL request example

{% highlight sh %}
curl --request GET \
 --url https://noice.link/api/url?slug=your_slug \
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

### Possible error codes:

[Here](https://docs.noice.link/errors)
