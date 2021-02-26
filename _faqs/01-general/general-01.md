---
question: "What are the possible environments / workflows for using Verovio?"
---

Verovio is a C++ codebase that can be compiled and wrapped into different programming languages and integrated into various environments.

#### Workflow

The [Command-line interface](command-line.xhtml) or the [Python toolkit](python.xhtml) can be used in scripting environments or server side. Typical use cases would be :

* generate SVG and MIDI from MEI documents or other supported formats,
* generate MEI documents from other supported formats (e.g., convert files).

Resulting SVG or MEI documents can then be embedded in a HTML page or used as such.

![]({{ site.baseurl }}/images/overview_server.png)<br>

The [JavaScript toolkit](javascript.xhtml) makes it possible to generate SVG and MIDI directly in the browser. It is easy to set up and platform independent. Interaction with the user can then be handled with basic JavaScript or CSS. [An example of how to handle events](tutorial.xhtml?id=topic02) is given in the tutorial. It is also possible to process the MEI via XSLT in the browser before loading it into Verovio.

![]({{ site.baseurl }}/images/overview_client.png)<br>

Both approaches can be combined: one may choose to process the MEI and to generate the SVG server side for better performance, and then handle interactions client side with JavaScript and CSS.
![]({{ site.baseurl }}/images/overview_hybrid.png)<br>

##### Font limitation

Firefox on Linux (Ubuntu), uses "DejaVu Serif" as default font, which can cause some text layout problems when displaying the SVG files generated with Verovio.