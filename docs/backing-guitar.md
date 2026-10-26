# Backing Guitar: What It Is and How It Works

Oct 25, 2026 · @Owen

## Overview

Backing guitar is a practice page for 44 tunes from the Bronson Fiddle Songbook. It plays a guitar backing, and a fiddle melody for 34 of the tunes, while a fretboard shows exactly which shape to hold and which strings to hit on every beat.

It's built for a guitarist learning to back up a fiddle session. You can pick a tune, watch the chord changes come up in time, and play along at any tempo. Everything in it comes from the songbook file itself:

- **Chords:** read from the sheet music's chord symbols or from your written chord charts.
- **Capo positions:** from your "easiest way" notes.
- **Melodies:** from the notation stored in the songbook's Learn Melody sections.
- **Reference links:** to each tune's recording and sheet source.

It runs as a web page in any browser, on a phone or a computer, at https://olv02.github.io/Bronson-Book/. The backing and melody are generated in the browser, so there are no audio files to download. The sheet music images sit in the `sheets/` folder next to the page.

## What you see on the page

The page is one column with four panels, top to bottom, like a music stand.

### 1. Song panel

- A song picker grouped by tune type, with previous and next buttons. The groups are reels, jigs, hornpipes, polkas, marches, waltzes, breakdowns, and songs and jams.
- Tags for key, tune type, time signature and capo position. Other tags mark songs that have a melody and songs whose chords or timing are estimated or suggested.
- Links to the reference recording or video and the sheet music source, from your songbook.
- A short note when something about the song needs explaining, such as a key change or a chart that was adjusted to match the melody.

### 2. Fretboard panel

