# Third-party notices and license tracking

This file tracks candidate upstreams. It does not mean their source code or assets have been copied into NOVA.

| Project | Candidate use | Checks required |
|---|---|---|
| [N.E.K.O](https://github.com/Project-N-E-K-O/N.E.K.O) | Candidate primary runtime | Preserve Apache-2.0 LICENSE/NOTICE; inspect bundled assets and dependencies separately. |
| [AILIS](https://github.com/haowenGuo/AILIS) | VRM/avatar, memory, voice and screen-context reference | Verify source license and all asset/dependency licenses. |
| [Warashi](https://github.com/inni918/warashi) | Memory, proactive conversation and barge-in reference | Inspect repository license, notices, bundled components and assets. |
| [Utsuwa](https://docs.utsuwa.ai/docs/overview/introduction) | Local speech/model and avatar reference | Identify current source repository and verify license before copying. |
| [Open-LLM-VTuber](https://github.com/Open-LLM-VTuber) | Live2D and speech reference | Verify source license and model/voice/avatar terms. |

Before importing any component:
1. Record upstream URL and exact commit/tag.
2. Preserve copyright and license notices.
3. Check model, voice, Live2D, VRM and other media terms separately.
4. Document modifications and imported files.
5. Exclude assets with unclear or incompatible terms.
