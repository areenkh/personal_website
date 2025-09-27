---
layout: page
title: "Home"
class: home
---

# Hi, I'm Areen Khalaila

<div class="columns" markdown="1">
<div class="intro" markdown="1">
I design and study accessible systems for non-visual data interaction. My research sits at the intersection of human–computer interaction, data visualization, and accessibility, with a particular focus on tactile graphics and multisensory interfaces for blind and low-vision (BLV) users. I aim to develop frameworks, design guidelines, and interactive tools that expand how people with disabilities can perceive, create, and engage with data.

I am currently a PhD student in Computer Science at Tulane University. Previously, I completed my BSc in Computer Science (summa cum laude) at Brandeis University, where I received the full-ride Malkin Scholarship and the departmental Jacques Cohen Award for outstanding research. During my undergraduate studies, I was a member of the [BraVa lab](https://brandeis-visual-analytics.github.io/brava.github.io/) and mentored by Dr. [Patrick Carrington](https://patrickcarrington.com) and [Frankling Mingzhi Li](https://franklin-li.com) at [Human-Computer Interaction Institute](https://hcii.cmu.edu) at Carnegie Mellon University. 

My work has introduced new insights into tactile chart perception, design implications for accessible graphics, and interactive systems for inclusive learning. This research has been recognized with a Best Paper Award at IEEE VIS 2025 and published across premier venues in visualization and accessibility, including IEEE VIS, CHI, and ASSETS.

Through my work, I aim to reimagine visualization beyond sighted norms, designing systems that allow users with disabilities not only to access data, but to explore, interpret, and author it on their own terms. 
Feel free to contact me and check my [CV](https://areenkh.com/cv/) for more details.

<!-- 


I research, design, and engineer solutions at the intersection of accessibility and technology.

I just completed a Bachelor of Science in Computer Science, with a minor in Physics, at [Brandeis University](https://www.brandeis.edu/) with highest honors. I was advised by Prof. [Dylan Cashman](https://dylancashman.github.io) as part of the BraVa lab . My senior honors thesis, titled "From Touch to Insight: Exploring Tactile Strategies and Design Guidelines for Non-Visual Graphical Perception," explored visual perception studies with tactile representations of data for visually impaired users. Throughout my time at Brandies, I have received several awards, which you can find in my [CV](https://areenkh.com/cv/).

I was formerly a research intern at the [Human-Computer Interaction Institute](https://hcii.cmu.edu/) at [Carnegie Mellon University](https://www.cmu.edu/). I conducted research under the guidance of [Patrick Carrington](https://www.patrickcarrington.com/) and Franklin Mingzhi Li, using form factor cameras to enhance cooking experiences for visually impaired individuals.

Outside of research, I was a teaching assistant (TA) for different Computer Science courses, ranging from introductory classes to more advances ones, every semester since freshamn year. I also led both small and big classes as a head TA. I served as a mentor for first-gen students, offering them academic support.

I am always open to new opportunities and collaborations. Feel free to reach out to me via email at first name kh at brandeis dot edu or on [LinkedIn](https://www.linkedin.com/in/areenkh). Check out my [GitHub](https://github.com/areenkh). -->

</div>

<div class="me" markdown="1">
<picture>
  <source srcset='images/areenkh.png' type='image/png' />
  <img
    src='images/areenkh.png'
    alt="this is me smiling, wearing a white top and a black blazer on top">  
</picture>

{:.no-list}

- <a href="mailto:{{ site.email }}">{{ site.email }}</a>
- {{ site.address }}
<p>Fun fact about me is my name <br>
in Arabic means lion's den.</p>
</div>
</div>

## Featured Projects

<div class="featured-projects">
  {% assign sorted_projects = site.data.projects | sort: 'highlight' %}
  {% for project in sorted_projects %}
    {% if project.highlight %}
      {% include project.html project=project %}
    {% endif %}
  {% endfor %}
</div>
<a href="https://github.com/areenkh" class="button">
  <i class="fas fa-chevron-circle-right"></i>
  Show More Projects
</a>

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
<!-- <ul>
{% for news in site.data.news limit:10 %}
  <li>{% include news.html news=news %}</li>
{% endfor %}
</ul> -->
<ul id="news-list">
    {% for news in site.data.news %}
      <li class="news-item{% if forloop.index > 5 %} hidden{% endif %}">{% include news.html news=news %}</li>
    {% endfor %}
  </ul>
  <!-- <button id="show-more-btn" onclick="showMoreNews()">Show More</button> -->
</div>
</div>
<div class="journey-pics" markdown="1">
## Pieces of My Life
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
    <div class="photo-container">
      <img src="{{ '/images/journey/cs-graduation-ceremony.JPG' | relative_url }}" alt="Me on the stage receiving an award at the graduation ceremony">
      <div class="overlay">Computer Science Graduation Ceremony
      </div>
    </div>
    <div class="photo-container">
      <img src="{{ '/images/journey/graduation-pic.JPEG' | relative_url }}" alt="A picture of me in my graduation dress with my graduation cap on">
      <div class="overlay">Graduation Photoshoot
      </div>
    </div>
        <div class="photo-container">
      <img src="{{ '/images/journey/StreetScape.png' | relative_url }}" alt="My teammates and I holding a check award for our project">
      <div class="overlay">Asper Award for Global Entrepreneurship
      </div>
    </div>
  </div>
</div>

<!-- <a href="{{ "/journey/" | relative_url }}" class="button">
  <i class="fas fa-chevron-circle-right"></i>
  Show All Images
</a>  -->


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

<!-- </div> -->
