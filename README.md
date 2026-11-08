# Free Christmas wrapping paper calculator (one HTML file, nothing stored)

Say how many presents you have in each size and what your roll looks like (width, length). You get the paper needed, the paper with a spare allowance, and the number of whole rolls to buy. No sign-up, no server, no cookies, no build step: it is one `index.html` file. Sizes are in centimetres.

**Use it now, no install:** download `index.html` and open it in any browser, or use the page version with a longer how-to at [tchworks.co.uk/free/christmas-wrapping-paper-calculator-2026](https://www.tchworks.co.uk/free/christmas-wrapping-paper-calculator-2026/?utm_source=github&utm_medium=repo&utm_campaign=wrap-calc-repo).

**Free printable PDF (no install):** [Download the A4 pack](https://github.com/wilsonryan-hue/christmas-wrapping-paper-calculator/releases/download/v1.0.0-free-printable/christmas-wrapping-paper-planner-2026-free.pdf) — size reference table, blank planning sheet, worked 15-present example, tips ([release notes](https://github.com/wilsonryan-hue/christmas-wrapping-paper-calculator/releases/tag/v1.0.0-free-printable)).

## The sum

For one box with length L, width W and height H, the paper has to go right round the box and run past each end:

- Round the box: `2 x (W + H) + 2` cm (the 2 cm is for the overlap).
- Past the ends: `L + min(W, H)`.

The calculator tries all three ways of turning the box, in both directions across the roll, keeps only those where the round-the-box side fits the roll width, and takes the shortest length of paper. A box that fits no way round is flagged as too wide, not counted. Total paper = sum of (length per box x how many), times `1 + spare%`; rolls to buy = total / roll length, rounded up.

Worked example (defaults: 70 x 300 cm roll, 10% spare): 4 books 22x15x3, 4 mugs 12x12x12, 4 shoeboxes 32x20x12, 2 board games 40x28x8 and 1 big box 50x40x30 come to 15 presents, 6.5 m of paper, 7.2 m with spare, so 3 rolls to buy with about 1.8 m left over (checked against a separate hand calculation).

## Change it

Open `index.html` in a text editor. The row names and starting sizes are in the table; the spare allowance default is the `sp` field. Everything runs in your browser; typed numbers are never sent anywhere.

## Limits

An estimate only. Odd shapes: enter the smallest box that would hold them. Check the size on the roll label before you buy.

## Licence

MIT. Made by [TCH Works](https://www.tchworks.co.uk/?utm_source=github&utm_medium=repo&utm_campaign=wrap-calc-repo), which also publishes free [printable gift tags](https://www.tchworks.co.uk/free/christmas-gift-tags-printable-2026/?utm_source=github&utm_medium=repo&utm_campaign=wrap-calc-repo), [Christmas cards](https://www.tchworks.co.uk/cards/christmas/?utm_source=github&utm_medium=repo&utm_campaign=wrap-calc-repo) and a printable [Christmas Budget & Gift Planner](https://tchworks.gumroad.com/l/kazjns?utm_source=github&utm_medium=repo&utm_campaign=wrap-calc-repo).

## Free printable on Gumroad

Get the A4 wrapping paper planner free (£0, pay what you want): https://tchworks.gumroad.com/l/bpurzh
