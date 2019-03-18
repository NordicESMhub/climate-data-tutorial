---
title: About
---
---
layout: default
title: About us
image: /images/about.jpg
---


## What are we doing?

**Vision/Mission statement:**

The aim of the Nordic Earth System Modeling Hub to build a Nordic ESM community within the 
Nordic countries (Denmark, Finland, Sweden, Iceland, Estonia, Norway) for sharing knowledge, 
codes (climate models, Galaxy climate data analysis and visualization tools), 
training tutorials so that our contributions to the Coupled Model 
Intercomparison Project can be easily exploited/reused within the Nordic countries and beyond, 
and by other communities.


### The problem

- Students, PhDs, postdocs, researchers often have to re-invent the wheel and waste lots of time to find out
where to find NorESM climate data, which model configurations are supported to run, how to visualize data 
over the Nordics i.e. which projection to use, etc. 
- The number of inhabitants in each Nordic country is little (12 millions in Sweden, about 6 millions in Finland 
and Norway but 300 000 inhabitants in Iceland) so it is often difficult to find specialists working on 
similar problems within your own University and country.


### The solution

* provide the Nordic ESM community with up to date information (i.e. documentation that can be easily updated by contributors)
* connect students, PhDs, postdocs and researchers by providing a knowledge map, listing skills and competences.
* make the Nordic contributions more visible and favor new collaborations.


## Who are we?

The founder of the NordicESMHub is [Anne][link_AnneFouilloux]. 

<div class="people">
  {% for entry in site.data['people'] %}
    {% assign username = entry[0] %}
    {% include people.html username=username %}
  {% endfor %}
</div>

## Our values

We have high ethical standards, including:

- **Education**: Help educate the public about science and biotechnology, their
  benefits and implications
- **Transparency**: Emphasize transparency and the sharing of ideas, knowledge, data,
  protocols and results.
- **Open science**: Promote open science and decentralized access to science.
- **Modesty** Know you don't know everything.
- **Community**: Carefully listen to any concerns and questions and respond honestly
- **Respect**: Respect humans and all living systems.
- **Responsibility**: Recognize the complexity and dynamics of living systems and our
  responsibility towards them.

## What do we need?

**You!** In whatever way you can help.

We need expertise in fundraising, science, education, communication, interaction
with the public. 

## Get involved

If you think you can help or are willing to contribute
then please check out [our contributors'
guidelines](/CONTRIBUTING) and
our [roadmap](roadmap).

Please note that it's very important to us that we maintain a positive and
supportive environment for everyone who wants to participate. When you join us
we ask that you follow our [code of conduct]({{ site.github.repository_url
}}/blob/master/CODE_OF_CONDUCT.md) in all interactions both on and offline.

### Want to join the Nordic Earth System Modeling Community?

You are very welcomed and invited to join the community and participate in the upcoming events. 
You can simply contact us at [{{ site.email|replace:'@','[at]' }}](mailto:{{ site.email }}) or chat with us on [Zulip]({{ site.zulip }})

{% include links.md %}
