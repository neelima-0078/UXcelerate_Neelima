## My Submission — AEGIS: Rescue Robot Coordination

**By Neelima**

### The problem
Coordinating rescue robots after an earthquake isn't a navigation problem — it's an *uncertainty* problem. Maps are incomplete, robots go silent, survivor detections aren't always confirmed, and routes that were safe five minutes ago might not be now. A dashboard that hides that uncertainty gets people hurt.

### Design decisions

1. **Incomplete maps are shown, not hidden.** Unexplored areas are marked as visible "fog" zones on the map rather than left blank — operators always know what the robots *haven't* seen yet.

2. **Silence looks different from confirmation.** A robot that's lost communication is shown greyed out with a dashed uncertainty ring around its last known position — instead of pretending it's still live, the interface makes the *staleness* of that data obvious.

3. **Survivor detections carry a confidence level.** Each survivor marker shows how it was detected (thermal-only vs. visually confirmed) and a confidence percentage, so responders can prioritize confirmed survivors over unconfirmed heat signatures.

4. **Route changes are visible events, not silent updates.** When a hazard blocks a path, the old route is struck through and the new one is drawn alongside it — so a reroute is something the operator notices and can question, not something that happens invisibly.

### Try it
Open `index.html` — or the live link below — and use the "Simulate detection" / "Simulate hazard" buttons top-right to see the map and incident feed update in real time.

**Live demo:** _[add your GitHub Pages link here once step 6 is done]_
