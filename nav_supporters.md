---
layout: frame
title: "- Supporters"
icon: <i class="fas fa-handshake"></i>
permalink: /supporters/
---
<section class="page-header" style="padding-bottom:1px">
  <div class="container" style="color: #ffffff">
    <h1 style="font-size: 3em;">{{ page.icon }}{{ page.title }}</h1>
    <p>행사를 열고 진행하는데 도움을 주신 분들입니다.</p>
  </div>
</section>
<div class="container" style="padding-top:32px; padding-bottom:32px; ">
  <div class="row">
    <div style="padding: 5px 5px 5px 5px; margin: auto; float:center; text-align:center">
    {% for host-b in site.host-b %}
    <div class="card" style="width: 20rem; height: auto;">
      <img class="card-img-top" src="{{ site.baseurl }}/assets/imgs/{{ host-b.image }}" alt="{{ host-b.name }}" style="max-width: 100%;height: 10rem;">
      <div class="card-body">
        <h5 class="card-title">{{ host-b.name }}</h5>
        <p class="card-text">{{ host-b.desc }}</p>
        <a href="{{ host-b.url }}" class="btn btn-primary">웹사이트 방문</a>
      </div>
    </div>
    {% endfor %}
    </div>

    <div style="padding: 5px 5px 5px 5px; margin: auto; float:center; text-align:center">
    {% for host-a in site.host-a %}
    <div class="card" style="width: 20rem; height: auto;">
      <img class="card-img-top" src="{{ site.baseurl }}/assets/imgs/{{ host-a.image }}" alt="{{ host-a.name }}" style="max-width: 100%;height: 10rem;">
      <div class="card-body">
        <h5 class="card-title">{{ host-a.name }}</h5>
        <p class="card-text">{{ host-a.desc }}</p>
        <a href="{{ host-a.url }}" class="btn btn-primary">웹사이트 방문</a>
      </div>
    </div>
    {% endfor %}
    </div>

    <div style="padding: 5px 5px 5px 5px; margin: auto; float:center; text-align:center">
    {% for host-c in site.host-c %}
    <div class="card" style="width: 20rem; height: auto;">
      <img class="card-img-top" src="{{ site.baseurl }}/assets/imgs/{{ host-c.image }}" alt="{{ host-c.name }}" style="max-width: 100%;height: 10rem;">
      <div class="card-body">
        <h5 class="card-title">{{ host-c.name }}</h5>
        <p class="card-text">{{ host-c.desc }}</p>
        <a href="{{ host-c.url }}" class="btn btn-primary">웹사이트 방문</a>
      </div>
    </div>
    {% endfor %}
    </div>
    
    <div style="padding: 5px 5px 5px 5px; margin: auto; float:center; text-align:center">
    {% for supporters in site.supporters %}
    <div class="card" style="width: 20rem; height: auto;">
      <img class="card-img-top" src="{{ site.baseurl }}/assets/imgs/{{ supporters.image }}" alt="{{ supporters.name }}" style="max-width: 100%;height: 10rem;">
      <div class="card-body">
        <h5 class="card-title">{{ supporters.name }}</h5>
        <p class="card-text">{{ supporters.desc }}</p>
        <a href="{{ supporters.url }}" class="btn btn-primary">웹사이트 방문</a>
      </div>
    </div>
    {% endfor %}
    </div>

  </div>
</div>
{% include sponsors.html %}
