JLPT N2 quiz project. Furigana lookup data is stored separately in jlpt-n2-furigana-dictionary.js and is display-only; it is not used for quiz generation.


## v65 study-focused improvements

- Added phrase-level furigana overrides for common compounds and inflected forms, including 今週（こんしゅう） and 受け付けて（うけつけて）. Phrase matches take precedence over per-kanji fallback readings.
- In regular vocabulary sessions, inserts one contextual advanced item after each five vocabulary questions. It alternates between contextual blank-fill and sentence-order reconstruction when the example supports the format.
- Hides furigana while an advanced question is being answered and reveals the completed sentence with furigana after submission.
- Adds a visible three-second preview gauge and allows tapping the kanji preview card to reveal the answer choices immediately.
- All inline JavaScript passed syntax validation. Full linguistic correctness still requires native-speaker review; the phrase-level corrections are not a claim that every reading in all 653 examples has been human-verified.


## v66 advanced-question fixes

- Removed the Korean sentence translation from the unanswered advanced blank-fill question; it is now shown only after answering (or skipping), so it cannot reveal the answer prematurely.
- Changed the blank-fill prompt to ask learners to infer the missing vocabulary from context and grammar rather than relying on the translation.
- After answering or skipping an advanced question, the explanation now explicitly renders the key vocabulary as ruby text with its reading, in addition to the sentence-level furigana. This keeps the dictionary headword reading visible even when the sentence uses an inflected form.


## v67 kanji preview countdown gauge

- Added a visible remaining-time gauge under the kanji during the three-second meaning-question preview.
- The gauge animates for the same three seconds as the existing choice-reveal delay.
- The gauge disappears when choices appear, and tapping the kanji to reveal choices early cancels the gauge immediately.
- No question timing, scoring, or answer logic was changed.
