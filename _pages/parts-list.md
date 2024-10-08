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

{: .notice--warning}
Note that we give all measurements and link to components in **imperial units**. If you want to use metric units, you
will have to make sure to convert all measurements and find the respective components.

The [Frame box](#frame-box) and [Transportation case](#transportation-case) sections are optional. The former lists the
parts required to build a solid frame with acrylic sheets for protection, the latter lists a sturdy transportation case
that allows you to take your baby coronagraph on adventures.

## Optical Components

{: .notice--success}
The total price estimate for the optical components listed below is **$4,200**.  
Without the alignment tools and with the simpler aperture, this reduces to **$3,400**.

Note how the above price estimate includes the three alignment optics (labelled with "Alignment") which together cost
~$300 and can be omitted if you already own similar components.

It is further possible to reduce the cost by replacing the laser-cut aperture mask listed in the table below with a
2.5 mm [Thorlabs alignment tool](https://www.thorlabs.com/thorproduct.cfm?partnumber=AP2.5) that doubles as an aperture,
for $12. The quality of the aperture image will be lower, but it is easy to upgrade this at a later time.

<table>
    <thead>
        <tr>
            <th>Description</th>
            <th>Quantity</th>
            <th>Unit Price Estimate</th>
            <th>Source</th>
            <th>Vendor</th>
            <th>Component Name</th>
            <th>Used For</th>
            <th>Notes</th>
        </tr>
    </thead>
    <tbody>
        {% for item in site.data.parts_list_optics %}
        <tr>
            <td>{{ item.Description }}</td>
            <td>{{ item.Quantity }}</td>
            <td>${{ item["Unit price estimate ($)"] }}</td>
            <td><a href="{{ item.Source }}" target="_blank">{{ item.Source }}</a></td>
            <td>{{ item.Vendor }}</td>
            <td>{{ item["Component name"] }}</td>
            <td>{{ item["Assembly location"] }}</td>
            <td>{{ item.Notes }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>

## Screws and Tools

The below table lists the screws and washers necessary for the full optical setup, exclusive all the screws that are
already included in some of the parts in [Optical Components](#optical-components), like for example the 8-32 set screws
that come with the 1/2" posts.

However, it is not unlikely that you either have enough of these standard screws already lying around or that you can
scavange them from colleagues or your lab. If not, we also list the respective screw kits you could buy, below.

{: .notice--warning}
**Adapter screws** for the magnetic mounts are not included in any of the listed screw kits. You will still need to
acquire these separately.

### Screws and Washers

<table>
    <thead>
        <tr>
            <th>Description</th>
            <th>Min. Quantity</th>
            <th>Unit Price Estimate</th>
            <th>Source</th>
            <th>Vendor</th>
            <th>Component Name</th>
            <th>Used For</th>
            <th>Notes</th>
        </tr>
    </thead>
    <tbody>
        {% for item in site.data.parts_list_screws %}
        <tr>
            <td>{{ item.Description }}</td>
            <td>{{ item["Min. quantity"] }}</td>
            <td>
                {% if item["Unit price estimate ($)"] %}
                    ${{ item["Unit price estimate ($)"] }}
                {% endif %}
            </td>
            <td>
                {% if item.Source %}
                    <a href="{{ item.Source }}" target="_blank">{{ item.Source }}</a>
                {% endif %}
            </td>
            <td>{{ item.Vendor }}</td>
            <td>{{ item["Component name"] }}</td>
            <td>{{ item["Assembly location"] | newline_to_br }}</td>
            <td>{{ item.Notes }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>

If you prefer to get the full screw kits (remember that they do not include the adapter screws for the magnetic mounts):

<table>
    <thead>
        <tr>
            <th>Description</th>
            <th>Unit Price Estimate</th>
            <th>Source</th>
            <th>Vendor</th>
            <th>Component Name</th>
            <th>Notes</th>
        </tr>
    </thead>
    <tbody>
        {% for item in site.data.parts_list_screw_kits %}
        <tr>
            <td>{{ item.Description }}</td>
            <td>${{ item["Unit price estimate ($)"]}}</td>
            <td><a href="{{ item.Source }}" target="_blank">{{ item.Source }}</a></td>
            <td>{{ item.Vendor }}</td>
            <td>{{ item["Component name"] }}</td>
            <td>{{ item.Notes }}</td>
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
            <th>Description</th>
            <th>Unit Price Estimate</th>
            <th>Source</th>
            <th>Vendor</th>
            <th>Component Name</th>
            <th>Used For</th>
            <th>Notes</th>
        </tr>
    </thead>
    <tbody>
        {% for item in site.data.parts_list_tools %}
        <tr>
            <td>{{ item.Description }}</td>
            <td>${{ item["Unit price estimate ($)"]  }}</td>
            <td> <a href="{{ item.Source }}" target="_blank">{{ item.Source }}</a></td>
            <td>{{ item.Vendor }}</td>
            <td>{{ item["Component name"] }}</td>
            <td>{{ item["Assembly location"] | newline_to_br }}</td>
            <td>{{ item.Notes }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>


## Laptops

The portable coronagraph requires at least one laptop. The laptop should have two USB 3.0 ports and be able to run the
software required to control the cameras. If you want to be able to operate both cameras at the same time, you might
consider using two laptops.

## Frame Box

The frame box is an optional protection around the assembled coronagraph. It is made of aluminum frames and acrylic
sheets that can be assembled and disassembled. The frame box is designed to protect the coronagraph during transport and
also during outreach and teaching activities.

{: .notice--success}
The total price estimate for the frame box is **$490**.

The frame box is extremely useful if you intend to transport your demo coronagraph in any sort of transportation case.

<table>
    <thead>
        <tr>
            <th>Description</th>
            <th>Quantity</th>
            <th>Unit Price Estimate</th>
            <th>Source</th>
            <th>Vendor</th>
            <th>Component Name</th>
            <th>Notes</th>
        </tr>
    </thead>
    <tbody>
        {% for item in site.data.parts_list_frame_box %}
        <tr>
            <td>{{ item.Description }}</td>
            <td>{{ item.Quantity }}</td>
            <td>${{ item["Unit price estimate ($)"] }}</td>
            <td><a href="{{ item.Source }}" target="_blank">{{ item.Source }}</a></td>
            <td>{{ item.Vendor }}</td>
            <td>{{ item["Component name"] }}</td>
            <td>{{ item.Notes }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>

## Transportation Case

This case is large enough to fit the coronagraph including the frame, spare parts and laptops. The foam is pre-scored
into small cubes, so you can make the indentations in the foam whatever sizes they needed to be.

<table>
    <thead>
        <tr>
            <th>Description</th>
            <th>Price Estimate</th>
            <th>Source</th>
            <th>Vendor</th>
            <th>Component Name</th>
            <th>Notes</th>
        </tr>
    </thead>
    <tbody>
        {% for item in site.data.parts_list_case %}
        <tr>
            <td>{{ item.Description }}</td>
            <td>${{ item["Unit price estimate ($)"] }}</td>
            <td><a href="{{ item.Source }}" target="_blank">{{ item.Source }}</a></td>
            <td>{{ item.Vendor }}</td>
            <td>{{ item["Component name"] }}</td>
            <td>{{ item.Notes }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>