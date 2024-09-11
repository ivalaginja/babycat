---
title: Parts List
layout: splash
permalink: /parts-list/
sidebar:
  nav: "parts"
---

## Optical Components

<table>
    <thead>
        <tr>
            <th>Description</th>
            <th>Quantity</th>
            <th>Price Estimate</th>
            <th>Source</th>
            <th>Vendor</th>
            <th>Component Name</th>
            <th>Assembly Location</th>
            <th>Notes</th>
        </tr>
    </thead>
    <tbody>
        {% for part in site.data.parts_list %}
        <tr>
            <td>{{ part.Description }}</td>
            <td>{{ part.Quantity }}</td>
            <td>${{ part["Unit price estimate ($)"] }}</td>
            <td><a href="{{ part.Source }}" target="_blank">{{ part.Source }}</a></td>
            <td>{{ part.Vendor }}</td>
            <td>{{ part.Name }}</td>
            <td>{{ part["Assembly location"] }}</td>
            <td>{{ part.Notes }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>

## Screws and tools

## Frame box

## Transportation case

