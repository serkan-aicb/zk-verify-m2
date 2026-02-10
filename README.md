AI.COREBLOCK — zkVerify Milestone 2 Evidence

This repository contains the evidence package for Milestone 2 (Initial Traction) of the AI.COREBLOCK project in the Thrive zkVerify Web3 Program.

The goal of this repository is to allow independent verification of the milestone requirements without any prior knowledge of the project.

⸻

What is included

This repository contains two core artifacts:

1. Technical Documentation (PDF)
	•	AICB-zkTelemetry-zkVerify_080226.pdf
	•	Describes the full end-to-end pipeline:
	•	smartphone telemetry ingestion
	•	proof job creation in Supabase
	•	submission via Kurier
	•	verification on zkVerify mainnet
	•	persistence of correlation identifiers (Kurier job ID, zkVerify tx hash)
	•	Documents real-time and batch testing, worker configuration, retries, and synchronization logic.

This document explains how the system works.

⸻

2. Proof-Level Dataset (CSV)
	•	Supabase Snippet Smartphone Telemetry Sessions Overview.csv
	•	Contains proof-level records extracted from Supabase.
	•	Each row represents a telemetry session and/or proof job processed through the system.

The CSV is intentionally detailed to ensure full traceability.

Key fields include (non-exhaustive):
	•	commitment_hash — proof-level identifier
	•	kurier_request_id — Kurier job correlation ID
	•	zkverify_tx_hash — zkVerify on-chain extrinsic hash
	•	zkverify_explorer_url — direct link to the public explorer
	•	session identifiers linking raw and derived (scaled/batched) proofs
	•	timestamps and job state metadata

This dataset explains what actually happened.
