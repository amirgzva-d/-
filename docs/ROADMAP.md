# NOVA Roadmap

## Phase 0 — Audit and foundation
- [x] Establish project scope and modular architecture.
- [ ] Inspect N.E.K.O Windows install/build path and dependency footprint.
- [ ] Inspect exact licenses for source, models, voices, and avatar assets.
- [ ] Evaluate AILIS, Warashi, Utsuwa, and Open-LLM-VTuber feature boundaries.
- [ ] Confirm webcam feasibility and design a permission-based capture module.
- [ ] Establish repeatable Windows development setup and smoke tests.

## Phase 1 — Text conversation
- [ ] Minimal desktop chat UI.
- [ ] Streaming responses, cancellation, and conversation history.
- [ ] Provider adapter interface.
- [ ] At least one local model adapter and one hosted adapter.

## Phase 2 — Personality and memory
- [ ] Editable persona profile.
- [ ] Persistent memory with retrieval and provenance.
- [ ] Review, edit, export, and delete memory controls.
- [ ] Optional proactive conversation with quiet hours and opt-out.
- [ ] Verify that changing model providers does not erase persona or memory.

## Phase 3 — Voice
- [ ] Explicit microphone permission.
- [ ] Speech recognition and natural speech synthesis.
- [ ] Barge-in and playback cancellation.
- [ ] Persian speech recognition and voice quality tests.

## Phase 4 — Avatar
- [ ] Choose Live2D or VRM based on compatibility and asset licenses.
- [ ] Emotion mapping, lip sync, idle and conversational motion.

## Phase 5 — Perception
- [ ] Screen capture with monitor/window/region selection.
- [ ] Webcam capture with explicit permission and visible active indicator.
- [ ] Vision provider adapter and data minimization.

## Phase 6 — Release quality
- [ ] Windows packaging and update strategy.
- [ ] Performance profiling and crash recovery.
- [ ] Persian RTL UI and accessibility review.

## Later milestone — Windows control
Only after the companion experience is stable: permission-scoped actions, allowlisted commands, confirmation for consequential actions, audit history, and emergency stop.

## First usable build acceptance
A Windows user can launch NOVA, chat by text, select a local or hosted model, edit the companion persona, and retain history/memory across model switches. No camera, screen, microphone, or computer-control activity occurs without an explicit user action.
