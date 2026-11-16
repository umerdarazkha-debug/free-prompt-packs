# Turn your handwriting into a working font (Claude Code)

From Umer does AI. Want the finished tool instead of building your own? It's here: [handwriting-to-font](https://github.com/umerdarazkha-debug/handwriting-to-font).

This needs Claude Code, Claude's coding agent, because it runs Python on your computer. The regular Claude chat can't do it.

## Step 1: paste this prompt into Claude Code

```
Build me a tool that turns my handwriting into a font I can install.

1. Make a printable A4 template: one box per character (A-Z, a-z, 0-9 and
   common punctuation), a baseline and a cap-height line in each box, and a
   solid black square in each corner so a phone photo can be straightened.
2. Write a script that takes my phone photo of the filled sheet, finds the four
   corner squares, flattens the page, evens out the lighting, cuts out each box,
   traces the ink into smooth vector outlines and saves a real .otf font
   (use Python with opencv, potracer and fontTools).
3. Before giving me the font, show me my 5 worst letters first: the ones that
   run out of the box, break into pieces, sit off the baseline or don't match
   the height of the others. Show each one cropped from my photo with the reason.
4. Then render "The quick brown fox jumps over the lazy dog" in the new font
   so I can see it working.

Test the whole thing yourself on a fake filled sheet before you hand it over.
Don't invent letters I didn't write: leave a glyph empty and tell me instead.
```

## Step 2: fill the sheet
- Print the template. Use a black pen or marker, not blue and not pencil.
- One character per box. Letters sit on the baseline, and capitals touch the top line.
- Take the photo flat from above in daylight, with all four black squares in frame.

## Step 3: the "5 worst letters first" trick
Don't rewrite the whole sheet. Ask Claude for your 5 worst letters, rewrite only those boxes on a new sheet, and ask it to swap them in. Two rounds is usually enough.

## Install
Double-click the `.otf` file, then click Install (Mac Font Book or Windows). After that it shows up in Figma, Word and Keynote, and you can upload it to Canva on Canva Pro.
