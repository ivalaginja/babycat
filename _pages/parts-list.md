---
title: Parts List
layout: single
classes: wide
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
        {% for part in site.data.parts_list_optics %}
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

## Laptops

The portable coronagraph requires at least one laptop. The laptop should have two USB 3.0 ports and be able to run the
software required to control the cameras. If you want to be able to operate both cameras at the same time, you might
consider using two laptops.

## Frame box

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
        {% for part in site.data.parts_list_frame_box %}
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

## Transportation case

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
        {% for part in site.data.parts_list_case %}
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