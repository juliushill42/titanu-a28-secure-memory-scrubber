# titanu-a28-secure-memory-scrubber

> Scrubs PII and sensitive fields from MongoDB documents on configurable retention policy.

**Track:** MONGODB | **Author:** Julius Cameron Hill — TitanU AI LLC | **Patent:** JCH-2026-001

## Overview

Built for the **Google Cloud Rapid Agent Hackathon** using **Gemini 2.5 Flash** + **Vertex AI** + **Mongodb MCP Server**.

## Architecture

```
User Query → Gemini 2.5 Flash (Vertex AI)
                    ↓
         MONGODB MCP Server
                    ↓
         Structured JSON Response
```

## Setup

```bash
npm install
cp .env.example .env
# Set GOOGLE_CLOUD_PROJECT, GOOGLE_APPLICATION_CREDENTIALS
node src/index.js
```

## Environment

| Variable | Description |
|---|---|
| `GOOGLE_CLOUD_PROJECT` | GCP project ID |
| `GOOGLE_CLOUD_LOCATION` | Region (default: us-central1) |
| `MCP_URL` | Mongodb MCP endpoint |

## Tech Stack

- **AI:** Gemini 2.5 Flash via Vertex AI / Google ADK
- **Partner:** Mongodb MCP Server
- **Runtime:** Node.js
- **Cloud:** Google Cloud

## License

MIT — see [LICENSE](LICENSE)

## IP Notice

TitanU AI LLC — Julius Cameron Hill. JCH-2026-001.
