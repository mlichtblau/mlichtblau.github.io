---
title: "Hi, my name is Marius"
layout: splash
permalink: /
date: 2023-04-18T21:47:00+02:00
header:
  overlay_color: "#000"
  overlay_filter: "0.7"
  overlay_image: /assets/images/cinque-terre-splash.jpg
  actions:
    - label: "Education"
      url: "/#education"
      button:
        style_class: ".btn--inverse"
        size_class: "btn--small"
    - label: "Experience"
      url: "/#experience"
      button:
        style_class: ".btn--inverse"
        size_class: "btn--small"
    - label: "Projects"
      url: "/#projects"
      button:
        style_class: ".btn--inverse"
        size_class: "btn--small"
  caption: "Cinque Terre (2022)"
excerpt: "Welcome to my Homepage.<br>Find out more about me and my work below.<br>Or checkout the [blog](/blog). (soon...)"
feature_row_me:
  - image_path: /assets/images/me.jpg
    alt: "Marius"
    title: "About me"
    excerpt: "I am Software Engineering Master student living in Munich.<br>I like programming and finding solutions to difficult problems.<br>When I don't code I like to travel, ride my motorbike or take pictures with my film camera."
    url: "/blog"
    btn_label: "Go to Blog"
    btn_class: "btn--inverse"
gallery:
  - url: /assets/images/meer.jpg
    image_path: /assets/images/meer-th.jpg
    alt: "Dark sand"
    title: "California, 2019"
  - url: /assets/images/ocean.jpg
    image_path: /assets/images/ocean-th.jpg
    alt: "Waves near the shore"
    title: "California, 2020"
  - url: /assets/images/motorrad.jpg
    image_path: /assets/images/motorrad-th.jpg
    alt: "Motorbikes in front of forrest"
    title: "Montenegro, 2020"
master:
  - title: "Software Engineering Elite Graduate Program (Master)"
    time: "2020 - now"
    location: "TU Munich, LMU, Universität Augsburg"
    images:
      - image_path: /assets/images/tum.png
        alt: "TU München Logo"
      - image_path: /assets/images/lmu.png
        alt: "LMU München Logo"
      - image_path: /assets/images/augsburg.png
        alt: "Universität Augsburg Logo"
    excerpt: 'The Software Engineering Elite Graduate Program provides a unique learning opportunity with allowing only 16 students per year. I am currently taking a variety of courses from "modelling, specification and verification of reactive systems" to "database implementations". I will receive my Master egree in 2022.'
    url: "https://elite-se.informatik.uni-augsburg.de/"
    btn_label: "Program Homepage"
    btn_class: "btn--inverse"
bachelor:
  - title: "IT Systems Engineering (Bachelor)"
    time: "2016 - 2019"
    location: "Hasso-Plattner-Institut"
    images:
      - image_path: /assets/images/hpi.png
        alt: "Hasso Plattner Institut Logo"
    excerpt: 'My bachelor studies included a broad range of topics around computer science and software engineering. I particularly enjoyed the theoretical classes as I loved finding solutions to hard problems in the exercises. For my bachelors project I used process modelling and execution tools to optimise the delivery of parcels on the last mile to the receiver.'
    url: "https://hpi.de/en/studies/before-the-study/degree-programs/bachelor.html"
    btn_label: "Program Homepage"
    btn_class: "btn--inverse"
celonis:
  - title: "Celonis"
    time: "2021 - now"
    location: "Munich, Germany"
    images:
      - image_path: /assets/images/celonis.png
        alt: "Celonis Logo"
        width: 160px
    excerpt: 'I am a software engineering working student in the SaolaDB team at Celonis. The SaolaDB is a fast in-memory database built for business processes, that allows customers to use the PQL language for process mining. I am currently working on the Java Spring microservices responsible for delivering fast and reliable access to the database while scaling to the large number of new customers.'
    url: "https://www.celonis.com/"
    btn_label: "Homepage"
    btn_class: "btn--inverse"
koppla:
  - title: "Koppla"
    time: "2020"
    location: "Potsdam, Germany (Remote)"
    images:
      - image_path: /assets/images/koppla.png
        alt: "Koppla Logo"
        width: 160px
    excerpt: 'At Koppla I was working on the GraphQL backend using TypeScript. I developed new features in a test driven environment and helped transitioning from a monolithic architecture to Microservices. Specifically I was responsible for designing and developing the notification Microservice, which delivered push notifications to the customer apps.'
    url: "https://www.koppla.de/"
    btn_label: "Homepage"
    btn_class: "btn--inverse"
sap:
  - title: "SAP"
    time: "2019-2020"
    location: "Palo Alto, California"
    images:
      - image_path: /assets/images/sap.png
        alt: "SAP Logo"
        width: 160px
    excerpt: 'As a software engineering intern at SAP Labs Silicon Valley I helped develop an internal prototype for improving the hiring process at SAP. In cooperation with local hiring managers we built an application, using SAP process automation tools on SAP Cloud Platform, to automate manual tasks, improve transparency for applicants and provide analytics to the Talent Acquisition team at SAP.'
    url: "https://www.sap.com/about/sap-labs-silicon-valley.html"
    btn_label: "Homepage"
    btn_class: "btn--inverse"
freiheit-software:
  - title: "freiheit.software"
    time: "2017-2018"
    location: "Potsdam, Germany"
    images:
      - image_path: /assets/images/freiheit-software.jpg
        alt: "freiheit.software Logo"
        width: 160px
    excerpt: 'Using an agile approach our team of four developers created web projects for a variety of customers. I specialised in front end development using Angular and JQuery. Amongst other things I built a tool to create and sign PDF documents online and a single page ticket shop for an event agency.'
    url: "https://freiheit.software/"
    btn_label: "Homepage"
    btn_class: "btn--inverse"
projects:
  - image_path: /assets/images/spotihub.png
    alt: "SpotiHub Logo"
    # title: "SpotiHub"
    excerpt: "Colaboration and Version Control for your Spotify playlists."
    url: "https://spotihub.com/"
    btn_label: "SpotiHub"
    btn_class: "btn--inverse"
  - image_path: /assets/images/kraggl.png
    alt: "Kraggl Logo"
    # title: "SpotiHub"
    excerpt: "(Archived) Integrate your time tracking with Toggl in your project management with GitKraken Boards."
    url: "https://github.com/mlichtblau/kraggl"
    btn_label: "Kraggl GitHub"
    btn_class: "btn--inverse"
  - title: "More"
    excerpt: "Maybe?"
---

<div class="text-center" id="feature-row-container">
{% include feature_row id="feature_row_me" type="right" %}
</div>

{% include gallery class="if-big-screen" %}

## Education
{: .text-center}

{% include timeline_row id="master" %}

{% include timeline_row id="bachelor" %}

## Experience
{: .text-center}

{% include timeline_row id="celonis" %}

{% include timeline_row id="koppla" %}

{% include timeline_row id="sap" %}

{% include timeline_row id="freiheit-software" %}

## Projects
{: .text-center}

{% include feature_row id="projects" %}