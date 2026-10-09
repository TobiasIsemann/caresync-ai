# CareSync: Automated Shift Handovers for Nursing
Final project for the Building AI course

## Summary
CareSync uses AI-driven speech-to-text and natural language processing to automate shift handovers for nursing staff. By translating spoken notes into structured reports, it reduces administrative burden and gives care workers more time for patients. 

## Background
In care facilities and hospitals, a significant portion of a shift is spent manually documenting notes and summarizing patient statuses for the next team. My personal motivation comes from my own experience working in nursing assistance, where I saw firsthand how much time and energy is spent on administrative tasks at the end of a demanding shift. 

This idea solves several overlapping problems:
- Manual documentation consumes valuable time that should be spent on actual patient care.
- Fatigue at the end of a shift increases the risk of human error or omitting critical medical details.
- Incoming staff need clear, standardized, and quick overviews rather than disorganized or fragmented notes.

## How is it used?
CareSync is used at the end of a nursing shift in care facilities, clinics, or hospitals. Instead of sitting at a computer typing out notes, a care worker speaks naturally into a secure mobile app or tablet, describing their patient rounds, vital sign changes, and general observations. 

The AI instantly translates and formats this into a standardized, bulleted handover report for the incoming shift team. The solution must take into account the high-stress, fast-paced environment of healthcare, meaning the interface must be extremely simple, and the voice recognition must be highly accurate.

## Data sources and AI methods
For a working prototype, the project would rely on simulated, anonymized voice memos to train and test the model. In a real-world scenario, the data would consist of live dictated notes from care staff.

The project depends on Natural Language Processing (NLP) and Speech-to-Text models. 

| Data Type      | AI Technique | Output Description |
| ----------- | ----------- | ----------- |
| Raw Audio Dictation      | Speech-to-Text (e.g., Whisper)       | Raw Text Transcript |
| Raw Text Transcript   | NLP / LLM Summarization        | Structured Medical Handover |

[OpenAI Whisper API](https://platform.openai.com/docs/guides/speech-to-text) is an example of an open-source model that could handle the initial transcription phase.

## Challenges
CareSync **does not** replace human judgment. A medical professional must always verify the AI-generated summary before finalizing the handover. 

Technical and ethical limitations include:
- The AI may struggle with heavy local dialects, accents, or highly specific medical jargon.
- Strict adherence to data privacy laws (like GDPR) is critical. Patient data cannot be sent to public, unsecured AI models, meaning a localized or highly secure enterprise model is required.

## What next?
The project could eventually grow to integrate directly with existing hospital Electronic Health Record (EHR) systems. It could also expand to include real-time, automated translation, allowing diverse, multilingual care teams to read the handover notes in their native language. 

To move forward, the project would need assistance from developers experienced in secure API integrations, as well as legal experts in European healthcare data compliance.

## Acknowledgments
- Inspiration drawn from the hard-working nursing and care staff who prioritize patient well-being every day.
