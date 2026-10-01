---
# --- Shown on the landing page and at the top of this project page ----------
order: 1
field: Retail Robotics
title: Semi-Automated Retail Assistant Robot
tagline: >-
  Designing a physical retail-assistance prototype that combines a tablet interface,
  a POS demonstration, and Arduino-based proximity detection.
subtitle: "Independent Innovation and Technology Project | Project Leader: Diego Romero Nervi | Lima, Peru | 2026"
summary: >-
  A student-led engineering project that analysed retail checkout delays and built a
  physical prototype combining an MDF structure, a tablet interface and an Arduino
  proximity-detection subsystem.

tags:
  - Robotics
  - Semi-Automation
  - Retail Technology
  - Arduino
  - Prototyping
  - Engineering Design

card_image: retail-robot/prototype-front.jpg
hero_image: retail-robot/prototype-front.jpg
hero_narrow: true
hero_alt: The early cardboard and Arduino prototype of the retail assistant robot
hero_caption: Early prototype of the retail assistant robot, with the tablet interface mounted on the side.

# --- Buttons at the bottom of the page --------------------------------------
# Leave url blank until the record is published, then paste the link between
# the quotation marks. Nothing else needs to change.
doi: ""
citation: ""
buttons:
  - label: View Full Project Report
    url: ""
  - label: View Zenodo Record
    url: ""
---

<section class="section" markdown="1">
<div class="prose" markdown="1">

## Early Prototype and Functional Testing

An early physical prototype was built from a cardboard body mounted on an Arduino-based wheeled
chassis, with an ultrasonic sensor at the front and a tablet mounted on the side. The short clips
below show the prototype moving during functional testing.

</div>

<div class="wrap">
<div class="gallery">
  <figure>
    <img src="{{ '/assets/img/retail-robot/prototype-tablet-side.jpg' | relative_url }}" alt="Side view of the prototype with the tablet mounted" loading="lazy">
    <figcaption>Side view, showing the mounted tablet interface.</figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/img/retail-robot/prototype-wheels.jpg' | relative_url }}" alt="The prototype body on its wheeled chassis" loading="lazy">
    <figcaption>The prototype body on its wheeled chassis.</figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/img/retail-robot/prototype-chassis-sensor.jpg' | relative_url }}" alt="Arduino chassis with the ultrasonic sensor" loading="lazy">
    <figcaption>Arduino chassis with the ultrasonic sensor used for proximity detection.</figcaption>
  </figure>
</div>

<div class="gallery" style="margin-top:var(--gap-sm)">
  <figure>
    <video controls muted playsinline preload="none" poster="{{ '/assets/img/retail-robot/prototype-test-1.jpg' | relative_url }}">
      <source src="{{ '/assets/img/retail-robot/prototype-test-1.mp4' | relative_url }}" type="video/mp4">
    </video>
    <figcaption>Functional test: the prototype moving across the floor.</figcaption>
  </figure>
  <figure>
    <video controls muted playsinline preload="none" poster="{{ '/assets/img/retail-robot/prototype-test-2.jpg' | relative_url }}">
      <source src="{{ '/assets/img/retail-robot/prototype-test-2.mp4' | relative_url }}" type="video/mp4">
    </video>
    <figcaption>Functional test: a longer run of the prototype in operation.</figcaption>
  </figure>
</div>
</div>
</section>

<section class="section" markdown="1">
<div class="prose" markdown="1">

## The Problem

Long checkout lines can reduce service efficiency and negatively affect the retail shopping
experience. During the initial stage of the project, the team compared three problems: excessive
checkout waiting times, insufficient customer assistance and question resolution, and confusion
during the shopping experience.

Using a weighted problem-selection matrix, excessive checkout waiting times received the highest
score and was selected as the main problem to address.

</div>

<div class="prose">
<div class="table-wrap">
<table>
  <thead>
    <tr><th>Problem considered</th><th>Score</th></tr>
  </thead>
  <tbody>
    <tr><td>Excessive checkout waiting times</td><td>64</td></tr>
    <tr><td>Confusion during the shopping experience</td><td>48</td></tr>
    <tr><td>Insufficient customer assistance and question resolution</td><td>30</td></tr>
  </tbody>
</table>
</div>
</div>
</section>

<section class="section" markdown="1">
<div class="prose" markdown="1">

## The Idea

The team proposed a semi-automated retail assistant robot intended to support selected shopping
and customer-service functions. The physical prototype combines a wooden structure, a tablet-based
web interface, a POS device used for demonstration, and an Arduino-based electronic subsystem.

