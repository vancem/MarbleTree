---
description: "If you have exactly 1’ x 2’ x 1/8” plywood, you will not need to modify the design at all and you can skip this step"
---

# Modifying the Laser Cutter Design File

If you have exactly 1’ x 2’ x 1/8” plywood, you will not need to modify the
design at all and you can skip this step. However it is reasonably likely that
you may need to scale or rearrange the pieces to fit the material you have. You
may also make mistakes when cutting, and need to re-cut just a few of the
pieces. You may also wish to personalize the tree by adding text that will be
rasterized onto the base or the leaves. For all these cases, you will want to
modify the SVG files that represent the design.

SVG stands for Scalable Vector Graphics file, and is a straightforward XML
(text) file that describes lines, circles, splines and text in a way that can
scaled to any size without losing resolution (unlike bitmap technologies). SVG
files can be read by web browsers directly (it is an internet standard), and
just about any CAD program should have the ability to read SVG files.

There is a program called [InkScape](https://inkscape.org/en/download/) that can
be downloaded from the web (see [https://inkscape.org](https://inkscape.org))
that directly edits SVG files (SVG is its native file format, but it also can
read or write out in other formats including PDF, etc). Simply download and
launch Inkscape and ask it to open one any of the SVG files to edit it. The
program has good help/tutorial documentation, but here is a quick cheat sheet to
get you going quickly.

- There is a toolbar on the left side. By default it is on the ‘arrow’ icon,
  which is the ‘select’ which is a good default, and for simple adjustments you
  may never need anything else. In this mode if you click on an object, it
  selects it, once selected you can move it (there are also resize handles)
- Ctrl-Z – undo (You will be very happy to know this when you accidentally type
  something)
- + zoom in
- - zoom out
- Ctrl-A - selects all objects (useful for centering the design on the sheet).
- Alt-O – Opens the object menu. Use things include rotating, flipping
  horizontally or vertically, and Transforming (used to scale thickness).
- Shift- Ctrl – F – Fill and Stroke. This opens a tabbed pane, and one of these
  tabs is the ‘stroke style’ of the lines. One of the attributes you can set is
  the line thickness. This is important because the lines need to be thin (less
  than 1 pixel) for the cutter to recognize it as a cut. Thus you may wish to
  select all objects (Ctrl-A) and set their line thickeness to .001” This
  insures that lines are thin enough to be interpreted as cuts.
- Shift-Ctrl-G Ungroup object – I have grouped many of the pieces so that you
  can move them easily as a group. However you may need to break up the groups
  for it to fit in a particular space.
- Ctrl-G – Group objects – It is a good idea to group the objects back again
  after you have finished whatever edit required you to ungroup them.

## Orienting the leaves.

If you fiddle with the leaves (for example you may have broken a leave and need
to print a single new one), there is one ‘gotcha’ I want you to alert you to.
Plywood has different stiffness depending on the direction of the grain. What
this means is that it is important that all the leaves of any marble tree are
all oriented in the same direction with respect to the grain of the wood. Thus
don’t cut one leaf across the grain and one with the grain. If you do this they
will ‘ring’ differently and instead of getting a pleasant descending scale you
get a discordant set of notes.


## Compensating for thickness

The SVG file is designed for 1/8” plywood. However the design does scale, and
thus if you simply scaled the entire design by 2, you could make it out of ¼”
plywood. Conversely, most plastic is slightly less than 1/8” closer to 1/10”, so
you would want to scale the design so that it works for that thickness. This is
very easy to do in Inkscape. Before you do this you have to calculate the %
scaling that you will need. To do this:

- Measure the thickness of your material. Ideally you do this with a dial or
  Vernier caliper that allows you to very accurately measure small distances. If
  you don’t have this you can use the ‘speced’ thickness. For example some
  plywood say it is 2.6 mm = .102” thick.
- Calculate the scale percentage as (TrueThickness/.125”) * 100 . Thus the case
  of 2.6mm, it would be (.102”/.125”)* 100 = 81.6 %
- Note that because wood naturally varies a bit, you don't want to be too
  precise. You want a little bit of 'wiggle room' so that the leaves don't bind.
  Thus once you have calculated the % above you will want to make it about 3%
  larger than calculated so that you have this extra space. 3% is enough for
  this but won't cause 'wobble'.

Once you have this number you can scale your design by doing

- select everything (Ctrl-A)
- From the Object Menu select the Transform menu item. This will bring up a
  ‘transform’ pane on the right hand side of the screen.
- Select the ‘scale’ tab.
- Check the ‘scale proportionally’ checkbox.
- Enter a % scale factor calculated above (e.g. 81.6)
- Click the Apply button.

If you don’t have a dial caliper you can also do this by trial and error by only
printing one of the trunk shingles and seeing if the material slides nicely into
the slot. If it is too big scale it by 95%. If it is too small scale it by 105%.
Keep making adjustments until you don’t’ have to force the material into the
slot (too small) and it does not wobble (too big).

Even if you do have a dial caliper, I would recommend printing a test to confirm
that it is perfect before committing to the 20 min or to print the pieces.
