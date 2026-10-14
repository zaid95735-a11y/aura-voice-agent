# Aura Skincare - AI Voice Agent Aria
Built for Datastraw Assessment by Mohd Zaid Khan

Live URL: [Vercel ke baad yaha daalna]

## Architecture
Browser-native modular pipeline: Web Speech API (STT en-IN) -> JS reasoning with get_order_details tool -> SpeechSynthesis (TTS Indian voice). No API keys needed for instant evaluation.

## Why this stack?
Per assessment, vendor not important. Focused on UX, guardrails, low latency. Deploys anywhere.

## Section 9 Answers
1. Architecture: Chose browser-native to avoid API costs, frictionless testing, meets all core reqs.
2. Difficult: Continuous listening after TTS. Solved via onend callback restarting recognition.
3. One more week: Add real LLM (Gemini), barge-in, Hinglish, vector DB.
4. 1000 calls/day: Move to LiveKit, Deepgram STT, GPT-4o mini, ElevenLabs, Redis, Postgres, monitoring, PII redaction.
