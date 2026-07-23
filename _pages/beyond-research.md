---
layout: single
title: "Beyond Research"
permalink: /beyond-research/
author_profile: true
---

Away from work, I like to travel ocassionally. Here is a map highlighting the small list of countries I have been fortunate to explore so far.

<!-- Map library (loaded only on this page) -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/jsvectormap@1.6.0/dist/css/jsvectormap.min.css">

<div id="travel-map"></div>

{% assign n_countries = site.data.travel.countries | size %}{% assign n_markers = site.data.travel.markers | size %}{% assign travel_total = n_countries | plus: n_markers %}
<p class="travel-count">
  <strong>{{ travel_total }}</strong>
  countries &amp; territories visited
</p>

<div class="travel-chips">
{% assign sorted_countries = site.data.travel.countries | sort: "name" %}{% for c in sorted_countries %}<span class="travel-chip">{{ c.name }}</span>{% endfor %}{% if site.data.travel.markers %}{% assign sorted_markers = site.data.travel.markers | sort: "name" %}{% for m in sorted_markers %}<span class="travel-chip travel-chip--marker">{{ m.name }}</span>{% endfor %}{% endif %}
</div>

<style>
  #travel-map {
    width: 100%;
    max-width: 960px;
    height: clamp(300px, 58vw, 540px);
    margin: 1.2em auto 0.6em auto;
    background-color: #f7f9fb;
    border: 1px solid #e6e9ee;
    border-radius: 10px;
  }
  .travel-count {
    text-align: center;
    color: #555;
    font-size: 0.95em;
    margin: 0.2em 0 1em 0;
  }
  .travel-count strong { color: #007ACC; font-size: 1.15em; }
  .travel-chips {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    justify-content: center;
    max-width: 780px;
    margin: 0 auto 1em auto;
  }
  .travel-chip {
    display: inline-block;
    padding: 4px 12px;
    font-size: 0.85em;
    color: #005a99;
    background-color: #eaf4fb;
    border: 1px solid #cfe6f6;
    border-radius: 999px;
    white-space: nowrap;
  }
  .travel-chip--marker {
    color: #7a4d00;
    background-color: #fdf3e3;
    border-color: #f2ddb8;
  }
  /* jsVectorMap tooltip tweak */
  .jvm-tooltip {
    background-color: #007ACC;
    font-family: inherit;
    font-size: 0.85em;
  }
</style>

<script src="https://cdn.jsdelivr.net/npm/jsvectormap@1.6.0/dist/js/jsvectormap.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/jsvectormap@1.6.0/dist/maps/world.js"></script>
<script>
  document.addEventListener("DOMContentLoaded", function () {
    if (!window.jsVectorMap) return;
    new jsVectorMap({
      selector: "#travel-map",
      map: "world",
      backgroundColor: "transparent",
      zoomOnScroll: false,
      zoomButtons: true,
      regionsSelectable: false,
      selectedRegions: ["{{ site.data.travel.countries | map: 'code' | join: '", "' }}"],
      regionStyle: {
        initial:       { fill: "#e3e7ec", stroke: "#ffffff", strokeWidth: 0.4 },
        hover:         { fill: "#9eccec", fillOpacity: 1 },
        selected:      { fill: "#007ACC" },
        selectedHover: { fill: "#025c96" }
      },
      markersSelectable: false,
      markers: [
{%- for m in site.data.travel.markers -%}
        { name: {{ m.name | jsonify }}, coords: [{{ m.coords[0] }}, {{ m.coords[1] }}] }{% unless forloop.last %},{% endunless %}
{%- endfor -%}
      ],
      markerStyle: {
        initial: { fill: "#e8890c", stroke: "#ffffff", strokeWidth: 1.5, r: 5 },
        hover:   { fill: "#c56f00" }
      }
    });
  });
</script>
