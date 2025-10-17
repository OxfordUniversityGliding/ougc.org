---
layout: sidebar_default
title: " "
tagline: " "
permalink: competitions/varsity_results/
cover: "/assets/images/competitions/esb_derig.jpeg"
sidebar_title: "competitions"
---

<title>Varsity Results - OUGC</title>

## Varsity Match
This year's varsity match was held at Gransden Lodge on 16 - 18th June 2025.

Day 1 (Raw scores):
Teddy: 141
Brooke: 137
Adam: 61
Sergey: 73

Day 2:
Teddy: 167
Brooke: 151
Adam: 188
Sergey: 106

## Historical Record

<table>
  <thead>
    <tr>
      <th>Year</th>
      <th>Airfield</th>
      <th>Result</th>
    </tr>
  </thead>
  <tbody>
    {% for row in site.data.varsity_results %}
      <tr>
        <td>{{ row.year }}</td>
        <td>{{ row.airfield }}</td>
        <td>
          {% if row.note %}
            <em>{{ row.note }}</em>
          {% else %}
            {% if row.winner == "Oxford" %}
              <strong>Oxford {{ row.oxford }}</strong> Cambridge {{ row.cambridge }}
            {% else %}
              Oxford {{ row.oxford }} <strong>Cambridge {{ row.cambridge }}</strong>
            {% endif %}
          {% endif %}
        </td>
      </tr>
    {% endfor %}
  </tbody>
</table>

See also the Cambridge [record](https://wiki.cugc.org.uk/wiki/Varsity#Results).