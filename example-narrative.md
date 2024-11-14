# Example Narrative <!--{ as="video" mode="hero" src="https://dlmultimedia.esa.int/download/public/videos/2023/06/010/2306_010_AR_EN.mp4" }-->

#### An introduction on how to write interactive and multimedial stories using markdown. Scroll down to get started! <!--{ style="font-size:1rem;opacity:0.7;margin-top:1rem;" }-->

## Why storytelling?

Storytelling is crucial in the realm of science because scientific data, while rich in information, can often be complex and challenging to communicate. By framing data within narratives, storytelling makes scientific concepts accessible, engaging, and memorable to a wider audience. It bridges the gap between the technical details of research and the public's understanding, fostering appreciation, curiosity, and ultimately, a deeper connection to the wonders of science.

## How do I get started?

### Markdown with superpowers

The main story language is Markdown, a lightweight markup language that uses plain text formatting syntax to convert plain text into structured HTML documents. Read more about Markdown [in this Wikipedia article](https://en.wikipedia.org/wiki/Markdown) and find a guide on how to get started (including a cheatsheet) [here](https://www.markdownguide.org/).

Addtiionally to normal Markdown, the storytelling rendering engine allows adding additional configuration; this configuration is only visible to you, the editor, and is hidden to the reader.
It allows adding "superpowers" to Markdown using [HTML](https://en.wikipedia.org/wiki/HTML) comments and attributes.

To write a HTML comment, use the following syntax:

```html
<!--{ *custom HTML attributes* }-->
```

---

Let's say we want a small image with a specific size and a colored text underneath. With normal Markdown you would write something like this:

**Input**:

```md
![Image](https://placehold.co/800x100)

_Some italic text_
```

**Output**:

![Image](https://placehold.co/800x100)

_Some italic text_

---

Let's add some configuration to reduce the width of the image and add color to the text:

**Input:**
```
![Image](https://placehold.co/800x100) <!--{ width="300" }-->

_Some italic text, now in red_ <!--{ style="color:red" }-->
```

**Output**:

![Image](https://placehold.co/800x100) <!--{ width="300" }-->

_Some italic text, now in red_ <!--{ style="color:red" }-->

---

You can use any HTML attributes, plus some shorthands: `#` is a shorthand for `id` (e.g. `#hello` renders as `id="hello"`) and `.` is a shorthand for `class` (e.g. `.foo` renders as `class="foo"`).

## Story structure

### The hero

The hero is the initial section of a story. It can be either a full-screen image or a full-screen video, with some overlaying text. You can either write the hero section by hand, or by using the "plus" icon in the editor toolbar (or in the story preview).
In each story, only one hero should be added at the very beginning. After the hero, you will see the nav menu, and after that, the story content. The hero uses the Markdown syntax for `h1` (Header 1), so it starts with one `#`.

### Story sections

To start a new section, use the Markdown syntax for `h2` (Header 2), so starting with `##`. Eeach section is automatically added to the nav menu.

### Special sections

Additionally to the hero section, there are other special sections (like media, map), and the most convenient way to add them is via the "plus" icon. They use the "as" attribute, which replaces the entire section with the corresponding element. So, for example, `as="div"` will replace the entire section (including the title) with a `div`.
We will now have a more in-depth look about the map section. The map section shows a single map, with optional text underneath. It is powered by [EOxMap](https://eox-a.github.io/EOxElements/?path=/docs/elements-eox-map--docs), so you can use the same syntax as with any EOxMap.

**Input:**

```
## Map section <!--{as="eox-map" style="width: 100%; height: 500px;" [...]
```

To see the full input of this and the following section, check the Markdown file directly.

**Output:**:
## Map section <!--{as="eox-map" style="width: 100%; height: 500px;" config='{ "controls": { "Zoom": {}, "Attribution": {}, "FullScreen": {}, "OverviewMap": { "layers": [ { "type": "Tile", "properties": { "id": "overviewMap" }, "source": { "type": "OSM" } } ] } }, "layers": [ { "type": "Tile", "properties": { "id": "overviewMap" }, "source": { "type": "TileWMS", "url": "https://ows.mundialis.de/services/service", "params": { "LAYERS": "TOPO-WMS" } } } ], "view": { "center": [15,48], "zoom": 1 } }'}-->

## Map Tour section <!--{ as="eox-map" mode="tour" }-->

### <!--{ layers='[{"type":"Tile","properties":{"id":"osm"},"source":{"type":"OSM"}}]' center=[12.46,41.89] zoom="5" animationOptions="{duration:500}" }-->

#### This is a map tour.

It allows you to have different layers, zoom and center settings for each tour "step".

### <!--{ layers='[{"type":"Tile","properties":{"id":"customId"},"source":{"type":"WMTSCapabilities","url":"https://tiles.maps.eox.at/wmts/1.0.0/WMTSCapabilities.xml","layer":"s2cloudless-2017"}},{"type":"Tile","properties":{"id":"osm"},"source":{"type":"OSM"}}]' center=[12.46,41.89] zoom="10" }-->

#### Second tour step.

Each tour step is described as an `h3` (`###`) heading.

### <!--{ layers='[{"type":"Tile","properties":{"id":"customId"},"source":{"type":"WMTSCapabilities","url":"https://tiles.maps.eox.at/wmts/1.0.0/WMTSCapabilities.xml","layer":"s2cloudless-2017"}},{"type":"Tile","properties":{"id":"osm"},"source":{"type":"OSM"}}]' center="[16.36,48.2]" zoom="10" animationOptions="{duration:500}" }-->

#### Third tour step.

To change individual parameters like zoom or center, or to change the map layers for a step, just set them using the HTML comment syntax. This changes the map setting for the current map

## Final Words

Hopefully, this was a good introduction to the story writing possibilities using EOxStorytelling - get started writing your own story!
More features will be added soon, so feel free to follow progress at the [EOxElements GitHub repository](https://github.com/EOX-A/EOxElements).
