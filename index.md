---
layout: page
title: "Home"
class: home
---

# Hi, I'm Frank Elavsky

<div class="columns" markdown="1">

<div class="intro" markdown="1">
I research, design, and engineer solutions at the intersection of accessibility and technology. I am passionate about improving the usability of technology for visually impaired users and consider myself both a creator and a problem-solver.

I am a Research Intern at the [Human-Computer Interaction Institute](https://hcii.cmu.edu/) at [Carnegie Mellon University](https://www.cmu.edu/). I have conducted research under the guidance of [Patrick Carrington](https://www.patrickcarrington.com/) and Franklin Mingzhi Li, focusing on assistive technology to enhance cooking experiences for visually impaired individuals. My work involves evaluating different camera specifications to provide real-time visual feedback and guidance in kitchen environments.

I am currently pursuing a Bachelor of Science in Computer Science, with a minor in Physics, at [Brandeis University](https://www.brandeis.edu/), where I am a member of the Phi Beta Kappa honor society. My senior honors thesis, advised by Prof. Dylan Cashman, explores visual perception studies with tactile representations of data for visually impaired users.

In addition to my academic pursuits, I offer part-time consulting services on a case-by-case basis, from single-session calls to larger, ongoing projects. My recent collaborations include projects with [Apple](https://www.apple.com/) <i class="fab fa-apple"></i>, [Fizz Studio](https://fizz.studio/), and [SRI](https://www.sri.com/research/education-learning/).

I am always open to new opportunities and collaborations. Feel free to reach out to me via [LinkedIn](https://www.linkedin.com/in/areenkh) or [GitHub](https://github.com/areenkh).

<!-- Upcoming: Adobe, Atlassian?, Highcharts, UW-Madison's WGNHS, ?? -->

</div>

<div class="me" markdown="1">
<picture>
  <source srcset='/images/frank.jpg' type='image/jpg' />
  <img
    src='/images/frank.jpg'
    alt="It's me! A white man smiling with medium-short brown hair, glasses, and a grey t-shirt.">
</picture>

{:.no-list}
* <a href="mailto:{{ site.email }}">{{ site.email }}</a>
* {{ site.address }}
</div>

</div>

## Featured <a href="{{ "/projects/" | relative_url }}">Projects</a>

<div class="featured-projects">
  {% assign sorted_projects = site.data.projects | sort: 'highlight' %}
  {% for project in sorted_projects %}
    {% if project.highlight %}
      {% include project.html project=project %}
    {% endif %}
  {% endfor %}
</div>
<a href="{{ "/projects/" | relative_url }}" class="button">
  <i class="fas fa-chevron-circle-right"></i>
  Show More Projects
</a>

## Featured <a href="{{ "/publications/" | relative_url }}">Publications</a>

<div class="featured-publications">
  {% assign sorted_publications = site.publications | sort: 'year' | reverse %}
  {% for pub in sorted_publications %}
    {% if pub.highlight %}
      <a href="{{ pub.html }}" class="publication">
        <strong>{{ pub.title }}</strong>
        <span class="authors">{% for author in pub.authors %}{{ author }}{% unless forloop.last %}, {% endunless %}{% endfor %}</span>.
        <i>{% if pub.venue %}{{ pub.venue }}, {% endif %}{{ pub.year }}</i>.
        {% for award in pub.awards %}<br/><span class="award"><i class="fas fa-{% if award == "Best Paper Award" %}trophy{% else %}award{% endif %}" aria-hidden="true"></i> {{ award }}</span>{% endfor %}
      </a>
    {% endif %}
  {% endfor %}
</div>

<a href="{{ "/publications/" | relative_url }}" class="button">
  <i class="fas fa-chevron-circle-right"></i>
  Show All Publications
</a>

## My background

<div class="intro" markdown="1">

Before embarking on a PhD I was a staff design systems engineer at Visa on their Data Experience team and lead contributor to the accessibility efforts of their first open source library, [Visa Chart Components](https://github.com/visa/visa-chart-components). We were able to do some pretty extraordinary things together and I am fortunate to have worked alongside such world-class folks.

Prior to Visa I had a high-octane 2 years at Northwestern University working for Research Computing Services providing data visualization support to over two dozen research projects across a wide range of disciplines. Several of my projects [won awards](https://www.frank.computer/cv/#awards) and have been featured in over 60 research publications (including the privilege of being uncredited in the [2017 Nobel Lecture on Physics](https://journals.aps.org/rmp/abstract/10.1103/RevModPhys.90.040502)), 100+ web articles, 4 PhD theses, 4 graduate courses, and [9 textbooks](https://www.google.com/search?q=%22Frank+elavsky%22&hl=en&tbm=bks&sxsrf=APq-WBuA3-rFi5BAWgvu7rf_ax78Iee66w:1648824562316&ei=8hBHYsf-Eu-FytMPsZ-B0AI&start=0&sa=N&ved=2ahUKEwjHv9WSjvP2AhXvgnIEHbFPACo4ChDy0wN6BAgBED0&biw=896&bih=931&dpr=2).

In my early career (before Northwestern), I worked in federal policy analyzing large, complex medicare/medicaid datasets and building visualization tools for lawyers and policymakers.

</div>

<div class="news-travel" markdown="1">

<div class="news" markdown="1">
## Latest News

<ul>
{% for news in site.data.news limit:10 %}
  {% include news.html news=news %}
{% endfor %}
</ul>

</div>

<div class="travel" markdown="1">
## Latest Visits

<table>
<tbody>
{% assign future_travel = site.data.travel | where_exp:'item','item.start == null' %}
{% for travel in future_travel %}
  {% include travel.html travel=travel %}
{% endfor %}
{% assign sorted_travel = site.data.travel | where_exp:'item','item.start' | sort: 'start' | reverse %}
{% for travel in sorted_travel limit:10 %}
  {% include travel.html travel=travel %}
{% endfor %}
</tbody>
</table>

</div>

</div>
