---
layout: page
title: tfCodeGenerator Playground
description: Tensorflow playground with code generation
img: assets/img/tf-logo.png
importance: 2
category: machine learning
---

Tensorflow plaground is a website developed by the tensorflow team to help visualize how neural networks learn. It's available <a href="https://playground.tensorflow.org/#activation=tanh&batchSize=10&dataset=circle&regDataset=reg-plane&learningRate=0.03&regularizationRate=0&noise=0&networkShape=4,2&seed=0.65008&showTestData=false&discretize=false&percTrainData=50&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false&hideText=false">here</a>.

It however did not give the code for implementing the visualized model in python. So we modfified the code and UI to generate th corresponding code. Our version of the site is available <a href="https://co-science.github.io/tfCodeGenerator-playgroud/#activation=tanh&batchSize=10&dataset=circle&regDataset=reg-plane&learningRate=0.03&regularizationRate=0&noise=0&networkShape=4,2&seed=0.64197&showTestData=false&discretize=false&percTrainData=50&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false&hideText=false">here</a>.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="assets/video/2023-07-08 19-13-28.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="caption">
    Demo of our deployed site
</div>

Check out the modified code <a href="https://github.com/Co-Science/tfCodeGenerator-playgroud">here</a>.

The edits were done in typescript, and the generated code is in python.

A lot of the information regarding the visualized model was available in the site url itself. So it was simply a job of parsing it and printing the corresponding python code.