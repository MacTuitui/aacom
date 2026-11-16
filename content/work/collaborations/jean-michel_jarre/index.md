+++
title = "EoN - Jean-Michel Jarre"
weight = 3

[extra]
medium = ["Physical", "Digital"]
tags = ["Music","Infinite", "Animation", "App"]
year = 2017
+++

A collaboration with the legend Jean-Michel Jarre to create visuals for the application [EoN](https://jeanmicheljarre.com/eon). Infinite music with infinite visuals, timed to the music, fitting the mood, and following along musical changes.

<div class="image-mosaic">
{% for asset in page.assets | sort %}
{% set filename = asset | split(pat="/") | last %}
{% if filename is matching(pat="^eon[0-9]{2}[.]png$") %}
{{ <art_image
  file={filename}
  alt={"EoN screenshot " ~ filename}
  sizes="(min-width: 43rem) 13rem, calc(50vw - 1.75rem)"
/> }}
{% endif %}
{% endfor %}
</div>


A special physical edition "Snapshots from EoN" was also released, with sampled generated snapshots, accompanied by two printed vinyl using outputs of the generative system André wrote, and an illustrated book showcasing the variety in the outputs.

{{<art_image
    file="snapshots.jpg"
    alt="Physical edition"
    caption="Physical edition of Snapshots from EoN"
/> }}
