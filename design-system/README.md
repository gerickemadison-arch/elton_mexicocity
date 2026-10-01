# Elton John Mexico City

**Bottle-green satin, gold-foil stars, one flash of pink. A rock-and-roll night dressed for Mexico City.**

This system covers the stationery and screens for an Elton John night in Mexico City: invitation, itinerary, tickets, signage, menus and social posts. It is built on the 1975 Walk of Fame suit: a pistachio satin jacket with a bottle-green lapel, gold stars and pink star-shaped glasses. It also borrows the 1989 letterpress concert poster (star rows, tight billing) and carnival stationery (the sunburst, the ticket stub).

## Three principles

1. **Green is the room.** Every piece sits on lapel green, and everything else is lit against it. Cream is the light, gold is the sparkle and pink is the wink. Star Glasses pink is the late-night side room, small and saved for the after-party.
2. **One showpiece per piece.** Each item gets one loud moment, such as the wordmark, the sunburst or a pink line. Everything around it stays quiet and easy to read.
3. **Spanish first.** Dates, places and headlines are in Spanish (*Sábado 18 de febrero*). English sits underneath, smaller, only where a guest needs it.

## Colour

There are two themes built from the same role tokens. **Lapel** is the system; **Star Glasses** is a small accent you switch on for one panel or one small piece.

On a Lapel piece, aim for roughly **60% `ground`, 25% `text` and `stock`, 10% `stripe` and `ground-deep`, and 5% `star` and `spark`.**

| Token | Role | Lapel (main) | Star Glasses (accent) |
| --- | --- | --- | --- |
| `ground` | background | bottle green #1e5a3c | hot pink #ff6f9c |
| `text` | all main text | cream, 7.3:1 | deep green, 5.5:1 |
| `text-second` | addresses, captions | pistachio, 6.1:1 | berry, 5.2:1 |
| `label` | eyebrows, times | gold, 5.0:1 | deep green, 5.5:1 |
| `star` | star rows, wordmark star | gold foil | deep green |
| `spark` | the one italic aside | pink, 4.5:1 (21px+) | berry, 5.2:1 |
| `stripe` | satin band | pistachio | tangerine |
| `ground-deep` | deep panels, sunburst field | #123d28 | #0e3020 |
| `ray` | sunburst rays | gold | tangerine (unused: no pink sunburst) |
| `seam` | hairlines only | #3f7a5a | #e0507f |
| `stock` / `stock-ink` | tickets | cream with green text | cream with deep-green text |

Rules:
- Gold and pink never sit on cream. On cream stock, the only text colour is `stock-ink`.
- Each piece gets one pink moment: either the `spark` line or a Star Glasses panel, not both.
- Don't add colours. If a piece needs more emphasis, use scale, not a new colour.

### The Star Glasses accent

Hot pink from the sunset lenses, used as a **side accent** for the late-night moments. See the Star Glasses accent component.
- **As a panel:** up to one third of a Lapel piece, such as the after-party column on the night's schedule.
- **As a small piece:** drink tickets, after-party cards, wristbands, stickers.
- The invitation front and the itinerary stay fully Lapel. There's never a pink sunburst, because the concert is always Lapel.
- **To use it:** put `data-theme="star-glasses"` on the panel. Every role token remaps, so the components work unchanged.

## Type

| Role | Face | Use |
| --- | --- | --- |
| Display | **Shrikhand** | The name, one headline, the featured event. 32px and up only. |
| Accent | **Cormorant Garamond Medium Italic** | The emotional line (*una noche nada más*) and event names. |
| Text | **Josefin Sans** | Body, details and tracked capitals for days, times and labels. |

Hierarchy on a typical piece, top to bottom: `eyebrow` (`label` caps), then `wordmark` or `headline` (`text`, Shrikhand), then `aside` (`spark` italic), then `body` (`text`), then `detail` (`text-second`).

- Track all capitals at 0.18 to 0.22em. Never track Shrikhand or the italic.
- Never set Shrikhand in all caps, and never set more than six words in it.
- Use lining numerals for times and dates.

## The lockup

There's no logo file yet, so the name is the mark: **Elton ★ John**, set in Shrikhand in cream with a gold five-point star between the words. There are two arrangements, both shown in the Wordmark component:
- **Inline:** *Elton ★ John* on one line, for headers and social posts.
- **Stacked:** *Elton* over *John*, with the star hanging to the right of *Elton*. Use it for posters and the invitation front.

Keep at least one star-height of clear space around it, and keep it at least 120px (or 1.25in) wide. When it appears on cream, the type is lapel and the star stays gold only if the piece is foil-stamped.

## Signature elements

- **The satin band.** Vertical `stripe` stripes (pistachio, or tangerine in Star Glasses) (36px stripe, 12px gap) across the top edge of a piece, finished with a scalloped bottom edge (24px pitch). It's the system's frame: use it on the invitation, menus and the itinerary header.
- **Star rows.** A row of small `star` stars marks a threshold, such as above the name or between sections. Use one row per piece.
- **The sunburst.** Gold rays on `ground-deep` behind a cream ticket. It marks **the one main event** (the concert) and appears once in the whole itinerary. This is the borrowed carnival moment; its rarity is what makes it work.
- **The notched ticket.** Cream `stock` with cut corners (`notch`, 12px), `stock-ink` text and an eyebrow at the top. It's used for the featured stop, drink tickets and place cards.

## Layout

- **Margins:** `space-5` (48px on screen, about ½in on a 5×7 card).
- **Alignment:** left-aligned by default. Centre only inside a ticket.
- **Rows:** itinerary rows use a fixed day-and-time column (gold caps) next to the event (cream italic over a pistachio detail line), divided by `seam` hairlines.
- Corners are square except the ticket notch.

## Voice

- **Warm, theatrical, short.** *Step right up. Una noche nada más. Pásale.*
- Use song titles as section names, at most once per piece: *Tiny Dancer* for the dance floor, *Rocket Man* for the after-party.
- Times read like a ticket: *Sáb · 8 PM*, not "Saturday at 8:00 p.m."

## Production notes

- **Print:** cream or white uncoated stock, flooded with lapel green, or a green duplex card. Gold becomes **gold foil**, so keep foil to the stars, rays and eyebrow labels, never small body text. Star Glasses pieces print as a pink flood with tangerine and deep-green spot inks; a fluorescent pink makes drink tickets glow under bar lighting.
- Screen tokens are not print matches. Match lapel, pistachio and pink to a printed swatch book before running stock.
- **Screen:** the Lapel theme is the default for social posts and the web RSVP. Use Star Glasses for after-party stories only.

## Don'ts

- Don't use black anywhere. The darkest colour is `ground-deep`.
- Don't put a sunburst on more than one stop, or a star row and a sunburst together in one panel.
- Don't use cursive scripts. The italic serif is the only "handwritten" voice.
- Don't use photos of Elton or his album art. The references in the Moodboard group are for mood only.

## Moodboard

The **Moodboard** asset group holds the reference images this system was built from, with notes on what each one contributed.
