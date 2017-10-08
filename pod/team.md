---
title: "Das Team"
---

# Das Team

Wer sich schon immer gefragt hat, wer den Pod eigentlich betreibt und betreut...

{% for member in site.team %}
  <div class="team-member clearfix">
    <h3>{{member.name}}</h3>

    <img alt="Profile {{member.name}}" src="{{member.picture}}" class="img-thumbnail rounded float-right">

    <p class="lead">{{member.introduction}}</p>
    <dl class="row">
      <dt class="col-sm-2">
        diaspora*
      </dt>
      <dd class="col-sm-10">
        <a href="{{member.diaspora_link}}" target="_blank">{{member.diaspora}}</a>
      </dd>

      <dt class="col-sm-2">
        eMail
      </dt>
      <dd class="col-sm-10">
        <a href="mailto:{{member.email}}" target="_blank">{{member.email}}</a>
      </dd>

      <dt class="col-sm-2">
        Rollen
      </dt>
      <dd class="col-sm-10">
        {{member.content}}
      </dd>
    </dl>
  </div>
{% endfor %}
