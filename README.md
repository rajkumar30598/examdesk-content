# ExamDesk content

These are the static exam papers for the ExamDesk app. Push this folder as the root of a public GitHub repo, then point `CONTENT_BASE_URL` in the app's `lib/config.ts` at it.

- `index.json` lists every exam and paper. Each paper `path` is relative to this repo's root.
- `exams/<exam-id>/<file>.json` holds the paper files: `{ id, exam, year, title, questions: [...] }`.
- Each question has the shape `{ id, exam, year, subject, topic, question, options[4], answerIndex (0-3), explanation }`.

`exams/demo/sample.json` contains original demo questions, not real previous-year questions.

Use the **Issues** tab to report errors in questions. The app's "Report an error" button opens a pre-filled issue here.
