# Hello!

{% comment %} Keep Pinto's age up to date :) {% endcomment %}

{% assign dateStart = "April 26, 2020" | date: "%s" %}
{% assign dateNow = "now" | date: "%s" %}
{% assign diffSeconds = dateNow | minus: dateStart %}
{% assign diffDays = diffSeconds | divided_by: 3600 | divided_by: 24 %}
{% assign diffMonths = diffDays | divided_by: 30.417 | round %}

My name is Phil - thanks for checking out my personal site!

This site is still being put together but it's underway with some general information [about me](about "Go to About Me!") and some of the [projects](projects "Go to Projects!") I've worked on or am currently working on :)

Below is a picture of my dog, Pinto!

She is {{ diffMonths }} months old and loves exploring the world, her frisbee, and wiggling!

<img src="{{ '/public/images/pinto.jpg' | relative_url }}" alt="Pinto!">
