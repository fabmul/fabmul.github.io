---
layout: post
title: Personendaten über die lobid-API mit der GND abgleichen und anreichern

---

Das Hochschulbibliothekszentrum Nordrhein-Westfalen stellt im Rahmen seiner Linked Open Data-Dienste (lobid) auch eine Schnittstelle zur GND (lobid-gnd) zur Verfügung. Neben einer webbasierten Rechercheoberfläche und der Integration in OpenRefine wird auch eine allgemeine Web-API angeboten. Die Datenbasis bilden die RDF-Version der GND und die zusätzlich angereicherten EntityFacts. Serialisiert sind die bereitgestellten Daten in JSON-LD.

In diesem Artikel soll anhand eines einfachen Beispiels die GND über die API von lobid-gnd abgefragt werden. Als Input dient das folgende CSV:


{% highlight python %}
import requests
response = requests.get("https://api.open-notify.org/astros.json")
print(response.status_code)
{% endhighlight %}

Auch Museen stellen ihre Sammlungsdaten zunehmend über maschinenlesbare APIs zur Verfügung. In diesem Artikel soll anhand einfacher Beispiele die Funktionsweise und die Datenstruktur der API des Metropolitan Museum of Art sowie deren Abfrage in Python aufgezeigt werden.

*The Strange Case of Dr. Jekyll and Mr. Fabian* tells the story of a lawyer investigating the connection of two persons, Dr. Henry Jekyll and Mr. Edward Hyde. Chief among the novel's supporting cast is a man by the name of Mr. Poole, Dr. Jekyll's loyal butler.

-----

Poole is the butler for [Jekyll](http://jekyllrb.com), the static site generator. It's designed and developed by [@mdo](https://twitter.com/mdo) to provide a clear and concise foundational setup for any Jekyll site. It does so by furnishing a full vanilla Jekyll install with example layouts, pages, posts, and styles.

This demo site was last updated {{ site.time | date: "%B %d, %Y" }}.

There are currently two themes built on Poole:

* [Hyde](http://hyde.getpoole.com)
* [Lanyon](http://lanyon.getpoole.com)

Learn more and contribute on [GitHub]({{ site.github.repo }}).

## What's included

Poole is a streamlined Jekyll site designed and built as a foundation for building more meaningful themes. Poole, and every theme built on it like this one, includes the following:

* Complete Jekyll setup included (layouts, config, [404]({{ '404.html' | relative_url }}), [RSS feed]({{ 'atom.xml' | relative_url }}), posts, [archive page]({{ 'archive' | relative_url }}), and [example page]({{ 'about' | relative_url }}))
* Mobile friendly design and development
* Easily scalable text and component sizing with `rem` units in the CSS
* Support for a wide gamut of HTML elements
* Related posts (time-based, because Jekyll) below each post
* Syntax highlighting, courtesy Jekyll's built-in support for Rouge

Additional features are available in individual themes.

## Browser support

Poole and its themes are by preference a forward-thinking project. In addition to the latest versions of Chrome, Safari (mobile and desktop), Firefox, and Edge.

## Download

These themes are developed on and hosted with GitHub. Head to the [GitHub repository]({{ site.github.repo }}) for downloads, bug reports, and features requests.

Thanks!
