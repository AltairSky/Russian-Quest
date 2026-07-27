# Test post: everything the blog can render

This first paragraph is plain text. Below, every capability the site's markdown supports, one by one — plus a table at the end, which is **not** supported yet (it will render as plain text, so you can see what failure looks like too).

## Inline formatting (rich text)

Here is **bold text**, here is *italic text*, and here is Russian highlighted in the accent color: `ру́сский язы́к идёт хорошо́`. A normal [external link](https://en.wikipedia.org/wiki/Russian_language) opens in a new tab, and a command link like [open the game](#game) runs a site command instead.

Mixed in one sentence: **learn** the root `-уч-` *once*, then [read why](#main) it pays off.

## Headings

The line above this paragraph is a `##` heading. The site renders `#` and `##` identically inside a post (the very first `#` line of the file became the post title). There is no third level — a `### heading` is not parsed and will show as plain text with the hashes visible:

### this line demonstrates an unsupported heading level

## Lists

- first item, plain
- second item with **bold** and `ру́сское сло́во`
- third item with a [link](https://example.com)

## Divider

A `---` line renders as the dashed rule below:

---

## Picture

![This is the caption under an image — it renders in the dim color with a # prefix](https://picsum.photos/seed/test/720/400)

## Self-hosted video

![An .mp4 file gets a native player with controls](https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4)

## YouTube embed

![A YouTube link becomes an embedded player](https://youtu.be/jNQXAC9IVRw)

## Button link

A link whose text starts with ./ renders as a button:

[./press-me](https://example.com)

## Table — NOT supported (yet)

The markdown table below will NOT render as a table; the site's renderer doesn't parse pipe syntax, so it comes out as raw text lines:

| prefix | meaning | example |
|--------|---------|---------|
| в- | in | войти́ |
| вы- | out | вы́йти |

If tables turn out to be needed for your grammar materials, ask Claude to add table support to the renderer.

## Edge cases

A paragraph with an asterisk that should *not* break: 2 * 2 = 4 works because italics need no spaces around the marked text. Stress marks in plain text: за́мок, замо́к, вы́учить — check these render cleanly on your phone.

The end. If everything above looks right except the table and the ### heading, the renderer is working exactly as designed.
