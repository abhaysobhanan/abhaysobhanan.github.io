---
title: Beyond research
permalink: /beyond-research/
layout: prose
---

Away from work, I like to travel occasionally. The map shows the countries I have visited so far.

<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/jsvectormap@1.6.0/dist/jsvectormap.min.css">

<div id="travel-map"></div>

{% assign n_countries = site.data.travel.countries | size %}{% assign n_markers = site.data.travel.markers | size %}{% assign travel_total = n_countries | plus: n_markers %}
<p class="travel-count">{{ travel_total }} countries and territories:
{% assign sorted_countries = site.data.travel.countries | sort: "name" %}{% for c in sorted_countries %}{{ c.name }}{% unless forloop.last %}, {% endunless %}{% endfor %}{% if site.data.travel.markers %}{% assign sorted_markers = site.data.travel.markers | sort: "name" %}{% for m in sorted_markers %}, {{ m.name }}{% endfor %}{% endif %}.</p>

<style>
  #travel-map {
    width: 100%;
    height: clamp(260px, 50vw, 420px);
    margin: 1.5rem 0 1rem;
  }
  .travel-count { color: var(--graphite); font-size: 0.9375em; }
  .jvm-tooltip { font-family: inherit; font-size: 0.875rem; background: var(--ink); color: var(--paper); }
  .jvm-zoom-btn { background: var(--graphite); }
</style>

<script src="https://cdn.jsdelivr.net/npm/jsvectormap@1.6.0/dist/jsvectormap.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/jsvectormap@1.6.0/dist/maps/world.js"></script>
<script>
  document.addEventListener("DOMContentLoaded", function () {
    var el = document.getElementById("travel-map");
    if (typeof jsVectorMap === "undefined") {
      el.innerHTML = "<p>The map could not be loaded. Check your connection and reload the page.</p>";
      return;
    }
    var css = getComputedStyle(document.documentElement);
    var v = function (name) { return css.getPropertyValue(name).trim(); };
    new jsVectorMap({
      selector: "#travel-map",
      map: "world",
      backgroundColor: "transparent",
      zoomOnScroll: false,
      zoomButtons: true,
      regionsSelectable: false,
      selectedRegions: {{ site.data.travel.countries | map: 'code' | jsonify }},
      regionStyle: {
        initial:       { fill: v("--rule"), stroke: v("--paper"), strokeWidth: 0.4 },
        hover:         { fillOpacity: 0.8 },
        selected:      { fill: v("--accent") },
        selectedHover: { fill: v("--accent"), fillOpacity: 0.85 }
      },
      markersSelectable: false,
      markers: {% if site.data.travel.markers %}{{ site.data.travel.markers | jsonify }}{% else %}[]{% endif %},
      markerStyle: {
        initial: { fill: v("--accent"), stroke: v("--paper"), strokeWidth: 1.5, r: 5 }
      }
    });
  });
</script>
