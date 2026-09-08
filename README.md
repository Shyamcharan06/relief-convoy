# Relief Convoy

A disaster-relief logistics planner built for a Design & Analysis of Algorithms (DAA) project.

Given a manifest of relief resources and a road network between a warehouse and relief locations, it:

- Splits resources into unsplittable and splittable classes and solves them with **0/1 Knapsack** and **Fractional Knapsack** respectively, with a full DP-table / greedy-fill trace.
- Finds the optimal delivery loop with **TSP solved via Dynamic Programming**, with a step-by-step trace of how the tour was built.
- Lets you block roads (simulating floods, landslides, bridge collapses, earthquakes) and re-solves the route live around the disruption.
- Reports resource, route, and algorithm-performance statistics, plus a printable mission report.

Static site, no backend — everything runs client-side in a single `index.html`.
