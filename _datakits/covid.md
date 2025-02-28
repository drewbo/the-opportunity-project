---
title: COVID-19
permalink: /data/covid-19/
class: datakit

sprint-name: ASA Data Challenge Expo
problem-statement-name: 'Helping Families, Businesses, and Communities Respond to COVID-19'
date: 2021-03-01

lead: Datasets selected as part of the The American Statistical Association Annual Data Challenge Expo

image: /assets/img/data-kits/covid.jpg
image-alt: 'Sticky notes on a window with the words &quot;Sorry - Closed. COVID-19&quot;'

data-experts:
  - category: General Census Data Questions
    contacts: 
      - name: Eric Coyle
        email: eric.a.coyle@census.gov
      - name: Tyson Weister & Kanin Reese
        email: cedsci.feedback@census.gov
  
  - category: Census Data Skills Questions
    contacts:
      - name: Alexandra Barkeremail
        email: alexandra.s.barker@census.gov
  
  - category: Census API Questions
    contacts:
      - name: Logan Powell
        email: logan.t.powell@census.gov
  
  - category: Census Data Visualization Questions
    contacts:
      - name: Gerson Vasquez
        email: gerson.d.vasquez@census.gov
---

### Below are additional points of contact for Census data in the following topics:

{% for group in page.data-experts %}
  <p class="margin-bottom-0 text-bold">{{ group.category }}:</p>
  <ul class="margin-top-0 usa-list--unstyled padding-left-4">
    {% for contact in group.contacts %}
      <li>
        {{contact.name}},
        <a class="usa-link" href="mailto:{{contact.email}}">{{contact.email}}</a>
      </li>
    {% endfor %}
  </ul>
{% endfor %}