- The current chord in large type, with the next chord shown beside it.
- A fretboard diagram of the current shape (details in [The fretboard](#the-fretboard) below).
- A button for every chord shape the song uses. Tap one to see it and hear it strummed.
- Beat boxes for the strum pattern, such as "1 bass, 2 strum, 3 bass, 4 strum", which light up in time.
- Toggles for player's view and alternating bass, plus a color legend.

### 3. Play-along panel

- Play/Stop button and a status line showing the part and bar, or the count-in.
- Sliders for tempo, melody volume and guitar volume.
- Toggles for count-in bar, metronome click and loop.
- The form, such as A A B B, with the part now playing highlighted.
- The chord chart: one grid per part, one box per bar. The current bar lights up, and tapping a bar starts playback from there.
- A collapsible copy of your original chord chart text from the songbook.

The page follows your device's light or dark mode, and fits a phone screen without sideways scrolling.

### 4. From your songbook panel

Everything else the songbook holds for the tune, so you don't need the songbook open alongside:

- **Sheet music:** every sheet image saved for the tune, with its caption, such as "Page 1 of 4" or "Simple harmony". Tap an image to open it full size. Tunes with no saved image link to their sheet source instead.
- **Nashville numbers:** the tune's Nashville Number System line, with the songbook's note on how to read it.
- **Recordings:** a player for each saved recording, with 0.5×, 0.75× and 1× speed buttons. Father Kelly's has Melody 90, Harmony 90 and Slow 64 versions, and Reel de Montréal has Main and Slow. Tunes with a YouTube reference embed the video, and tunes with no direct audio file link to their source with the songbook's note about why. Starting the play-along pauses any recording.
- **Learn melody:** for the 33 tunes with stored notation, a collapsible section that draws the melody as notation with guitar TAB. Tap a note to see its letter name. It also has the songbook's practice note and a warm-up scale in the tune's key.
- **Tags:** the songbook's tags for the tune, such as "New tunes — October 2026".

A Circle of fifths reference sits at the bottom of the page.

## How playback works

Press Play and the page plays the whole tune in its written form, such as AABB. The guitar plays a boom-chick vamp: a single bass note, then a strum on the higher strings. The rhythm of the vamp depends on the tune type.

| Tune type | Time | Pattern per bar | Tempo counted in |
|---|---|---|---|
| Reels, hornpipes, breakdowns, marches, songs | 4/4 | bass, strum, bass, strum | quarter notes |
| Jigs | 6/8 | bass on 1, strum on 3, bass on 4, strum on 6 | dotted quarters |
| Polkas | 2/4 | bass, strum, bass, strum on eighth notes | quarter notes |
| Waltzes | 3/4 | bass, strum, strum | quarter notes |

- **Alternating bass:** with the toggle on, the second bass note of the bar moves to a different string, such as the open 5th string under a D chord. In waltzes it alternates bar by bar.
- **Chord changes mid-bar:** when a bar has two or more chords, they split the bar evenly. If a change lands on a strum, the new chord's bass note plays there instead, so you always hear its root.
- **Melody:** for 34 tunes a fiddle-style melody plays on top at the written fiddle pitch, with its own volume slider. Turn it to 0 to practice over the backing alone.
- **Count-in:** one bar of clicks before the tune starts. Pickup notes come in at the end of the count-in, the way the tune is written.
- **Metronome click:** an optional click on every beat, with an accent on beat 1.
- **Tempo:** each tune starts at a learning-friendly default of 80 to 120 bpm. You can move the slider from 40 to 220 bpm while it plays, and the music speeds up or slows down smoothly without restarting.
- **Start from any bar:** tap a bar in the chord chart to start there, with a count-in, so you can drill one tricky change.
- **Loop:** plays the tune over and over, carrying the pickup notes into each new time through.
- **Previewing a chord:** tap a chord button while stopped to hear one bass note and one strum.

On a computer, the space bar starts and stops playback.

## The fretboard

The fretboard shows frets 1 to 5 in standard tuning, with every shape drawn as you'd finger it and the strings for each beat marked by color.

- **Bass note:** a filled orange dot, with its string drawn in orange.
- **Alternate bass:** an orange ring, with its string dashed. It shows only when alternating bass is on.
- **Strummed strings:** green. Fretted notes show which finger to use (1 = index, 4 = pinky).
- **Unplayed strings:** marked ×. Open strings that aren't part of the pattern get a plain ring.
- **On the beat:** the string being played thickens, so you can see the bass and strum alternate.

**Player's view.** By default the high e string is on top, like a chord chart. Turn on player's view to put the low E on top, matching what you see looking down at your guitar. The page remembers this setting.

**Capo.** When a song uses a capo, the nut bar turns green and a label reads "Shapes shown relative to capo 2" (or whichever fret). Fret numbers count from the capo, so you read the shapes as you know them. The audio is transposed up by the capo amount, so it sounds at the real pitch and matches recordings and fiddlers.

**Shapes used across the songbook:** G, G7, C, D, D7, Dm, A, A7, A5, Am, Am7, E, E7, Em, B7 and B5. All are open shapes, except the A5 and B5 power chords.

## Where the chords and melodies come from

Every chord and note on the page traces back to the songbook file. The rules below decide which source wins for each song.

1. **Melody notation, when a tune has it.** 33 tunes have melody notation stored behind their Learn Melody panels. That notation sets the tune's structure: its parts, repeats, endings, pickup and key. The chord chart is fitted to it, so every one of the 33 lines up bar for bar. Where the notation file has its own chord symbols, those can be used too.
2. **Chord symbols on the sheet music.** Where the sheet image prints chords above the staff, they're read bar by bar and translated into your capo shapes. Slash chords become the plain chord (G/B plays as G), following your cheater rules.
3. **Your written chord chart.** When the sheet has no chord symbols, your own chart is used. If it lists fewer entries than the tune has bars, each entry is spread over 2 bars.
4. **Suggested chords.** For the few tunes with no chords anywhere in the file, the chords are a suggestion based on the melody line, and the song is tagged so you know to check them by ear.

Bonnie Kate has no stored notation. Its melody was worked out from your sheet image when the first Bonnie Kate player was built. It's a traditional tune.

## What the tags on a song mean

| Tag | Meaning |
|---|---|
| Melody included | A fiddle melody plays along, taken from the songbook's notation. |
| Timing estimated | No chords on the sheet or no sheet at all, so your chart was spread across the bars. The chords are yours, but where each change falls is a best guess. |
| Suggested chords | The songbook has no chords for this tune, so these are a starting point. |
| Chart borrowed from #2 | Mason's Apron (The Session #74) has no chords of its own, so it uses #2's chart. |

A song's note also flags anything specific. Examples include a key change (Reel de Montréal into Sherbrooke), a different setting from your sheet (Rubber Dolly, Orange Blossom Special), or a chord that differs from your chart. In the Tennessee Waltz bridge, for instance, the B7 shape replaces your chart's F#5 because B7 matches the sheet with capo 7.

## Song-by-song coverage

All 46 of the songbook's entries are on the page. 44 have a backing, and 34 of them play a melody. The two bossa nova songs are listed under "Songbook only (no backing)" and show just their songbook panel. In the Form column, letters and numbers name the parts in playing order. Songs with special part names, like Redwing's verse and chorus, use labels like V1, V2 and C.

| # | Tune | Type | Key | Capo | Melody | Chords from | Form |
|---|---|---|---|---|---|---|---|
| 2 | The Mason's Apron | Reel | A Major | 2 | Yes | Sheet chord symbols | 1 1 2 2 3 3 4 4 5 5 |
| 3 | The Irish Washerwoman | Jig | G Major | — | Yes | Sheet chord symbols | A A B B |
| 4 | Redwing | Reel | G Major | — | Yes | Sheet chord symbols | V1 V2 C C |
| 5 | The Tennessee Waltz | Waltz | D Major | 7 | Yes | Sheet chord symbols | A B |
| 6 | Swallowtail Jig | Jig | E Dorian | — | Yes | Sheet chord symbols | A A B B |
| 7 | Saint Anne's Reel | Reel | D Major | — | Yes | Sheet chord symbols | A A B B |
| 8 | The Maid Behind The Bar | Reel | D Major | 7 | Yes | Your chart, timing estimated | A A B B |
| 9 | Ashokan Farewell | Waltz | D Major | — | Yes | Your chart | A A B B |
| 10 | Mason's Apron (The Session #74) | Reel | A Major | 2 | Yes | Chart from #2 | 1 1 2 2 3 3 4 4 5 5 |
| 11 | The Silver Spear | Reel | D Major | 7 | Yes | Your chart, timing estimated | A A B B |
| 12 | The Devil's Dream | Reel | A Major | 2 | Yes | Sheet and melody file | A A B B C C |
| 13 | Father Kelly's | Reel | G Major | — | Yes | Sheet chord symbols | A A B B |
| 14 | Reel de Montréal / Reel de Sherbrooke | Reel | G Major to D Major | 7 | Yes | Sheet chord symbols | A A B B |
| 15 | The Road to Errogie | Reel | G Major | — | Yes | Your chart | A A B |
| 16 | Rannie MacLellan | Reel | D Major | 7 | Yes | Your chart | A A B B |
| 17 | Maple Sugar | March | A Major | 2 | Yes | Sheet chord symbols | A A B B A A C C |
| 18 | Bert Ferguson | Jig | A Major | 2 | Yes | Your chart, timing estimated | A A B B |
| 19 | Big John McNeil | Reel | A Major | 2 | Yes | Your chart | A A B B |
| 20 | Shady Nook | Jig | G Major | — | Yes | Your chart | A A B B |
| 21 | Irishman’s Heart to the Ladies | Jig | A Major | 2 | Yes | Your chart | A A B B |
| 22 | Memories of Father Angus MacDonnell | March | G Major | — | Yes | Sheet chord symbols | A A B B |
| 23 | The Frost Is All Over / Done | Jig | D Major | — | Yes | Sheet chord symbols | A A B B |
| 24 | Rubber Dolly (Back Up and Push) | Breakdown | F Major | 5 | Yes | Fitted to melody file | A1 A2 B1 B2 |
| 25 | The Ale Is Dear | Reel | B Minor | 2 | Yes | Sheet chord symbols | A A B |
| 26 | Cock of the North | Jig | D Major | 7 | Yes | Sheet chord symbols | A A B B |
| 27 | The High Road to Linton | Reel | A Major | 2 | Yes | Suggested | 1 1 2 2 |
| 28 | I’ll Tell Me Ma | Polka | G Major | — | Yes | Your chart and melody file | A B |
| 29 | John Ryan’s Polka | Polka | D Major | 7 | Yes | Your chart | A B |
| 30 | My Cape Breton Home | Waltz | G Major | — | Yes | Your chart | A B A B |
| 31 | Orange Blossom Special | Breakdown | E Major | 2 | Yes | Fitted to melody file | A1 A2 |
| 32 | The Rakes of Kildare | Jig | A Minor | — | Yes | Your chart | A A B B |
| 33 | The Soldier’s Joy | Reel | D Major | 7 | Yes | Sheet chord symbols | A A B B |
| 34 | The Wind That Shakes the Barley | Reel | D Major | 7 | Yes | Melody file chord symbols | A A B B |
| 35 | St. Anne's Reel (Hayes Griffith Guitar Arrangement) | Reel | D Major | — | No | Sheet chord symbols | A A B B |
| 36 | Country Bluegrass Jam in G | Jam | G Major | — | No | Sheet chord symbols | A A |
| 38 | Kettle Valley Line | Song | A Minor | 3 | No | Sheet (verse), suggested (bridge) | A A B A |
| 40 | Growling Old Man and Grumbling Old Woman | Reel | A Dorian / A Mixolydian | — | No | Sheet chord symbols | A A B B |
| 41 | The Tarbolton | Reel | E Dorian | — | No | Sheet chord symbols | A A B B |
| 42 | Rambler’s Hornpipe / Old French | Hornpipe | D Major | — | No | Suggested | A A B B |
| 43 | Fisher’s Hornpipe | Hornpipe | D Major | — | No | Sheet chord symbols | A A B B |
| 44 | Fiddler’s Despair | Reel | E Minor | — | No | Suggested | A A B B |
| 45 | Reel Béatrice | Reel | A Minor | — | No | Sheet chord symbols | A A B B C |
| 46 | Spootiskerry | Reel | G Major | — | No | Sheet chord symbols | A A B |
| 47 | Bonnie Kate | Reel | D Major | — | Yes | Sheet chord symbols | A A B B |
| 37 | Água de Beber | Bossa nova | A Minor | — | No | Songbook only, no backing | — |
| 39 | How Insensitive | Bossa nova | — | — | No | Songbook only, no backing | — |

## Limitations and things to know

- **The sound is synthesized.** Guitar and fiddle are simple browser-generated tones, good for hearing the changes and the melody line, not realistic instruments. For the real feel, use the reference recording links.
- **Melody is missing for 10 tunes,** because the songbook has no stored notation for them. Those play guitar only, and the page says so.
- **Some melody files are different settings from the sheet.** Rubber Dolly's melody is in F and Orange Blossom Special's is a simple break in E, so their backing follows the melody, not the printed arrangement or your written chart.
- **Estimated and suggested chords need checking.** Tunes tagged "Timing estimated" or "Suggested chords" are best-effort, so trust your ear and the recording over the page.
- **Two songs have no backing.** Água de Beber and How Insensitive are bossa nova chord-melody arrangements with jazz voicings that don't fit a boom-chick vamp, and How Insensitive's sheet isn't saved in the songbook. Their sheet music, notes and links are still on the page.
- **Recordings and videos need internet.** They play from the original sites. If you open the page straight from your computer (file://), YouTube may refuse the embedded video; its link still works.
- **Sound needs a tap to start.** Browsers only allow audio after you press a button. On an iPhone, make sure the silent switch is off.
- **Settings stay on one device.** The page remembers your last song, player's view and alternating bass in your browser only, so they don't carry over to another device.
- **The site is public.** It's published with GitHub Pages at https://olv02.github.io/Bronson-Book/, so anyone with the address can open it.

## Quick start: practicing with it

1. Pick a tune and look at the capo tag. Put your capo on that fret, or play with none if the tag says "No capo".
2. Tap each chord button to learn the shapes before you play along.
3. Drop the tempo well below the default, leave count-in on, and press Play. Watch the beat boxes and the thickening strings to lock in the bass and strum pattern.
4. Turn on player's view if reading the strings upside down is slowing you down.
5. To drill a hard change, tap the bar just before it and turn on loop.
6. Raise the tempo a little each time through, toward session speed: about 100 to 120 bpm on dotted quarters for jigs, and 180 to 220 on quarter notes for reels.
7. Once the changes are solid, turn the melody down to 0 and back up the reference recording instead, using the link at the top of the song.
