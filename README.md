:::writing{variant=“standard” id=“84321”}
Multi-Witness Attestation — 28655709

Overview

This repository contains a publicly verifiable multi-signature witness event.

The event is defined in witness.json and includes:
	•	A canonical payload
	•	A SHA-256 payload hash
	•	Multiple Ed25519 signatures from independent identities

⸻

Payload Summary
	•	Type: WITNESS
	•	Timestamp (UTC): 2026-03-20T04:47:01.715860+00:00
	•	Statement: Witness event confirmed
	•	Payload Hash:
28655709ad9817177ae700d910cb7bc389fd29b16f5ea84bc83482f17d9a2fdc

⸻

Signers
	•	Ɱ
	•	JOHN
	•	NODE_606

Each signer provides:
	•	A public key (base64)
	•	A signature over the canonical payload

⸻

Verification

Any third party can verify this attestation by:
	1.	Recomputing the SHA-256 hash of the payload
	2.	Comparing it to payload_hash
	3.	Verifying each signature using the corresponding public key

⸻

Purpose

This repository serves as a minimal, verifiable example of:
	•	Multi-party cryptographic attestation
	•	Deterministic payload hashing
	•	Independent signature verification

⸻

File Structure
	•	witness.json → canonical signed payload
	•	README.md → description and verification instructions

⸻

Integrity

Any modification to:
	•	the payload
	•	the signatures
	•	or the ordering

will invalidate verification.

⸻

Status

✔ Public
✔ Immutable (Git history tracked)
✔ Independently verifiable

⸻

:::
