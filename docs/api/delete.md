---
layout: default
title: Delete a URL
parent: API
nav_order: 3
---

# Delete a URL

`DELETE` https://noice.link/api/url\
Deletes a short URL\
Required headers:

- `Authorization` (string): The link token

Example response:

<!-- prettier-ignore -->
{% highlight JS %}
{
    success: true
}

{% endhighlight %}

Possible error codes:\
[Here](https://docs.noice.link/errors)
