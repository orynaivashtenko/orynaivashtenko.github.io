---
layout: page
permalink: /publications/
title: Publications
description:
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->

<p class="pub-external">
  Full list on <a href="https://scixplorer.org/search?q=author%3A%22Ivashtenko%2C%20O%22&sort=date%20desc">SciX</a>
  and <a href="https://orcid.org/0000-0002-2805-9405">ORCID</a>.
</p>

<div class="publications">

<h2 class="pub-group">First-author</h2>

{% bibliography --group_by none --query @*[role=first]* %}

<h2 class="pub-group">Contributed</h2>

{% bibliography --group_by none --query @*[role=contributed]* %}

</div>
