+++
title = "720 Minutes"
weight = 1
+++

720 Minutes plays with time and generative stuff for profit.

{% set source = "content/work/720-minutes/720minutes.webp" %}
{% set small = resize_image(path=source, width=800, op="fit_width", format="webp", quality=85) %}
{% set medium = resize_image(path=source, width=1600, op="fit_width", format="webp", quality=85) %}

<figure>
  <img
    src="{{ medium.url }}"
    srcset="{{ small.url }} 800w,
            {{ medium.url }} 1600w,
            720minutes.webp 2400w"
    sizes="(min-width: 70rem) 67rem, calc(100vw - 3rem)"
    width="{{ medium.width }}"
    height="{{ medium.height }}"
    alt="One frame from 720 Minutes, with swirling and colourful patterns."
  >
</figure>
