I would recommend running through the workshop as a
participant before facilitating. At the very least,
scan though [the participant readme](readme-participant.md).

## Presentation

The slides are html/js built using reveal.js. To view the slides, navigate to presentation/xss.html.

For presentation mode and speaker notes: press `s` after opening. Will open in a seperate browser window

Use right and left arrow keys to navigate forward and backwards

`esc` will bring up a side overview

## Hands on sections

Hands on sections increase participation but add a lot of extra time. In order
to speed things up, you can choose to demonstrate the exploit in front of
everyone rather than having everyone exploit the vulnerability themselves.

To do this, have the demo application running before you start presenting,
and when you get to slide #7, switch away from the presentation, open up
`http://localhost:8081`, and demonstrate the exploit. One strategy to keep
people involved when doing this is having the participants make suggestions
about what you should type.

## Print / Export PDF

1. Open the presentation/xss.html file in your browser with the `print-pdf` query parameter
2. For example: `file:///path/to/xss-presentation/presentation/src/main/resources/static/xss.html?print-pdf`
3. Open the print dialog and either select a printer or export to PDF
