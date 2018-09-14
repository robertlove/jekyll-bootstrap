---
title: Home

breadcrumb_items:
  - name: Home
    url: /
  - name: Library
    url: /library
  - name: Data
    url: /library/data

list_group:
  - Cras justo odio
  - Dapibus ac facilisis in
  - Vestibulum at eros
---

<div class="jumbotron">
  <h1 class="display-4">{{ site.title }}</h1>
  <p class="lead">{{ site.description }}</p>
  <hr class="my-4">
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. In risus lectus, volutpat eget eros eu, pellentesque placerat odio.</p>
  <a class="btn btn-primary btn-lg" href="{{ '/about' | prepend: site.baseurl }}">Learn more</a>
</div>

Duis justo odio, accumsan non tortor sed, suscipit pretium dui. Etiam eros lectus, vehicula et mauris in, dapibus feugiat diam. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum eget lacinia elit. Proin placerat arcu et est suscipit, quis condimentum felis dictum. Nunc sollicitudin, dui sed cursus pharetra, elit dui luctus justo, non fermentum urna ex id diam. Etiam volutpat mattis odio et blandit. Quisque consectetur rutrum tristique. Nullam convallis tellus id bibendum rutrum. Duis placerat turpis lobortis massa convallis, id condimentum neque congue. Curabitur molestie fringilla est. Nulla ante magna, pharetra eu dui id, sodales consectetur tellus. Phasellus id efficitur enim. Cras finibus laoreet lorem.

{% include components/alert.html
  content="A simple info alert with <a href='#' class='alert-link'>an example link</a>. Give it a click if you like."
  color="info"
  dismissible="true"
%}

{% include components/badge.html
  content="Badge"
  color="info"
  pill="false"
  url="#"
%}

{% include components/breadcrumb.html
  items=page.breadcrumb_items
%}

{% include components/button.html
  content="Button"
  color="info"
  type="submit"
  outline="true"
  size="lg"
  block="true"
  state="active"
%}

{% include components/card.html
  style="width: 20rem"
  width="50"
  text-align="center"
  header="Card Header"
  title="Card Title"
  subtitle="Card subtitle"
  text="Some quick example text to build on the card title and make up the bulk of the card's content."
  link="#"
  link-text="Card Link"
  body="<p class='card-text'>This card has supporting text below as a natural lead-in to additional content.</p><p class='card-text'><small class='text-muted'>Last updated 3 mins ago</small></p>"
  footer="Card Footer"
  img-top="https://via.placeholder.com/350x150"
  img-top-alt="Card Top Image"
  img-bottom="https://via.placeholder.com/350x150"
  img-bottom-alt="Card Bottom Image"
  list-group=page.list_group
%}
