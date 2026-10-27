# Hospital Resource Management – Surge Twin

A simulated multi-agent system that helps a hospital respond to emergency
department (ED) surges, with a human approving every change.

**Live demo:** https://priyan3002.github.io/surge-twin/

## How it works
- **Surge agent:** detects surges and forecasts arrivals six hours ahead.
- **Bed, staff and equipment agents:** report on beds, nurses and equipment.
- **Coordinator:** drafts three plans (Conservative, Balanced, Aggressive).
- **Digital twin:** replays each plan six hours forward and scores it on
  ED boarding and nurse strain.
- **Safety verifier:** checks nurse ratios and reserve beds. A plan that
  fails cannot be approved.
- **Human approval:** nothing changes without approval. Every decision
  is written to an audit trail.

## Example
Click "Trigger ED surge". The Balanced plan gets the best twin score and
is recommended. The Aggressive plan moves the most patients but is rejected,
because it leaves too few ward beds free.

## How to run
Open the live demo link, or download `index.html` and open it in a browser.

## Limitations
- Runs on simulated, synthetic data. It is not connected to any hospital system.
- The agents are rule-based, not AI models.
- The forecast is a simple smoothing model.
- Safety thresholds are assumptions, not clinical standards.
- Not for clinical use.

## References
(Add your references here.)
