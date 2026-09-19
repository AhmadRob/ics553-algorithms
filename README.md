# ICS 553 Algorithms, Visualized

Interactive study notes for **ICS 553 (Algorithms)** at KFUPM. Every searching and sorting algorithm from the course notes is a step-by-step visualizer, with synced pseudocode and complexity explained in plain words.

**Live page:** https://ahmadrob.github.io/ics553-algorithms/

## What's inside

Nine algorithms, each with a visualizer, pseudocode, an explanation of how it works, and a complexity table with the reasoning behind it.

| Algorithm | Best | Average | Worst | Space |
|---|---|---|---|---|
| Linear Search | Θ(1) | Θ(n) | Θ(n) | Θ(1) |
| Binary Search | Θ(1) | Θ(log n) | Θ(log n) | Θ(1) |
| Merge | Θ(n) | Θ(n) | Θ(n) | Θ(n) |
| Bottom-Up Merge Sort | Θ(n log n) | Θ(n log n) | Θ(n log n) | Θ(n) |
| Selection Sort | Θ(n²) | Θ(n²) | Θ(n²) | Θ(1) |
| Insertion Sort | Θ(n) | Θ(n²) | Θ(n²) | Θ(1) |
| Bubble Sort | Θ(n) | Θ(n²) | Θ(n²) | Θ(1) |
| Radix Sort | Θ(kn) | Θ(kn) | Θ(kn) | Θ(n) |
| Quick Sort | Θ(n log n) | Θ(n log n) | Θ(n²) | O(n) |

Heap Sort has a placeholder card. It is not covered in the notes yet.

The page also has a short foundations section (what an algorithm is, its properties, O / Ω / Θ), a complexity cheat sheet, and a slider that compares the growth of log n, n, n log n and n².

## Using the visualizers

- **Play / Pause, Step, Back, Reset:** move through the algorithm one frame at a time, or scrub with the slider. Speed goes from 0.5x to 4x.
- **Pseudocode:** the lines being executed are highlighted on every step.
- **Live counters:** comparisons, interchanges, shifts or assignments, depending on the algorithm.
- **Presets:** switch between best, worst and random inputs. For example, Insertion Sort on sorted input takes n − 1 comparisons, and reversed input takes n(n−1)/2.
- **Your own input:** type numbers separated by commas in the `A` box (and `x` for the search cards), then click **Run** or press Enter. On Merge, split the two sorted runs with `|`, for example `2, 5, 8 | 1, 4, 6`.
- **Binary Search** also draws its decision tree, so you can see why the maximum is ⌊log₂ n⌋ + 1 comparisons.
- **Light and dark theme:** it follows your system setting, and the icon in the nav bar switches it.

## Run locally

There is no build step and there are no dependencies. Open `index.html` in a browser.

The page loads the Inter and JetBrains Mono fonts from Google Fonts. Without an internet connection it falls back to system fonts.

## Built with

Plain HTML, CSS and JavaScript in a single file. Each algorithm is a small function that records every step as a frame, and one shared player renders the frames. The visual style is monochrome liquid glass, matching my portfolio.

## Source

Based on my ICS 553 notes from KFUPM. The algorithm numbers (1.1, 1.2, 4.5, 5.5 and so on) follow the course notes.

## Author

Ahmed Abualrob ([@AhmadRob](https://github.com/AhmadRob))
