---
title: Parts List
layout: single
permalink: /parts-list/
class: wide
---

<h1>Parts List</h1>

<table>
    <thead>
        <tr>
            <th>Component Name</th>
            <th>Description</th>
            <th>Image</th>
            <th>Quantity</th>
            <th>Source</th>
            <th>Price Estimate</th>
        </tr>
    </thead>
    <tbody>
        {% for part in site.data.parts-list %}
        <tr>
            <td>{{ part.name }}</td>
            <td>{{ part.description }}</td>
            <td><img src="{{ part.image }}" alt="{{ part.name }}"></td>
            <td>{{ part.quantity }}</td>
            <td><a href="{{ part.source }}" target="_blank">Buy here</a></td>
            <td>{{ part.price }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>

<p><a href="/assets/data/parts-list.csv" download>Download PDF version of the parts list</a></p>
