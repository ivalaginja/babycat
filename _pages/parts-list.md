---
title: Parts List
layout: single
classes: wide
permalink: /parts-list/
sidebar:
  nav: "parts"
---

This page lists all the parts required to build the portable coronagraph. The list is divided into several categories
listed in the navigation bar on the left.

To build a fully functional coronagraph bench, you will need all components from the two sections
[Optical Components](#optical-components) and [Screws and tools](#screws-and-tools). Note how for the screws, you could
assemble them individually, but screw kits are also listed as a more convenient option. This does not include any devices
that can actually connect to the cameras and display their images. Since many teams are able to use some laptops they
already have, we just include the [Laptops](#laptops) section as a reminder.

The [Frame box](#frame-box) and [Transportation case](#transportation-case) sections are optional. The former lists the
parts required to build a solid frame with acrylic sheets for protection, the latter lists solid transportation case
that allows you to take your baby coronagraph on adventures.

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

The below table lists the screws and washers necessary for the full optical setup, exclusive all the screws that are
already included in some of the parts in [Optical Components](#optical-components), like for example the 8-32 set screws
that come with the 1/2" posts.

However, it is not unlikely that you either have enough of these standard screws already lying around or that you can
scavange them from colleagues or your lab. If not, we also list the respective screw kits you could buy, below.

Adapter screws for the magnetic mounts are not included in any of the listed screw kits. You will need to acquire these
separately.

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

If you prefer to get the full screw kits (remember that they do not include the adapter screws for the magnetic mounts):

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

The tools listed below are required for the assembly of the coronagraph. You might already have some of these tools, so
this list is just provided for convenience.

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

The frame box is an optional protection around the assembled coronagraph. It is made of aluminum frames and acrylic
sheets that can be assembled and disassembled. The frame box is designed to protect the coronagraph during transport and
also during outreach and teaching activities.

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

This case is large enough to fit the coronagraph including the frame, spare parts and laptops. The foam is pre-scored
into small cubes, so you could make the indentations in the foam whatever sizes they needed to be.

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