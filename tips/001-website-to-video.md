# Website-to-Video Prompt Playbook

Turn a website into a polished HyperFrames promotional video, create
reference-inspired variants, refine the result, localize the narration, and
deliver downloadable renders.

[Watch the Instagram demo](https://www.instagram.com/p/DbD9YR6SDPt/).

Replace every `[PLACEHOLDER]` before using a prompt.

## Recommended Workflow

1. Capture the website and define its visual identity.
2. Write the script and storyboard before building scenes.
3. Create and preview the first video.
4. Inspect the complete timeline and refine it.
5. Build separate reference-inspired variants when needed.
6. Validate and render every approved version.
7. Create localized versions as separate projects.
8. Verify and deliver the final files.

## 1. Create a Video From a Website

```text
Use the HyperFrames website-to-video workflow to capture [WEBSITE_URL] and
create a cinematic [WIDTH]×[HEIGHT], [FPS] fps promotional video lasting
approximately [DURATION] seconds.

Study the website before designing. Preserve its real logo, brand colors,
typography, product imagery, interface details, and overall personality.
Do not replace distinctive brand elements with generic SaaS visuals.

Create the following planning files before building the video:

- DESIGN.md — colors, typography, visual rules, motion direction, and
  anti-patterns.
- SCRIPT.md — concise narration written for the target duration.
- STORYBOARD.md — narrative beats, scene timing, assets, transitions, and
  audio direction.

Structure the video around [NUMBER_OF_SCENES] clear narrative beats:

1. [BEAT_1]
2. [BEAT_2]
3. [BEAT_3]
4. [BEAT_4]

Use a clear hero frame for every scene, purposeful entrance animations, and a
designed transition between scenes. Avoid jump cuts, generic templates,
unreadably dense text, and accidental overlaps.

After implementation, run HyperFrames linting, validation, contrast checks,
and timeline layout inspection. Resolve all errors and unintended overlaps.
Render a high-quality MP4 and provide both the preview URL and file path.
```

## 2. Open the Project in the Side Browser

```text
Start the HyperFrames preview server on an available localhost port and open
[PROJECT_NAME] in the in-app side browser.

Verify that the latest source changes are visible, the timeline plays from
beginning to end, and the narration is audible. Keep the downloadable render
available separately from the interactive preview.
```

## 3. Review and Refine the Entire Video

```text
Review the current render from beginning to end rather than editing only the
currently visible frame.

Fix all unintended text, card, image, and transition overlaps. Give each major
element a clear visual zone and preserve only intentional decorative layering.
Remove clutter, simplify competing motion, and increase breathing room where
the composition feels crowded.

Adjust the narration to [VOICE_DIRECTION] at approximately [VOICE_SPEED].
If the audio duration changes, retime the scenes and transitions so the spoken
ideas, visual reveals, proof points, and CTA remain synchronized.

Preserve [ELEMENTS_OR_VERSIONS_TO_KEEP].

After editing, rerun layout and contrast checks and render a new version without
overwriting the last approved MP4.
```

## 4. Use a Reference Video Safely

```text
Use [REFERENCE_VIDEO_URL] as a creative reference for a separate version of
[PROJECT_NAME].

Analyze the reference's:

- Pacing and scene rhythm
- Transition language
- Typography behavior
- Framing and camera movement
- Interface density
- Texture, lighting, and color treatment
- Relationship between sound and motion

Reinterpret those high-level qualities using the source website's content and
brand assets. Do not reproduce third-party branding, text, logos, footage,
music, illustrations, or proprietary graphics.

Describe the specific traits you are borrowing in the storyboard. Create this
as a separate project named [NEW_PROJECT_NAME] and keep all existing versions
unchanged.

Validate, preview, and render the result as a standalone MP4.
```

## 5. Create Multiple Reference-Inspired Concepts

```text
Create [NUMBER_OF_VARIANTS] distinct video concepts for [WEBSITE_URL].

Each concept should preserve the same brand, core message, proof points, and
CTA, but explore a different motion system:

1. [CONCEPT_1_DIRECTION]
2. [CONCEPT_2_DIRECTION]
3. [CONCEPT_3_DIRECTION]

Do not make the variants simple color swaps. Give each one a distinct scene
structure, typography rhythm, transition language, and visual metaphor.

Build every concept in a separate project directory. Preserve the original
version, validate every project independently, and render each approved concept
to its own MP4.
```

## 6. Render and Deliver the Final Videos

```text
Render the approved projects as high-quality [WIDTH]×[HEIGHT], [FPS] fps MP4
files using H.264 video and AAC audio.

For every output, verify:

- The file exists and opens successfully
- Duration
- Resolution
- Frame rate
- Video codec
- Audio codec, sample rate, and channel count
- File size
- Narration is present and synchronized
- The final frame holds long enough to read

Do not overwrite previously approved renders. Use clear filenames that include
the concept or language name.

Provide a direct download link and a HyperFrames preview URL for every video.
```

## 7. Compare Voiceover Providers

```text
I want to localize this video into [LANGUAGE] using [DIALECT_OR_LOCALE].

Compare the available text-to-speech providers for:

- Natural pronunciation
- Dialect and accent control
- Emotional range
- Speaking-rate control
- Brand-name and acronym pronunciation
- Voice cloning, if relevant
- Commercial usage rights
- Pricing
- API and production-workflow integration

Recommend the best option for a [CONTENT_TYPE] lasting approximately
[DURATION]. Keep script localization separate from speech generation, and
identify any licensing or disclosure requirements that need confirmation.
```

## 8. Localize the Narration

```text
Create a separate [LANGUAGE] version of [PROJECT_NAME] using
[DIALECT_OR_LOCALE].

Localize the meaning, persuasive structure, and brand tone rather than
translating word for word. Keep all key claims accurate. Shorten or restructure
sentences when necessary so the voiceover fits approximately [DURATION] without
sounding rushed.

Voice direction:

- Gender: [VOICE_GENDER]
- Register: [VOICE_REGISTER]
- Emotion: [VOICE_EMOTION]
- Pace: [VOICE_PACE]
- Accent or locale: [DIALECT_OR_LOCALE]

Add pronunciation guidance for:

- [BRAND_NAME]
- [ACRONYM_1]
- [ACRONYM_2]
- [TECHNICAL_TERM]

Preserve the original-language project. Generate the localized version in a
new directory named [LOCALIZED_PROJECT_NAME].

Measure the new narration duration, then retime scene boundaries, proof-point
reveals, transitions, and the final CTA to the localized audio. Validate and
render the localized project independently.
```

## 9. Authorize an External Speech Service

Use this only after reviewing the final script and the provider's terms.

```text
I approve sending only the finalized [LANGUAGE] narration text to
[SPEECH_PROVIDER] for text-to-speech generation.

Do not transmit project files, source media, captured website assets, private
documents, credentials, or unrelated text.

Generate a [VOICE_GENDER] voice with [VOICE_DIRECTION]. Save the audio inside
[LOCALIZED_PROJECT_NAME], verify its duration, and integrate it into the
localized video.
```

Never paste API keys or other credentials into a chat prompt. Configure them
through the local environment or an approved secrets interface.

## 10. Request a Specific Revision

```text
Review the complete current render and change only the items below:

1. Timestamp or scene: [TIMESTAMP_OR_SCENE]
2. Current problem: [PROBLEM]
3. Desired result: [DESIRED_RESULT]
4. Voice change: [VOICE_CHANGE_OR_NONE]
5. Timing target: [TIMING_TARGET]
6. Preserve unchanged: [ELEMENTS_TO_PRESERVE]

Check the surrounding scenes so the revision does not create new collisions,
abrupt transitions, timing gaps, or audio mismatches.

After editing, rerun layout and contrast checks, render a new version without
overwriting the previous approved file, and provide the preview and download
links.
```

## Complete End-to-End Prompt

```text
Use the HyperFrames website-to-video workflow to capture [WEBSITE_URL] and
produce a cinematic [WIDTH]×[HEIGHT], [FPS] fps promotional video lasting
[DURATION].

Preserve the website's real logo, colors, typography, product imagery,
interface details, and brand personality. First create DESIGN.md, SCRIPT.md,
and STORYBOARD.md. Build the narrative around [NUMBER_OF_SCENES] clear beats:
[LIST_THE_BEATS].

Use [VOICE_DIRECTION] narration. Give each scene a clear hero frame, purposeful
entrance animations, and a designed transition. Avoid generic SaaS visuals,
accidental overlaps, jump cuts, excessive text, conflicting animation, and
unreadable layouts.

If reference videos are supplied, analyze their pacing, motion language,
typography rhythm, framing, and texture. Reinterpret those qualities with the
source website's assets. Do not copy third-party branding, text, footage,
logos, music, or proprietary graphics. Create every reference-inspired
treatment as a separate project and preserve all earlier versions.

Run HyperFrames linting, validation, contrast checks, and timeline layout
inspection. Resolve all errors and unintended overlaps. Render a high-quality
H.264/AAC MP4 and verify its duration, resolution, frame rate, video stream,
audio stream, and file size. Start a localhost preview on an available port and
provide links to both the preview and rendered file.

Then create a separate [LANGUAGE] localization using [DIALECT_OR_LOCALE].
Adapt the marketing meaning instead of translating literally. Use
[LOCALIZED_VOICE_DIRECTION], keep the runtime near [LOCALIZED_DURATION], and
retime scenes and the CTA to the localized speech. Do not modify the original
project. Before using an external speech service, state exactly what will be
transmitted and obtain approval.
```