### What the prototype does

</div>

<div class="prose">
<ul class="cards">
  <li><strong>Tablet interface</strong> Simulates access to product, price and promotional information.</li>
  <li><strong>Product scanning concept</strong> Represents barcode scanning as part of the proposed shopping workflow.</li>
  <li><strong>POS demonstration</strong> Represents the payment stage of the proposed system.</li>
  <li><strong>Arduino proximity detection</strong> Uses an Arduino Mega, an ultrasonic sensor and LED indicators to implement basic obstacle and proximity detection.</li>
</ul>
</div>
</section>

<section class="section" markdown="1">
<div class="prose" markdown="1">

## Engineering Process

The team used a context mind map, a cause-and-effect (Ishikawa) diagram, a problem-selection
matrix and a weighted decision matrix to move from problem identification to solution selection
and prototype construction.

</div>

<div class="wrap">
<div class="gallery">
  <figure>
    <img src="{{ '/assets/img/retail-robot/mind-map.jpg' | relative_url }}" alt="Context mind map produced by the team" loading="lazy">
    <figcaption>Context mind map used to frame the retail problem. Original team working document, prepared in Spanish.</figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/img/retail-robot/ishikawa-diagram.jpg' | relative_url }}" alt="Cause and effect Ishikawa diagram produced by the team" loading="lazy">
    <figcaption>Cause-and-effect (Ishikawa) diagram identifying the causes of excessive checkout waiting times. Original team working document, prepared in Spanish.</figcaption>
  </figure>
</div>
</div>
</section>

<section class="section" markdown="1">
<div class="prose" markdown="1">

## Why This Solution?

Three alternatives were compared using implementation cost (35%), time to impact (25%) and
effectiveness (40%). The retail assistant robot received the highest weighted score.

</div>

<div class="prose">
<div class="table-wrap">
<table>
  <thead>
    <tr><th>Alternative considered</th><th>Weighted score</th></tr>
  </thead>
  <tbody>
    <tr><td>Retail assistant robot</td><td>3.60</td></tr>
    <tr><td>Digital queue and demand-management system</td><td>3.00</td></tr>
    <tr><td>Mobile payment system through an application</td><td>1.70</td></tr>
  </tbody>
</table>
</div>
</div>
</section>

<section class="section" markdown="1">
<div class="prose" markdown="1">

## Building the Prototype

The prototype was built from MDF wood and integrated a tablet, a POS device, an Arduino Mega, a
breadboard, Dupont wires, an ultrasonic sensor, LEDs, resistors and AA batteries. The construction
process included structural assembly, electronic connections, Arduino programming, development of
the tablet-based web interface, and installation of the demonstration components.

</div>

<div class="wrap">
<figure class="figure-single">
  <img src="{{ '/assets/img/retail-robot/construction-process.jpg' | relative_url }}" alt="Photographs of the prototype construction process" loading="lazy">
  <figcaption>Construction process, from structural assembly to Arduino wiring.</figcaption>
</figure>
</div>
</section>

<section class="section" markdown="1">
<div class="prose" markdown="1">

## What We Learned

The project provided hands-on experience in engineering design, electronics, programming,
prototyping and collaborative problem solving. It also highlighted the difference between building
a working physical prototype and validating a system in a real retail environment.

The payment, product-scanning and web-based shopping functions were simulated for the prototype,
while the Arduino subsystem implemented basic proximity detection. Future testing would be required
to determine whether the proposed system measurably reduces waiting times or improves customer
satisfaction.

</div>
</section>

<section class="section" markdown="1">
<div class="prose" markdown="1">

## Diego's Role

Diego Romero Nervi conceived the initiative as a collaborative project, brought together a group of
friends to develop it, and led and coordinated the team throughout the analysis, design and
prototype-construction process.

</div>
</section>

<section class="section" markdown="1">
<div class="prose" markdown="1">

## Next Steps

</div>

<div class="prose">
<ul class="cards">
  <li><strong>Validation</strong> Conduct controlled user tests and measure interaction times.</li>
  <li><strong>Usability</strong> Collect usability and satisfaction data.</li>
  <li><strong>Refinement</strong> Improve the physical structure and the digital interface.</li>
  <li><strong>Integration</strong> Explore integration with inventory and payment systems.</li>
  <li><strong>Documentation</strong> Document the Arduino code and the electronic architecture.</li>
</ul>
</div>
</section>
