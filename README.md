# ContexQ AI Integration Layer

Architecture and bindings interfacing Genuity's synthetic data engine with
ContexQ's Reality engines.

## Flow

1. **Ingest** client reality logs via the ContexQ API.
2. **Synthesize:** strip PII and generate synthetic equivalents that preserve
   temporal sequence.
3. **Deliver** processed data back to ContexQ downstream modules.

## Contents

- `integration_layer.py` — interface skeleton.
- `SYSTEM_ARCHITECTURE.md` — flow spec.

## Status

Integration scaffold. Happy-path bindings are defined; hard cases (schema drift,
backpressure, idempotent redelivery) are open and tracked as follow-ups.
