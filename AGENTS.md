# Authoring rules for daily-danish

This repository contains only generic Danish learning content. Never commit learner answers, personal evaluations, grades, recordings, private information, or individual corrections. Do not modify any other repository.

## Files and teaching
- Read AGENTS.md and these rules before editing. Preserve old lessons and stable field IDs. One self-contained static HTML per session: lessons/YYYY-MM-DD.html. Maintain index.html links. No backend, paid services, installation or runtime dependencies for the learner.
- Explain in Brazilian Portuguese; use Danish in teaching texts, examples and exercises. Combine everyday Danish with generic logistics contexts. Invented procedures must be labelled as fictional teaching scenarios, never official employer or safety instructions.
- Sessions total 30 minutes including instructions, phone typing, listening and review. No automatic optional homework. Regular lessons: date, stage, concrete objective, timed blocks, short review, one language explanation with examples, full main task, brief active production, review and response submission instructions.
- Glossaries and selective help come before the relevant task. Gradually fade support, reuse vocabulary and structures in new contexts and space reviews using observed errors. No automatic full translation or absolute translator ban.
- Practice short listening regularly and adjust duration/speed/complexity only with performance evidence. Teach classroom verbs: describe, explain, compare, justify, calculate, give examples. Cover quantities, units, dates, time, codes, receiving, storage, picking, deliveries, returns, discrepancies, sequences, clarification and messages.
- Do not infer a level from a past exam score or subjective listening percentage. Do not assume PD3 goal or claim an official assessment or guaranteed passing.
- Initial diagnosis uses two sessions of 30 minutes. Assess grammar (present, infinitive, modals, questions, negation, V2, connectors), everyday/logistics vocabulary, reading (gist, detail, sequence, conditions, exceptions), listening (gist, actions, numbers/time/quantities/responsibility), recipient/purpose-specific writing and two short oral tasks (response and procedure).
- Diagnosis is an exception to teaching the point first: do not reveal solutions in examples, placeholders, help, or audio before attempts. Reading and independent listening must not reuse the same text. Allow aids and record them without penalty. Preserve listening-only answers separately from transcript-assisted answers.
- After actual diagnostic responses: evidence-backed strengths, top three priorities and initial four-week plan adapted to real available time. Never infer completion from publication. Monthly mini-assessment and adjust load using reported real times.
- Corrections: original and corrected together, Markdown bold changes, preserve intention, separate errors and stylistic choices, evidence-based praise and at most three priorities; one short reuse. Transcripts alone cannot establish pronunciation or fluency.
- Only after correction add “Para lembrar” to that lesson with generic teaching rules, vocabulary and new examples with TTS. Never include answers or personal feedback in it.

## Interface
- Light background, separated cards, one column, no horizontal scrolling, legible text, fields at least 16px, touch-friendly buttons, visible associated labels, textareas, stable exercise/field IDs, no correction while typing.
- Danish TTS blocks: pale green, about 16px, font-weight 600, color #52655f. Audio button alongside every Danish phrase/example/question.
- Keep text near its questions. For long alternatives use accessible context modal if needed: named dialog, close button, Escape and return focus to opening control.
- Top Iniciar and bottom Parar timer. Timestamp-based, survives reload/app switches. Export total elapsed time.
- localStorage key unique by course, storage schema version, lesson ID/date; do not change key for content version updates. Input autosave debounce 500ms; include empty strings. Restore before listeners/defaults can overwrite data. Flush pagehide and hidden visibilitychange. Discreet saving/saved/error status; storage errors must not erase current input. Confirm before clearing.
- Explain storage is local to browser/device, not synced and lost if browser data is cleared. No answers sent to GitHub or any server.
- Copy answers button immediately flushes save and exports full self-contained correction prompt: date/title/ID/version, objectives, all needed instructions and reference texts/alternatives/transcripts separated from exact learner answers, every field ID, empty = “não respondido”, total time, aid/transcript-use records, request for generic-only “Para lembrar” update. No production answer keys or unnecessary browser/internal data.
- navigator.clipboard.writeText then confirm success only after resolve. On failure show selectable textarea. Never auto-send to ChatGPT.
- TTS URL: https://translate.google.com/translate_tts?ie=UTF-8&client=tw-ob&tl=da&q= plus encodeURIComponent(text). Play inline, no-referrer, one audio at a time, stop control, hide audio bar when idle. Split long source texts into short chunks without changing content. Show failures clearly; explicit speechSynthesis fallback only if a Danish voice exists, never another-language fallback.
- Listening: numbered audio buttons before transcript, speaker identity, initially hidden transcript controlled by learner, neutral playback bar without spoken text, record disclosure and preserve pre-disclosure attempt. Synthetic TTS is not spontaneous classroom speech.
- Validate storage, empty values, reload, transcript disclosure, timestamps, export success/fallback and mobile layout. Be transparent about untested live audio or publishing.

## Delivery
- Use only this repository. Verify actual hosted page before claiming it is live. If GitHub/Pages fails, explain and give available file fallback.
- No assumption that a lesson is completed; no catch-up accumulation. No duplicate dated files. Existing diagnosis session should be linked instead of creating a second workload for the same date.
