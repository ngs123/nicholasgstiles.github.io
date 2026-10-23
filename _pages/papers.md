---
layout: page
title: papers
permalink: /papers/
nav: true
nav_order: 1
---

<style>
  .papers-list ol.bibliography {
    list-style: none;
    padding: 0;
  }

  .papers-list h2.bibliography {
    display: block;
    color: var(--global-text-color, inherit);
    font-size: 1.5rem;
    border-top: 1px solid var(--global-divider-color, currentColor);
    border-bottom: 1px solid var(--global-divider-color, currentColor);
    margin-top: 2rem;
    margin-bottom: 1.25rem;
    padding: 0.75rem 0;
    text-align: right;
  }

  .papers-list ol.bibliography > li {
    margin-bottom: 2rem;
  }

  .papers-list .title {
    font-weight: 700;
    line-height: 1.4;
    margin-bottom: 0.35rem;
  }

  .papers-list .author a {
    border-bottom: 1px dashed currentColor;
    text-decoration: none;
  }

  .papers-list .author a:hover {
    border-bottom-style: solid;
  }

  .papers-list .periodical + .periodical {
    color: var(--global-text-color-light, #707070);
    font-size: 0.9rem;
    line-height: 1.6;
    margin: 0.5rem 0;
  }

  .papers-list .links a.btn {
    display: inline-block;
    color: var(--global-text-color, inherit);
    background: transparent;
    border: 1px solid currentColor;
    border-radius: 0.2rem;
    padding: 0.25rem 1rem;
    margin: 0.25rem 0.4rem 0.25rem 0;
    font-size: 0.875rem;
    text-decoration: none;
    box-shadow: none;
  }

  .papers-list .links a.btn:hover,
  .papers-list .links a.btn:focus-visible {
    color: var(--global-theme-color, currentColor);
  }
</style>

<div class="publications papers-list">
  {% bibliography --group_by year --group_order descending %}
</div>
