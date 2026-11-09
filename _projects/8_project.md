---
layout: page
title: MRI Imaging Project
description: A project that used test sets of MRI images to expedite testing of MRI machines.
img: assets/img/MRI-Phantom.jpg
importance: 3
category: work
---

This was a placement project where me and three other students created a pipeline for MRI phantom test images.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/MRI6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/MRI2.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
      We created this pipeline in the interest of expediting the testing process that every MRI machine must undertake yearly according to law.
      These tests take around a day sometimes longer and the machine is down for the entire duration. The pipeline uses python machine learning in order to speed this up and return pass or fail based on the model.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/MRI4.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

The project was largely successful and we were able to showcase an application that was housed on aws cloud services. We deployed a website that allowed a user to send zip files to the cloud server using flask and it was recieved into a bit bucket where it was then processed by the algorithm and a report was generated and returned to the webpage.
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/MRI1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Image results
</div>
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
      {% include figure.liquid path="assets/img/MRI5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
    Flask Code Snippet
</div>
We used Flask, a lightweight Python web framework, to handle the server-side functionality of my MRI ACR QA application. Flask manages the application's routes and HTTP requests, allowing the frontend to communicate with the backend through API endpoints. It handles user authentication and registration, processes uploaded ZIP files containing MRI DICOM images, and triggers the relevant image analysis algorithms. It also returns analysis results in JSON format, serves MRI slice images and generates downloadable PDF reports. Overall, Flask acts as the link between the frontend, backend processing and the application's data, allowing the different features to work together.
