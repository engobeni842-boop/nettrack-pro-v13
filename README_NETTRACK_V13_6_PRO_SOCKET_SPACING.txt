NetTrack Pro V13.6 — Pro Socket + Spacing Patch

Base: V13.5 Lock-In Signal Platform.

Fixes applied:
- Professional spacing pass: smoother cards, smaller heavy headings, cleaner Signal A/B flow.
- Socket recovery improved: REST candle preload failure no longer kills the dashboard.
- Crypto sockets now retry as RECONNECTING instead of staying stuck on ERROR.
- BTC/ETH/SOL/BNB can keep a backup feed active while the live socket retries.
- Broker/platform switch now refreshes dashboard alignment and Signal A/B provider view.
- Signal A/B follows selected broker/platform instead of stale provider text.
- Online/offline browser events now trigger reconnect logic.

Notes:
- Firebase/API settings were not removed or changed.
- Main V13 structure was preserved.
- Subscription locks still keep sensitive/advanced sections gated while Signal A/B remains usable.
