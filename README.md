# route-optimization-visualizer
An interactive, single-file web app that compares two approaches to the delivery-route (travelling salesman) problem: an exact brute-force search and a fast greedy nearest-neighbour heuristic. Pick stops on a city map, run both algorithms, and watch where the greedy approach goes wrong.

## Features
 
- Click up to 8 stops on a 12-location city map (depot at the centre)
- Animated brute-force search that tries every permutation and tracks the best route so far
- Step-by-step greedy nearest-neighbour run, with the distance to each candidate logged
- Side-by-side summary of distance, run time and optimality gap
- Auto-generated "Run Conclusion" that explains the exact stop where greedy diverged from the optimal route
- Presets: 4-stop case, straight line, and a "greedy fails" case
- Randomize stops, adjustable simulation speed, and a skip-animation button

## Limitations
 
Distances are straight-line (Euclidean), with 1 map unit = 0.2 km. The lab ignores road networks, traffic and multiple vehicles. Every route starts and ends at the depot.
 
## Tech
 
Plain HTML, CSS and JavaScript with three stacked `<canvas>` layers (grid, routes, UI). Fonts: IBM Plex Sans and IBM Plex Mono via Google Fonts.
