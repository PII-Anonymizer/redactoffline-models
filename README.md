# RedactOffline model downloads

Versioned model files for on-device text detection in RedactOffline. No user
documents, app credentials, or private application source are stored here.

## GLiNER2 base INT8 v1

- Source: [fastino/gliner2-base-v1](https://huggingface.co/fastino/gliner2-base-v1).
- Source revision: `f9634218e53580c56edf0de97ca1a7d3f1c2354e`.
- English base checkpoint, Apache-2.0; not the multilingual privacy-filter model.
- MLX affine INT8 encoder and token embeddings, group size 64; FP16 heads,
  norms and relative embeddings.
- Runtime download: 253,860,552 bytes across model.safetensors, tokenizer.json,
  and config.json. No account or document upload is required.
- Release assets include an artifact manifest with exact byte counts and SHA256
  checksums, LICENSE, and NOTICE.txt. Clients must verify hashes before loading.

Weights were mapped with MacPaw GLiNER2Swift at
`99459ae39598176c5ad8455b6469317ebe24f551` and quantized with MLX 0.32.3.
Quantized model scores are not guarantees of PII recall.
