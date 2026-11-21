# TaktTime

A presentation timer for many speakers sharing one time slot, such as
15 talks in a 90-minute class. Each speaker's allotment is the time left
until the end divided by the speakers left, recalculated at every handover,
so an overrun is spread over everyone after.

Live: https://zero3kw.github.io/TaktTime/

- Set the end time (default: 90 minutes from now) or a length, and the
  number of speakers.
- → / PageDown / Space / Enter starts and hands over to the next speaker;
  ← / PageUp undoes the last handover. Works with presentation remotes.
- State is kept in `localStorage`, so a reload continues where it was.

Plain HTML and JavaScript served by GitHub Pages from `docs/`; no build step.
To view it locally:

```
python3 -m http.server 8000 -d docs
```
