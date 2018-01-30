# Lessons Learned

## Hardware

RGB bulbs (I've tried Hue and LIFX) don't provide a nice, pleasant natural white light for working under.  They're better as accent lights, or nightlights if you want a dim red color.

Ikea Tradfri white spectrum bulbs provide a nice range of warm and cool whites, great for working under during the day.  But they don't dim enough to be used as a nightlight.

## Software

yaml looks deceptively easy, but the way it uses whitespace makes it infuriating.  I've spent hours twiddling with whitespace in config files to get yaml to parse them.  What it will and will not accept often seems completely arbitrary, but I'm making sure I only check in working config files to this repo so they should serve as good examples.  Note to self: if you ever design a programming language -- parentheses, braces, and brackets are a good idea.

# Configuration

## Front End

For group and customization files, a tab is called a `view`.  So:

```yaml
view: yes
```

effectively means, "make this a tab".

If you want something to be a card on the main page, add it as an entity to the `default_view`.  But note:  if you use `default_view`, any entity not listed there will not show up on the main page at all.

