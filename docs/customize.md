# Customize

All content is data at the top of the `<script>` in `index.html`. No build step.

## Add an industry preset

Add a key to `IND` and a button to `#indSeg`:

```js
IND.fin = {
  label: 'Fintech',
  leadsLbl: 'Demo requests / month',
  d: { leads: 60, acv: 30000, conv: 6, cycle: 90 },        // audit defaults
  eh: { easy: 'Head of product…', hard: 'Compliance and risk…' },
  subs: { s4: 'Security review, procurement' },              // node subtitle overrides
  caseT: 'Typical fintech leak pattern',
  caseL: ['<b>Leak.</b> Fix.', '…'],
};
```

```html
<button data-i="fin">🏦 Fintech</button>
```

## Add a leak

Add an object to `LEAKS`:

```js
{
  k: 'price',                      // short id, used in share links
  w: 10,                           // weight in the alignment score
  t: 'Discounts are given without approval',
  asm: 'Discount discipline recovers {p}% of revenue.',  // {name} becomes an editable input
  p: { p: 3 },                     // defaults for those inputs
  src: '<b>Source (year)</b>: what it says.',
  calc: (b, p) => b.rev * p.p / 100,   // b = {rev, deals, lost, acv}
  fix: ['Step 1', 'Step 2', 'Step 3'],
  zov: 'What gets automated.',
  edges: ['m2-s4'],                // map lines that turn red
}
```

Qualitative leak (score only): set `q: true` and leave out `asm`, `p` and `calc`.

Keep the weights summing to about 100 so the score stays 0–100.

## Change the call to action

Search for `zov911.com`. The links appear in the result card, the footer card and the Revenue Sprint dialog.

## Check before you push

1. Open `index.html` and click through the map, **Show leaks** and the audit.
2. Narrow the window to phone width: no horizontal scroll.
3. **Copy link**, open it in a new tab: the same numbers load.
