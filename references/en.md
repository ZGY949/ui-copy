# English wording

For English interfaces. Existing product conventions, real terminology, and the target locale take priority. These are defaults, not rules that apply to every language.

## Remove the sentence scaffolding first

- Use a direct word or phrase for a title or action. Remove repeated lead-ins such as "You can," "On this page," and "Please click below," while retaining a clear object and action.
- Let titles, field labels, states, and guidance serve separate purposes. Do not repeat a shorter version of the same introduction in several places.
- Choose familiar, precise words. A shorter phrase must still refer to the same object or action; do not replace clarity with a more decorative term.

## Tone and meaning

- Use familiar words and direct actions. Keep implementation terms out of general-user interfaces unless they help a decision. Specialized tools may retain terminology their users understand.
- Put the object, result, or consequence early. Remove empty lead-ins and repeated greetings. Follow an established brand voice in context; serious failures should not become jokes.
- Check pronouns and perspective. A statement to the user and an action that speaks on the user's behalf may need different wording.
- Use stable names for the same object and action. Understand business distinctions before unifying terms: Remove and Permanently delete, or Save draft and Publish, are not interchangeable.
- Choose labels such as Confirm, Done, and Apply according to the action they actually perform. They are neither forbidden words nor universal defaults.

## Numbers, dates, punctuation, and capitalization

- Use clear counts and units, such as 2 files and 3 days. Follow product and locale conventions for currency, percentages, dates, and measurements.
- Titles, buttons, labels, and standalone short hints usually do not need periods. Use normal punctuation in full explanations; do not strip punctuation from important sentences for visual consistency.
- Ordinary success and error messages do not need exclamation marks by default. Use conversational language or emoji only when the brand and situation allow it without reducing clarity.
- Use the product's capitalization convention consistently. Sentence case is often suitable for UI labels, but do not impose it over an established design system.
- Say when a date is unknown. Relative time needs a clear reference in notifications or shared content; use a date and relevant time zone when needed.
- Preserve names, code, email addresses, URLs, and user input in their actual form. Do not change punctuation or add spaces inside them.

## Dynamic text and localization

- Check missing values and changes in quantity: No files, 1 file, and 12 files. Avoid null values, negative remaining counts, and mismatched units or plural forms.
- Use complete messages or the existing localization placeholders. Preserve variable names and meaning when changing surrounding text; do not hard-code dynamic content.
- Translate the action rather than individual words. Done may close a view, finish a flow, or save an edit; choose the label from that behavior.
- Follow the target language's grammar, number formats, punctuation, and forms of address. A word-count or capitalization rule from one language does not automatically transfer to another.

## Length and actual presentation

There is no universal button word limit. Make the meaning complete first, then check readability in the real layout. With long names, filenames, or translated content, do not truncate the part needed to identify the object.

If only text or a screenshot is available, offer readability guidance and state that actual wrapping, target size, and screen-reader behavior were not checked. String length in source code does not prove the result on a device.
