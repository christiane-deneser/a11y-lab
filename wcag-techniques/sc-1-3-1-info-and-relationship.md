# SC 1.3.1 Info and Relationships – Messy Notes

* a) HTML structural elements for headings
* b) HTML structural elements for lists
* c) HTML structural elements for quotations
* d) Content structured logically
* e) Data tables structured correctly
* f) Association of table cells (complex tables)
* g) No structural markup for layout tables
* h) Programmatic labeling of form controls

## a) HTML structural elements for headings
## Überschriften mit HTML-Strukturelementen `h1` bis `h6`

* Dokumenten-Heading-Struktur
* Screenreader-Navigation per Headings
* die Gesamtstruktur der Seite sauber bleiben

### Examples (with ARIA)
....

---

## b) HTML structural elements for lists

### Examples (with ARIA)
...

---

## c) HTML structural elements for quotations

### <blockquote>: The Block Quotation element

* The `<blockquote>` HTML element indicates that the enclosed text is an extended quotation. Usually, this is rendered visually by indentation (see Notes for how to change it). A URL for the source of the quotation may be given using the `cite` attribute, while a text representation of the source can be given using the `<cite>` element.

```
<div>
  <blockquote cite="https://www.huxley.net/bnw/four.html">
    <p>
      Words can be like X-rays, if you use them properly—they’ll go through
      anything. You read and you’re pierced.
    </p>
  </blockquote>
  <p>—Aldous Huxley, <cite>Brave New World</cite></p>
</div>
```
```
<blockquote cite="https://datatracker.ietf.org/doc/html/rfc1149">
  <p>
    Avian carriers can provide high delay, low throughput, and low altitude
    service. The connection topology is limited to a single point-to-point path
    for each carrier, used with standard carriers, but many carriers can be used
    without significant interference with each other, outside early spring. This
    is because of the 3D ether space available to the carriers, in contrast to
    the 1D ether used by IEEE802.3. The carriers have an intrinsic collision
    avoidance system, which increases availability.
  </p>
</blockquote>
```

### `<cite>`: The Citation element

* The `<cite>` HTML element is used to mark up the **title of a creative work**.
* The reference may be in an abbreviated form according to context-appropriate conventions related to citation metadata.
* Typically, browsers style the contents of a `<cite>` element in italics by default. To avoid this, apply the CSS font-style property to the `<cite>` element.
* In the context of the <cite> element, a creative work could be, for example, one of the following:
  * 'book, research paper, essay, poem, musical score, song, play or film script, film, television show, game, sculpture, painting, theatrical production, play, opera, musical, exhibition, legal case report, computer program, website, web page, blog post or comment, forum post or comment, tweet, facebook post, written or oral statement'

```
<figure>
  <blockquote>
    <p>
      It was a bright cold day in April, and the clocks were striking thirteen.
    </p>
  </blockquote>
  <figcaption>
    First sentence in
    <cite>
      <a href="http://www.george-orwell.org/1984/0.html">
        Nineteen Eighty-Four
      </a>
    </cite>
    by George Orwell (Part 1, Chapter 1).
  </figcaption>
</figure>
```

---

## d) Content structured logically

### Examples (with ARIA)
...

### `<p>`: The Paragraph element

* The `<p>` HTML element represents a paragraph. Paragraphs are usually represented in visual media as blocks of text separated from adjacent blocks
* but HTML paragraphs can be **any structural grouping of related content, such as images or form fields**

```
<p>
  Geckos are a group of usually small, usually nocturnal lizards. They are found
  on every continent except Antarctica.
</p>

<p>
  Some species live in houses where they hunt insects attracted by artificial
  light.
</p>
```

### `strong` – Strong importance for its contents

* The `<strong>` HTML element indicates that its contents have strong importance, seriousness, or urgency. Browsers typically render the contents in bold type.
* Another accepted use for `<strong>` is to denote the labels of paragraphs which represent notes or warnings within the text of a page.
* Both `<strong>` and `<em>` can be nested to increase the relative degree of importance or stress emphasis, respectively.

```
<p>
  ... the most important rule, the rule you can never forget, no matter how much
  he cries, no matter how much he begs:
  <strong>never feed him after midnight</strong>.
</p>
```

```
<p>
  <strong>Important:</strong> Before proceeding, make sure you add plenty of
  butter.
</p>
```

### `<em>` – The Emphasis element

* The `<em>` HTML element marks text that has stress emphasis. The <em> element can be nested, with each level of nesting indicating a greater degree of emphasis.
* The `<em>` element is for words that have a stressed emphasis compared to surrounding text, which is often limited to a word or words of a sentence and affects the meaning of the sentence itself.

```
<p>Get out of bed <em>now</em>!</p>

<p>We <em>had</em> to do something about it.</p>

<p>This is <em>not</em> a drill!</p>
```

```
<p>
  Ice cream is made with milk, sweetener, and cream. Frozen custard, on the
  other hand, is made of milk, cream, sweetener, and <em>egg yolks</em>.
</p>
```

**but:**

```
<p>The word <i>the</i> is an article.</p>
<p>The <i>Queen Mary</i> sailed last night.</p>
```

### <br> The Line Break element

* The `<br>` HTML element produces a line break in text (carriage-return). It is useful for writing a poem or an address, where the division of lines is significant.
* Note: Do not use `<br>` to create margins between paragraphs; wrap them in `<p>` elements and use the CSS margin property to control their size.
* The `<br>` element has a single, well-defined purpose — to create a line break in a block of text. As such, it has no dimensions or visual output of its own, and there is very little you can do to style it.
* Accessibility: Creating separate paragraphs of text using <br> is not only bad practice, it is problematic for people who navigate with the aid of screen reading technology. Screen readers may announce the presence of the element, but not any content contained within <br>s. This can be a confusing and frustrating experience for the person using the screen reader.

```
<p>
  O’er all the hilltops<br />
  Is quiet now,<br />
  In all the treetops<br />
  Hearest thou<br />
  Hardly a breath;<br />
  The birds are asleep in the trees:<br />
  Wait, soon like these<br />
  Thou too shalt rest.
</p>
```
```
Mozilla<br />
331 E. Evelyn Avenue<br />
Mountain View, CA<br />
94041<br />
USA<br />
```

---

## 



