# Medium — Letter — throughline source

This document is **generated from the graph** by `tl docs`; `tl docs --check` gates
it in CI. The prose headings are hand-owned — everything between `tl:*` markers is
injected from the YAML items, so the published spec can never drift from the graph.

This source is the **medium axis** for one channel: a **letter**, posted or sent as a
PDF, read linearly on paper, with no links to click, no search and no scrolling, framed
by an address block, a salutation and a sign-off. It governs how delivery is *shaped
for that channel* — structure, length, navigation, framing and presentation — not
universal readability, spelling, punctuation, register, purpose or audience, each of
which is its own throughline source. Channels are mutually exclusive: **letter**,
**web**, **email**, **SMS** and **print** are sibling sources and a consumer composes
exactly one under the `medium` namespace. Every principle is a `user_requirement`;
every rule is a `system_requirement` that `implements` its principle. The throughline
UIDs are this source's own and immutable — a consumer cites a rule as `medium:SR-0001`.

It carries
<!-- tl:count type == 'user_requirement' -->
5
<!-- tl:end --> principles and
<!-- tl:count type == 'system_requirement' -->
10
<!-- tl:end --> rules.

## Purpose

<!-- tl:item INT-0001 -->
**INT-0001 — Text is delivered as a letter** — `intent`, status `approved`

> A letter, posted or sent as a PDF, is read linearly from top to bottom, on paper or a fixed page. The reader cannot click a link, search the text or scroll for more, so the letter must carry everything they need and frame itself with an address block, a salutation and a sign-off. This axis governs how delivery is shaped for that channel — structure, length, navigation, framing and presentation — not universal readability, spelling, register, purpose or audience, each of which is a separate source. Channels are mutually exclusive: a consumer composes exactly one of the web, letter, email, SMS or print sibling sources.

**source_ref**: TBS Medium — Letter
<!-- tl:end -->

## 1. Structure the letter as a linear read

<!-- tl:item UR-0001 -->
**UR-0001 — Structure the letter as a linear read** — `user_requirement`, status `approved`

> A letter is read straight through, so order it so each point follows from the last, from the reason for writing to what happens next.

*Derives from:* INT-0001

**source_ref**: TBS Medium — Letter — Structure for the channel
<!-- tl:end -->

<!-- tl:table attrs.get('principle') == 'UR-0001' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0001 | system_requirement | approved | Open with the reason for writing, then the detail, then what happens next |
| SR-0002 | system_requirement | approved | Do not rely on the reader jumping between sections |
<!-- tl:end -->

## 2. Keep the letter short and self-contained

<!-- tl:item UR-0002 -->
**UR-0002 — Keep the letter short and self-contained** — `user_requirement`, status `approved`

> The reader cannot click through for more, so keep the letter brief and make sure it holds everything they need.

*Derives from:* INT-0001

**source_ref**: TBS Medium — Letter — Length and density
<!-- tl:end -->

<!-- tl:table attrs.get('principle') == 'UR-0002' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0003 | system_requirement | approved | Keep the letter as short as the message allows |
| SR-0004 | system_requirement | approved | Include everything the reader needs within the letter |
<!-- tl:end -->

## 3. Point and prompt without anything to click

<!-- tl:item UR-0003 -->
**UR-0003 — Point and prompt without anything to click** — `user_requirement`, status `approved`

> There are no links or buttons, so write out addresses in full and state plainly what the reader must do.

*Derives from:* INT-0001

**source_ref**: TBS Medium — Letter — Navigation and actions
<!-- tl:end -->

<!-- tl:table attrs.get('principle') == 'UR-0003' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0005 | system_requirement | approved | Write addresses and references out in full for the reader to use |
| SR-0006 | system_requirement | approved | State plainly what the reader must do and by when |
<!-- tl:end -->

## 4. Frame the letter with its envelope

<!-- tl:item UR-0004 -->
**UR-0004 — Frame the letter with its envelope** — `user_requirement`, status `approved`

> A letter opens with an address block, date, reference and salutation, and closes with a sign-off; give it that framing.

*Derives from:* INT-0001

**source_ref**: TBS Medium — Letter — Opening and closing
<!-- tl:end -->

<!-- tl:table attrs.get('principle') == 'UR-0004' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0007 | system_requirement | approved | Open with the address block, date, reference and salutation |
| SR-0008 | system_requirement | approved | Close with a sign-off and the sender's name and role |
<!-- tl:end -->

## 5. Present for a fixed printed page

<!-- tl:item UR-0005 -->
**UR-0005 — Present for a fixed printed page** — `user_requirement`, status `approved`

> The letter may be printed in black and white, so keep the layout restrained and do not rely on colour or rich formatting.

*Derives from:* INT-0001

**source_ref**: TBS Medium — Letter — Presentation and formatting
<!-- tl:end -->

<!-- tl:table attrs.get('principle') == 'UR-0005' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0009 | system_requirement | approved | Make sure the letter still reads in black and white |
| SR-0010 | system_requirement | approved | Keep formatting restrained and suited to a letter |
<!-- tl:end -->
