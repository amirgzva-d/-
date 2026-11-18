# NOVA — Personal AI Companion

NOVA is a modular, Windows-first personal AI companion. The first milestone focuses on natural text and voice conversation, a consistent personality, long-term memory, and an expressive avatar. Screen and webcam perception are planned as permission-based capabilities. Windows automation is intentionally out of scope for the first milestone.

## Principles
- Keep personality and memory independent from the selected model.
- Support local and hosted model providers through adapters.
- Make microphone, webcam, and screen capture explicit, visible, and easy to stop.
- Build Windows-first and design for Persian RTL, speech recognition, and speech synthesis.
- Reuse upstream components only after checking compatibility, maintenance, security, and licenses.

## Candidate upstreams
- [N.E.K.O](https://github.com/Project-N-E-K-O/N.E.K.O) — leading runtime candidate.
- [AILIS](https://github.com/haowenGuo/AILIS) — VRM avatar, memory, voice, and screen-context reference.
- [Warashi](https://github.com/inni918/warashi) — memory, proactive conversation, and barge-in reference.
- [Utsuwa](https://docs.utsuwa.ai/docs/overview/introduction) — local speech/model and avatar reference.
- [Open-LLM-VTuber](https://github.com/Open-LLM-VTuber) — Live2D and speech reference.

N.E.K.O is the leading candidate, not yet integrated. The upstream repository metadata reports Apache-2.0. Code, models, voices, and avatar assets can have separate licenses and must be checked individually.

## Milestones
1. Audit upstream Windows support, dependencies, licenses, and webcam feasibility.
2. Build text chat and replaceable model-provider adapters.
3. Add a consistent personality and editable long-term memory.
4. Add speech recognition, speech synthesis, and interruption (barge-in).
5. Add avatar expressions, motion, and lip sync.
6. Add permission-gated screen and webcam perception.
7. Package, test, and document the Windows application.

## Current status
This repository is being prepared as the NOVA project workspace. The upstream N.E.K.O runtime has **not** been imported or forked yet. The first commits establish project scope and architecture; implementation will follow after the upstream audit.

## Language
فارسی: نُوا یک دستیار هوشمند شخصی و ماژولار است. هدف مرحله اول، مکالمه طبیعی متنی و صوتی، شخصیت پایدار، حافظه بلندمدت و آواتار زنده است. دسترسی به وب‌کم و صفحه‌نمایش فقط با اجازه روشن کاربر انجام می‌شود. کنترل ویندوز به مرحله بعد موکول شده است.
