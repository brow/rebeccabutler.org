---
layout: default
description: I design and build software. I led iOS development at Asana and cofounded Pod. I'm available for consulting sometimes.
---

<img 
  class="headshot"
  src="https://s.gravatar.com/avatar/857ce6f50d086b1232ccfcb9030ae4e2?s=360"
  alt="photo of Tom">

# Tom Brow

I design and build software for human use. For the last 10 years, I've focused on native iOS apps.

I'm sometimes available for [consulting](/consulting).

Previously I led iOS development at [Asana](https://asana.com), then cofounded [Pod](/pod).

Longer ago I worked at Google and Lytro, and consulted for startups funded by Y Combinator, Harrison Metal, and Accel Partners.

Longer ago yet I studied computer science at [Stanford](https://cs.stanford.edu/). My full CV is on [LinkedIn](https://www.linkedin.com/in/tombrow/).

## Contact

You can reach me anytime at [hello@tombrow.com](mailto:hello@tombrow.com).

[Subscribe to my newsletter](https://tinyletter.com/brow) to hear about new things I'm working on.

## Writing

{% for post in site.posts %}

* [{{post.title}}]({{post.url}}) ({{ post.date | date: '%B %Y' }})

{% endfor %}

