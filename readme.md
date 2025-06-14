# FilamentColors envelope and label generator

**Open directly on Github without downloading:** https://murk-sy.github.io/filamentcolors-sample-envelope/sample-envelope.html

This was developed as a hopefully easier, simpler, and more accessible way to pack filament samples to send in to FilamentColors.xyz.

Initially developed for generating envelopes, now also supports generating labels (non-standard sizing, intended for cutting and inserting into bags).

The goal is to:

1) Reduce the required material for the sender - just paper, a printer and either a stapler or duct tape required to pack the filament.
2) Reduce the workload for the sender - no data is entered twice and the interface is dead simple.
2) Reduce the workload for FilamentColors - scanning the QR code removes the need to manually reenter data from labels.


## Features

- Can run locally, make sure you have qrious.js in the correct path
- Paper-size agnostic (though you should probably use A4 and US Letter)
- Filament samples can be bulk dried without unpacking (though may need to be packed for transport)
- QR code uses newline delimited data


## QR code

QR code supports UTF8 characters. The format is as follows, separated by a single \n:
```
FilamentColors v0
filament name
filament type
manufacturer
sender name
ISO date of generation
```

For example:

```
FilamentColors v0
Pearlescent Blue
PLA
Atomic Filament

2025-05-24
```

## License

Applies to sample-envelope.html only: CC0 Public domain