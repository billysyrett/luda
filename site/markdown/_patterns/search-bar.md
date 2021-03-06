---
title: Search Bar
description: Learn how to create a search bar and combine an option filter.
---

## Usage

To create a search bar, add the `.search-bar` class to a container,
then wrap a search filed and a button inside.

{% capture search_bar %}
<div class="search-bar">
  <div class="fm fm-text">
    <input type="search" placeholder="Search anything...">
  </div>
  <button class="btn btn-ico btn-primary">
    <i class="ico ico-search"></i>
  </button>
</div>
{% endcapture %}
<div class="example">
  {{ search_bar }}
</div>
``` html{{ search_bar }}```

## Option Filter

If you need an option filter in the search bar,
prepend a form dropdown or a select field
into the search bar container like the below example.

{% capture options %}
<div class="search-bar">
  <div class="fm-dropdown dropdown-absolute">
    <div class="fm fm-select"><input></div>
    <div class="dropdown-menu">
      <div class="dropdown-items">
        <div class="btns-y">
          <div class="btn-radio btn-hollow-primary">
            <input type="radio" checked name="search_option" value="one">
            <label>Videos</label>
          </div>
          <div class="btn-radio btn-hollow-primary">
            <input type="radio" name="search_option" value="two">
            <label>Pictures</label>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="fm fm-text">
    <input type="search" placeholder="Enter keywords">
  </div>
  <button class="btn btn-primary">Search</button>
</div>
{% endcapture %}
<div class="example">
  {{ options }}
</div>
``` html{{ options }}```