---
layout: page
title: "Home"
class: home
---

# Hi, I'm Areen Khalaila

<div class="columns" markdown="1">

<div class="intro" markdown="1">
I research, design, and engineer solutions at the intersection of accessibility and technology.

I am currently pursuing a Bachelor of Science in Computer Science, with a minor in Physics, at [Brandeis University](https://www.brandeis.edu/), where I am a member of the Phi Beta Kappa honor society. My senior honors thesis, advised by Prof. Dylan Cashman, explores visual perception studies with tactile representations of data for visually impaired users.

I am a Research Intern at the [Human-Computer Interaction Institute](https://hcii.cmu.edu/) at [Carnegie Mellon University](https://www.cmu.edu/). I have conducted research under the guidance of [Patrick Carrington](https://www.patrickcarrington.com/) and Franklin Mingzhi Li, using AI to enhance cooking experiences for visually impaired individuals. 

I am always open to new opportunities and collaborations. Feel free to reach out to me via email at first name kh at brandeis dot edu or on [LinkedIn](https://www.linkedin.com/in/areenkh). Check out my [GitHub](https://github.com/areenkh).

<!-- Upcoming: Adobe, Atlassian?, Highcharts, UW-Madison's WGNHS, ?? -->

</div>

<div class="me" markdown="1">
<picture>
  <source srcset='images/areenkh.png' type='image/png' />
  <img
    src='images/areenkh.png'
    alt="this is me smiling, wearing a white top and a black blazer on top">
</picture>

{:.no-list}
* <a href="mailto:{{ site.email }}">{{ site.email }}</a>
* {{ site.address }}
<p>Fun fact about me is my name <br>
in Arabic means lion's den.</p>
</div>

</div>

<!-- ## Featured <a href="{{ "/projects/" | relative_url }}">Projects</a>

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
</a> -->

<!-- ## Featured <a href="{{ "/publications/" | relative_url }}">Publications</a>

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
</a> -->

<!-- ## My background

<div class="intro" markdown="1">

In 2021, I came to the United States as an international student to pursue an undergraduate degree at [Brandeis University](https://www.brandeis.edu/) in the Boston area. My passion for computer science began in eighth grade, learning to code in C# and later expanding into web development with ASP.NET. Recognizing my achievements, Brandeis awarded me a prestigious full-ride scholarship, which is given to 1 student every 4 years.

Thanks to my strong coding background, I became a teaching assistant in my first year at Brandeis. I am now a Head Teaching Assistant and lead weekly recitations while managing grading tasks and coordinating with other TAs.

At the Brandeis Visual Analytics Lab, under the guidance of Professor Dylan Cashman, we work on research focusing on visual perception studies with tactile data for visually impaired users. Additionally, I am a student researcher at the [Human-Computer Interaction Institute](https://hcii.cmu.edu/) at [Carnegie Mellon University](https://www.cmu.edu/). At the AXLE Lab, under the guidance of [Patrick Carrington](https://www.patrickcarrington.com/), I research assistive technology to enhance cooking experiences for visually impaired individuals. -->

<!-- Upcoming: Adobe, Atlassian?, Highcharts, UW-Madison's WGNHS, ?? -->


<!-- </div> -->

<div class="news-travel" markdown="1">

<div class="news" markdown="1">
## Latest News

<ul>
{% for news in site.data.news limit:10 %}
  <li>{% include news.html news=news %}</li>
{% endfor %}
</ul>

</div>
</div>

<div class="journey-pics" markdown="1">
<div class="journey" markdown="1">
## Highlights from My Journey

<div class="photo-grid">
  <div class="photo-container">
    <img src="{{ '/images/journey/IMG_4147.PNG' | relative_url }}" alt="Poster Presentation">
    <div class="overlay">Final Poster Presentation at CMU HCII REU 2024</div>
  </div>
  <div class="photo-container">
    <img src="{{ '/images/journey/brandies_urcc.png' | relative_url }}" alt="Conference Talk">
    <div class="overlay">Brandeis URCC Research Symposium 2024</div>
  </div>
  <div class="photo-container">
    <img src="{{ '/images/journey/IMG_0974.JPG' | relative_url }}" alt="Graduation Ceremony">
    <div class="overlay">High School Graduation</div>
  </div>
  <div class="photo-container">
    <img src="{{ '/images/journey/1718582117115.jpeg' | relative_url }}" alt="CMU HCII REU First Day">
    <div class="overlay">CMU HCII REU Orientation</div>
  </div>
  <div class="photo-container">
    <img src="{{ '/images/journey/IMG_1248.JPG' | relative_url }}" alt="Coding Camp in 2021">
    <div class="overlay">Coding Camp in 2021</div>
  </div>
  <!-- Add more photos as needed -->
</div>
</div>

<!-- <div class="travel" markdown="1">
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

</div> -->

</div>
