---
layout: default
title: "Discover Berkeley: A Student Guide"
---

# Discover Berkeley: A Student Guide

If you're new to Berkeley, this guide can help you find useful places and services around campus. Each entry includes information about the resource, how to access it, and where to find the latest official details.

<!-- Edit the heading and introduction above. The supplied loop below displays each row of the CSV. -->
{% for resource in site.data.locations %}

### {{ resource.name | escape }}

**Category:** {{ resource.category | escape }}  
**Area:** {{ resource.area | escape }}  
**Access note:** {{ resource.access_note | escape }}  
<a href="{{ resource.source_url | escape }}">Official source</a>

{% endfor %}

---

The entries come from this project's CSV. Confirm current details using the official links.
