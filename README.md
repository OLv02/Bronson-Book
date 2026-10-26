# Bronson Book

**Backing guitar**: a practice page for 44 tunes from the Bronson Fiddle Songbook. It plays a guitar backing, and a fiddle melody for 34 of the tunes, while a fretboard shows exactly which shape to hold and which strings to hit on every beat.

**Live page:** https://olv02.github.io/Bronson-Book/

Or open `index.html` in any browser, on a phone or a computer. There's no build step. Below the play-along, a songbook panel shows each tune's sheet music, Nashville numbers, recordings and melody notation with guitar TAB.

- `index.html`: the page, including all song data.
- `sheets/`: sheet music images from the songbook, plus the circle of fifths chart.
- `vendor/abcjs-basic-6.6.4.min.js`: [abcjs](https://abcjs.net) (MIT license), which draws the melody notation. It loads only when you open Learn melody.

Keep these together: the page loads the images and abcjs from those folders.

See [docs/backing-guitar.md](docs/backing-guitar.md) for the full guide: the panels, how playback works, where the chords and melodies come from, song-by-song coverage, limitations, and a practice quick start.
