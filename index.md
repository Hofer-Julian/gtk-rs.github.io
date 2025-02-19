---
layout: no-wrapper
---

<section markdown="1">

# Unlock the GNOME stack for Rust

<p style="text-align: center; margin: 0 2em;" markdown="1">
The **gtk-rs** project provides safe bindings to the [Rust] language for fundamental libraries from the GNOME stack like [GLib], [Cairo], [GTK 3][GTK] and [GTK 4][GTK].
</p>

[Rust]: https://www.rust-lang.org
[GLib]: https://developer.gnome.org/glib
[GTK]: https://gtk.org
[Cairo]: https://cairographics.org/documentation/

<div class="post-overview">
{% for post in site.categories.front limit:3 %}
  <a href="{{ post.url | prepend: site.baseurl }}">
      <span class="post-meta">{{ post.date | date: "%-d %b %Y" }}</span>
      <div>{{ post.title }}</div>
  </a>
{% endfor %}
</div>

<p markdown="1" class="badgets">
[![Open Collective backers and sponsors](https://img.shields.io/opencollective/all/gtk-rs?color=%2399c9ff&label=Support%20us%20on%20open%20collective&logo=open-collective&logoColor=white&style=for-the-badge&labelColor=%233385ff)](https://opencollective.com/gtk-rs)
</p>

## Available crates

The following table contains the most popular crates of **gtk-rs**. More information on all existing crates is available under the corresponding links in the **Project** column in the table below.

<!--
{% include crates.html %}
-->

<table>
<thead>
  <tr><th>Project</th><th colspan="2">Crate</th><th>Docs</th></tr>
</thead>
<tbody>

  <tr>
    <td class="section">
      <a href="/gtk-rs-core">Core</a>
    </td>
    <td>
      <a href="https://crates.io/crates/cairo-rs">
        cairo-rs
      </a>
    </td>
    <td>
      v0.9.0
    </td>
    <td class="docs">
      <a href="/gtk-rs-core/stable/latest/docs/cairo">🕮</a>
    </td>
  </tr>

  <tr>
    <td class="section">
      <a href="/gtk-rs-core"></a>
    </td>
    <td>
      <a href="https://crates.io/crates/gio">
        gio
      </a>
    </td>
    <td>
      v0.9.0
    </td>
    <td class="docs">
      <a href="/gtk-rs-core/stable/latest/docs/gio">🕮</a>
    </td>
  </tr>

  <tr>
    <td class="section">
      <a href="/gtk-rs-core"></a>
    </td>
    <td>
      <a href="https://crates.io/crates/glib">
        glib
      </a>
    </td>
    <td>
      v0.10.0
    </td>
    <td class="docs">
      <a href="/gtk-rs-core/stable/latest/docs/glib">🕮</a>
    </td>
  </tr>

  <tr>
    <td class="section">
      <a href="/gtk-rs-core"></a>
    </td>
    <td>
      <a href="https://crates.io/crates/pango">
        pango
      </a>
    </td>
    <td>
      v0.9.0
    </td>
    <td class="docs">
      <a href="/gtk-rs-core/stable/latest/docs/pango">🕮</a>
    </td>
  </tr>

  <tr>
    <td class="section">
      <a href="/gtk3-rs">GTK 3</a>
    </td>
    <td>
      <a href="https://crates.io/crates/gtk">
        gtk
      </a>
    </td>
    <td>
      v0.9.0
    </td>
    <td class="docs">
      <a href="/docs/gtk/">🕮</a>
    </td>
  </tr>

</tbody>
</table>

</section>

<section class="special" markdown="1">

## The introductory book

<div class="with-logo">

{% include book.svg %}

<div markdown="1">
Julian Hofer is writing a book titled [*GUI development with Rust and GTK 4*][book].
We most warmly recommend **gtk-rs** users to have a look at this book.
While this book is targeted at GTK 4 developers, it also covers more general
aspects of GLib like **GObject Concepts**, **The Main Event Loop** or **GSettings**.

- **Online Book:** [GUI development with Rust and GTK 4][book]

[book]: /gtk4-rs/git/book
</div>

</div>
</section>
<section markdown="1">

## Sponsors

Thanks to everyone supporting us on [open collective][opencollective]! A list of all sponsors can be seen on our [open collective page][opencollective].


<div style="text-align: center">
    <div class="sponsor-tiers">
        <a href="https://opencollective.com/alistair">
            <div><img alt="Alistair" src="/images/alistair.png"></div>
            <div>Alistair</div>
            <div class="metal bronze">Bronze Sponsor</div>
        </a>
    </div>
    <div class="sponsor-tiers">
        <a href="https://www.embark-studios.com/">
            <div><img alt="Embark Studios" src="/images/embark.png"></div>
            <div>Embark Studios</div>
            <div class="metal gold">Gold Sponsor</div>
        </a>
    </div>
</div>

[opencollective]: https://opencollective.com/gtk-rs

## Projects using gtk-rs

<div class="projects-overview">
{% capture projects %}{% include projects.md %}{% endcapture %}
{{ projects | markdownify }}
</div>

If you want your app to be added to this list, please create a [Pull Request](https://github.com/gtk-rs/gtk-rs.github.io/edit/master/_includes/projects.md) for it.

</section>
