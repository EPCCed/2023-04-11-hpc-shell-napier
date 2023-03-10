---
layout: lesson
root: .
permalink: index.html  # Is the only page that doesn't follow the pattern /:path/index.html
venue: Napier University
address: 
country: "UK"
language: "English"
latlng: 55.933146155905135, -3.2141915998127155
humandate: 11 April 2023
humantime: 09:30-16:00 BST
startdate: 2023-04-11
instructor: Tony Hallam
helper: 
email: ["support@archer2.ac.uk"]
collaborative_notes: 
---

This workshop is an introduction to using high-performance computing systems
effectively. We obviously can't cover every case or give an exhaustive course
on parallel programming in just two days of teaching time. Instead, this
workshop is intended to give students a good introduction and overview of the
tools available and how to use them effectively.

By the end of this workshop, students will know how to:

* Use the UNIX command line (also known as terminal or shell) to operate a
  computer, connect to a remote HPC system, and write simple shell scripts.

This lesson is part of a 2-day ARCHER2 course, you can find the material 
for day 2 at [Introduction to High Performance Computing](https://epcced.github.io/2023-04-12-hpc-intro-napier/).

<h2 id="general">General Information</h2>

{% comment %}
  LOCATION

  This block displays the address and links to maps showing directions
  if the latitude and longitude of the workshop have been set.  You
  can use https://itouchmap.com/latlong.html to find the lat/long of an
  address.
{% endcomment %}
<p id="where">
  <strong>Where:</strong>
  This course will be taught in person at <a href="https://www.accessable.co.uk/edinburgh-napier-university/access-guides/the-glassroom">The Glassroom</a>, Napier University, Edinburgh. All attendees will
  be sent the joining instructions prior to the event.
</p>
<iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d693.8732532289232!2d-3.2135287413311633!3d55.932869077044316!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4887c7094d1a3ff9%3A0x63b967e8d1488094!2sEdinburgh%20Napier%20University%20Merchiston%20Campus!5e0!3m2!1sen!2suk!4v1677580319047!5m2!1sen!2suk" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>

{% comment %}
  DATE

  This block displays the date and links to Google Calendar.
{% endcomment %}
{% if page.humandate %}
<p id="when">
  <strong>When:</strong>
  {{page.humandate}}.
  {% include workshop_calendar.html %}
</p>
{% endif %}

{% comment %}
  SPECIAL REQUIREMENTS

  Modify the block below if there are any special requirements.
{% endcomment %}
<p id="requirements">
  <strong>Requirements:</strong> Participants must bring a laptop with a
  Mac, Linux, or Windows operating system (not a tablet, Chromebook, etc.) that they are able to download and run software on. Specifically they should be able to run the portable version of <a href="https://mobaxterm.mobatek.net/download-home-edition.html">MobaXterm</a>.
  Alternatively, they should have a few specific software packages installed (listed
  <a href="#setup">below</a>). They are also required to abide by the <a href="https://www.archer2.ac.uk/training/code-of-conduct/">ARCHER2 Training Code of Conduct</a>.
</p>

{% comment %}
  ACCESSIBILITY

  Modify the block below if there are any barriers to accessibility or
  special instructions.
{% endcomment %}
<p id="accessibility">
  <strong>Accessibility:</strong> We are committed to making this workshop
  accessible to everybody. Accessibility details of the venue are outlined <a href="https://www.accessable.co.uk/edinburgh-napier-university/access-guides/the-glassroom">here</a>.
</p>
<p>
  Materials will be provided in advance of the workshop. If we can help making learning easier for
  you please get in touch (using contact details below) and we will attempt to provide them.
</p>

{% comment %}
  CONTACT EMAIL ADDRESS

  Display the contact email address set in the configuration file.
{% endcomment %}
<p id="contact">
  <strong>Contact</strong>:
  Please email
  {% if page.email %}
    {% for email in page.email %}
      {% if forloop.last and page.email.size > 1 %}
        or
      {% else %}
        {% unless forloop.first %}
        ,
        {% endunless %}
      {% endif %}
      <a href='mailto:{{email}}'>{{email}}</a>
    {% endfor %}
  {% else %}
    to-be-announced
  {% endif %}
  for more information.
</p>

<hr/>

> ## Prerequisites
> There are no prerequisites for this course.
{: .prereq}

> ## Requirements
> Participants must bring a laptop with a Mac, Linux, or Windows operating system (not a tablet,
> Chromebook, etc.) that they can download and run MobaXterm on. Alternatively, they should have a few specific software
> packages installed (listed in the Setup section below). They are also required to abide by the
> [ARCHER2 Training Code of Conduct](https://www.archer2.ac.uk/training/code-of-conduct/).
{: .prereq}
{: .prereq}
