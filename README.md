# platform_external_piper — Piper fork for JibarOS

JibarOS-maintained fork of [`rhasspy/piper`](https://github.com/rhasspy/piper).

Reference backend for OIR's `audio.synthesize` capability (text-to-speech).

## Why fork

- Reproducible snapshot pins.
- Android `Android.bp` wiring so Piper's VITS ONNX models can be loaded through the shared ONNX Runtime already on the device.

## Runtime requirements

Each voice model needs a G2P (grapheme-to-phoneme) sidecar at `<model>.phonemes.json`. Without it, `audio.synthesize` returns `CAPABILITY_UNAVAILABLE_NO_MODEL` cleanly — no silent bad audio.

## See also

- Upstream: [`rhasspy/piper`](https://github.com/rhasspy/piper)
- JibarOS consumer: [`oird`](https://github.com/jibar-os/oird)

## Migration status

🚧 Transfer/creation in progress.
