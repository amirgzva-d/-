# NOVA Architecture (Draft)

## Core rule
The LLM provider must be replaceable without losing the companion's personality, conversation history, or durable memories.

## Components
- **Desktop UI:** chat, settings, avatar surface, permission indicators.
- **Conversation orchestrator:** streaming turns, cancellation, interruption, context assembly.
- **Personality:** editable persona, tone, behavioral rules, boundaries.
- **Provider adapters:** common interface for local and hosted LLMs.
- **Memory service:** conversation history, summaries, durable facts, retrieval, correction and deletion.
- **Speech service:** speech-to-text, text-to-speech, voice activity, barge-in.
- **Avatar service:** expressions, phoneme/lip-sync events, animation.
- **Perception service:** separate webcam and screen capture sessions.
- **Settings/secrets:** local configuration and protected credentials.

## Conversation pipeline
1. Receive text or audio.
2. Transcribe audio when needed.
3. Retrieve only relevant memories.
4. Compose persona + context + user message.
5. Stream the model response.
6. Drive speech and avatar events from the response stream.
7. Propose candidate memories and persist according to user-controlled memory settings.

## Provider abstraction
Potential local providers include Ollama-compatible endpoints. Hosted providers can be added through documented APIs and user-provided credentials. A consumer ChatGPT subscription must not be assumed to include API access.

## Memory rules
- Conversation history and long-term memory are separate.
- Store source, timestamp, confidence, and editability.
- Provide inspect, correct, export, and delete controls.
- Do not store sensitive information by default.
- A model must not silently change privacy or permission settings.

## Webcam and screen are separate
Webcam capture and screen capture require independent permission flows, visible indicators, and start/stop controls. Screen understanding does not imply webcam support.

## Security
The first milestone does not execute shell commands, arbitrary scripts, or unattended Windows actions. Future computer-control tools must use scoped permissions, allowlists, confirmation for consequential actions, audit history, and an emergency stop.

## Upstream compatibility
N.E.K.O is the leading candidate runtime. AILIS, Warashi, Utsuwa, and Open-LLM-VTuber are reference projects, not code to merge wholesale. Different frameworks and dependency stacks must be integrated through stable interfaces rather than copied directly.
