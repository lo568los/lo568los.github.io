---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a first-year Physics PhD student and a Lanczos and Dean Fellow at the University of Maryland, College Park. I graduated summa cum laude from the Indian Institute of Science (IISc) Bangalore with an Integrated BS-MS in Physics and an additional minor in Quantum Technologies. I believe that a rigorous foundation at the intersection of physics, computer science, and mathematics is essential for advancing modern quantum technologies.

My research primarily focuses on quantum information theory, quantum computing, and their structural applications within condensed matter physics. I am particularly interested in exploring quantum error correction, open quantum systems and designing novel quantum circuits fault-tolerantly for simulating physical systems. Recently, I have also dabbled in quantum resource theories. I am always eager to collaborate on intriguing new ideas across these domains.

Email: ssarma03(at)umd(dot)edu

<a href="https://info.flagcounter.com/piz4"><img src="https://s05.flagcounter.com/count2/piz4/bg_FFFFFF/txt_000000/border_CCCCCC/columns_8/maxflags_10/viewers_0/labels_0/pageviews_0/flags_0/percent_0/" alt="Free counters!" border="0"></a>



Recent Research Experience:
---

- From Spring 2025 to 2026, I worked with Dariel Mok, Tobias Haug and John Preskill on magic of equilibrium states in quantum chaotic Hamiltonians.  
- Starting Srping 2025, I was a visiting student researcher for two months at A*STAR Agency, Singapore, under the guidance of Kishor Bharti.  
- From Fall 2024 to 2025, I was a Long Term Visiting student fellow at ICTS, working with Manas Kulkarni.  
- In the summer of 2024, I was a DAAD-WISE Fellow working with Elio Koenig.  
- In the summer of 2022, I was a National Initiative for Undergraduate Students Fellow at HBCSE-TIFR, and subsequently under the guidance of Deepak Dhar.

Recent Publications:
---
\* denotes equal contribution

<ul>
{% for post in site.publications reversed limit:5 %}
  <li>
    {{ post.title }}<br>
    {{ post.authors }}  <br>
    {% if post.extra %}
      {% if post.venue_url%}
        <em><a href="{{ post.venue_url }}">{{ post.venue }} ({{ post.date | date: "%Y" }})</a>, {{post.extra}}</em>.
      {% else %}
        <em>{{ post.venue }} ({{ post.date | date: "%Y" }}), {{post.extra}}</em>.
      {% endif %}
    {% else %}
      {% if post.venue_url%}
      <em><a href="{{ post.venue_url }}">{{ post.venue }} ({{ post.date | date: "%Y" }})</a></em>.
      {% else %}
        <em>{{ post.venue }} ({{ post.date | date: "%Y" }})</em>.
      {% endif %}
    {% endif %}


    {% if post.paperurl %}
      [<a href="{{ post.paperurl }}">PDF</a>]
    {% endif %}

    {% for link in post.extra_links %}
      [<a href="{{ link.url }}">{{ link.name }}</a>]
    {% endfor %}
  </li>
{% endfor %}
</ul>
