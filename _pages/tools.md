---
title: Tools
layout: collection
permalink: /tools/
collection: tools
entries_layout: list
classes: wide
---

A collections of **Tools** goes here...

{% assign tool_files = site.static_files | where: "tool", true %}
{% for mytool in tool_files %}
  {{ mytool.path }}
{% endfor %}

| Tool |   		|
| :--- | :--- |
| **Password Generator** | [PWD](/_tools/PWD.html) |
| **Password Generator (27)** | [PWD](/_tools/PWD27.html) |