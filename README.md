# testclock

A tiny single-file web page that shows a digital clock running at 4× real time. It starts at 4:00 PM local time as soon as you open the page, and displays in 12-hour format with AM/PM.

## How to run locally

Option 1: Open `clock.html` directly in your browser (double-click it).

Option 2: Serve it with a local web server and open the URL it prints (helpful to avoid any file URL quirks):

```bash
# From the repository root
python3 -m http.server 8000
# Then open http://localhost:8000/clock.html
```

## Notes

- The clock advances using a simulated time based on a monotonic timer, so it avoids drift and updates smoothly.
- Speed is fixed at 4×.
- There are no controls; it’s a passive display.
