# Maia-2 Chess Models

ONNX models for browser-based Maia-2 chess inference.

## Models

- `maia2_blitz.fp16.onnx` - Blitz time control model (~100MB)

## Usage

Load directly in browser with onnxruntime-web:

```javascript
const session = await ort.InferenceSession.create(
    'https://dxg7.github.io/maia-chess-models/maia2_blitz.fp16.onnx'
);
```

## About Maia

Maia is a human-like chess engine trained on millions of human games. Instead of finding the "best" move, it predicts what a human at a specific rating would play.

- Research: https://arxiv.org/abs/2008.10006
- Website: https://maiachess.com/

## License

Models are from the Maia Chess project (CC BY 4.0).
