# platform_external_piper — reserved

This repo is currently reserved but **not active** in the JibarOS manifest.

## Why it exists

JibarOS v0.6.9 runs Piper text-to-speech through `platform_external_onnxruntime` — `oird` loads the Piper `.onnx` voice model directly via ONNX Runtime. No separate Piper runtime is required today.

This repo is a placeholder in case we later need native Piper integration (custom G2P, new voice formats, Piper CLI tools on-device). Not currently wired into `jibar-os/manifest`.

## See also

- [`platform_external_onnxruntime`](https://github.com/Jibar-OS/platform_external_onnxruntime) — the runtime that actually executes Piper voices today.
- [`docs/MODELS.md`](https://github.com/Jibar-OS/docs/blob/main/MODELS.md#audio-synthesize) — how `audio.synthesize` is wired.

## Migration status

🚧 No active source import planned. Not on v1.0 critical path.
