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

### Screws and washers

<table>
    <thead>
        <tr>
            <th>Description</th>
            <th>Min. Quantity</th>
            <th>Unit Price Estimate</th>
            <th>Comment</th>
            <th>URL</th>
            <th>Full Name</th>
            <th>Used For</th>
        </tr>
    </thead>
    <tbody>
        {% for item in site.data.parts_list_screws %}
        <tr>
            <td>{{ item.Description }}</td>
            <td>{{ item["Min. quantity"] }}</td>
            <td>${{ item["Unit price estimate ($)"] | default: "N/A" }}</td>
            <td>{{ item.Comment }}</td>
            <td>
                {% if item.URL %}
                    <a href="{{ item.URL }}" target="_blank">{{ item.URL }}</a>
                {% else %}
                    N/A
                {% endif %}
            </td>
            <td>{{ item["Full name"] | default: "N/A" }}</td>
            <td>{{ item["Used for"] | newline_to_br }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>

Might be easier to just get the screw kits:

<table>
    <thead>
        <tr>
            <th>Description</th>
            <th>Quantity</th>
            <th>Unit Price Estimate</th>
            <th>Comment</th>
            <th>URL</th>
            <th>Full Name</th>
        </tr>
    </thead>
    <tbody>
        {% for item in site.data.parts_list_screw_kits %}
        <tr>
            <td>{{ item.Description }}</td>
            <td>{{ item.Quantity }}</td>
            <td>${{ item["Unit price estimate ($)"] | default: "N/A" }}</td>
            <td>{{ item.Comment }}</td>
            <td>
                {% if item.URL %}
                    <a href="{{ item.URL }}" target="_blank">{{ item.URL }}</a>
                {% else %}
                    N/A
                {% endif %}
            </td>
            <td>{{ item["Full name"] | default: "N/A" }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>

### Tools

<table>
    <thead>
        <tr>
            <th>Name</th>
            <th>Unit Price Estimate</th>
            <th>Comment</th>
            <th>URL</th>
            <th>Full Name</th>
            <th>Used For</th>
        </tr>
    </thead>
    <tbody>
        {% for item in site.data.parts_list_tools %}
        <tr>
            <td>{{ item.Name }}</td>
            <td>${{ item["Unit price estimate ($)"] | default: "N/A" }}</td>
            <td>{{ item.Comment | default: "N/A" }}</td>
            <td>
                {% if item.URL %}
                    <a href="{{ item.URL }}" target="_blank">{{ item.URL }}</a>
                {% else %}
                    N/A
                {% endif %}
            </td>
            <td>{{ item["Full name"] | default: "N/A" }}</td>
            <td>{{ item["Used for"] | newline_to_br }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>


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
            <th>Comment</th>
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
            <th>Comment</th>
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