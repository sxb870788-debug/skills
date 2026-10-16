# Selection, post-confirmation refinement, and rollback

## State and versioning

Stage order: color C → layout L → typography T → final appearance F. Alternative IDs use `C-R01-01`, with R for the candidate round. Revisions of a chosen option use `C-R01-01-V02`; increment V without overwriting previous images or confirmations. Identify reused versions and their upstream basis.

Record current stage, operation (initial exploration/chosen-option refinement/current-stage regeneration/return upstream/restore revision), base and revision IDs, preview/source paths, upstream versions, changes and retained decisions, feedback and verbatim confirmation, language/size scope, and status (candidate/selected awaiting confirmation/revision awaiting confirmation/confirmed/rejected/recheck or reconfirm needed). Preserve approval history, but never apply old approval to a new image. On resumption, read the record; assistant summaries are not approval.

## Selection and confirmation

1. Initially or when exploration is requested, render 3 meaningfully different alternatives by default. Follow a user-specified count, with at least 2 for alternatives.
2. Show IDs, actual previews, differences and concise tradeoffs. Recommendations do not select. Request personal selection and explicit confirmation; explain that refining the chosen option, regenerating, and returning upstream are available.
3. “Confirm L-R01-02” approves its uniquely identified version. “I like the second” only selects. A generic “okay” confirms only when the previous question uniquely identifies the version and scope.
4. Proceed after confirmation without an unnecessary second approval gate. The user may still refine this or an earlier confirmed option at any time. Confirmation approves a displayed version; it never permanently locks a design or waives further changes.

## Refine a confirmed option

For “confirm 2, but enlarge the headline”, “lighten the colors”, or “fine-tune this option”, use the selected/confirmed option as the base, apply changes, and present the revision first. Conditional confirmation never approves an unseen result or permits advancing before it is reviewed.

| Dimension | Adjustable elements | Retained basis |
| --- | --- | --- |
| Color | Background, primary/secondary/accent colors, area distribution, lightness and contrast | Original product colors, logo assets, exact copy and unaffected structure |
| Layout | Product/headline position and scale, reading hierarchy, whitespace, alignment and density | Approved palette and unaffected type rules; uniform product scaling |
| Typography | Font pairings, weights, sizes, line/letter spacing and language breaks | Approved colors and structure; show layout impacts from changed metrics |
| Final appearance | Background texture, lighting, decoration, shadows, edges and details | Approved palette, layout, type and original product/logo; return to an affected upstream stage when needed |

Normally render one actual revision plus a before/after comparison, identifying changes and retained elements. Do not force every small change back into three-option exploration. Provide revision branches when feedback has several reasonable interpretations or the user requests alternatives. Execute clear changes directly; clarify only necessary ambiguity about the target or scope.

Mark revisions awaiting confirmation, check affected factual, fidelity, readability and specification requirements, then present. Invite confirmation, further changes, restoration, or rollback. Each feedback triggers one round followed by a wait; keep refining while requested until the user explicitly confirms satisfaction, pauses or cancels. Old approval never transfers automatically to a revision. Do not advance dependent work or deliver an unconfirmed revision as final.

## Regenerate, return a stage, or restore a revision

| Intent or feedback | Action |
| --- | --- |
| “Redo” or “none are suitable”, without a return target | Regenerate alternatives at the current stage, retaining approved upstream choices. Do not restart the entire task. |
| “Go back one step” / “return to the previous stage” | Move one design stage in C → L → T → F: F→T, T→L, L→C. At color, return to palette generation rather than recollecting all inputs. Show the latest target-stage versions for refinement or exploration. |
| “Return to color/layout/typography” | Go directly to that stage and its selected base without asking at each intermediate stage. |
| Revision is disliked | Continue refining that base, or restore/regenerate/return as requested. Do not assume rejection abandons the whole design. |
| “Restore the previous version” | Restore the preceding revision of the current option; this differs from navigating to the preceding design stage. Identify the restored version and scope. If upstream choices changed, recheck and reconfirm. |
| Combine color A with layout B | Render a new combination ID and request confirmation of the actual result. |
| Request changes after final delivery | Open a revision branch from the specified delivered version and retain the old package. Verify and confirm the revision before saving a new delivery. |

Navigation alone does not change an approved image or invalidate all downstream decisions. An actual upstream change places its revision awaiting confirmation and lists affected downstream decisions; mark uncertain impacts for recheck. Color may affect text contrast and lighting; layout may affect line breaks and finishing; fonts may affect layout; finishing changes usually affect only finishing. Rerender, verify and reconfirm affected downstream previews. Retain unaffected choices and reuse suitable structure, fonts and decoration without forcing a full set of new alternatives. Never carry approval of an old-upstream finished image onto a changed image. Bind every confirmation to its actual version and language/size scope.

Honor requests limited to one language or size. Change only authorized scope and show necessary cross-version consistency checks. Exact copy, product shape/color and logo protections remain in force; aesthetic edits do not authorize factual rewriting or protected-asset redrawing.

Wait after each round. Silence, timeout and preselection are not consent. Stop generation and preserve progress on pause/stop/cancel. “Until satisfied” does not mean an unattended infinite loop or authorize execution beyond current tools, budget or time. If actual limits block continuation, identify limits and completed work and await a scope adjustment.

## Behavioral validation scenarios (pending execution)

- After color approval, “lighten the background”: render V02 from the chosen base, retain product colors, and await new confirmation.
- “Confirm 2, but enlarge the headline”: render the revision first; the unseen revision remains unapproved.
- At typography, “go back one step”: return to the chosen layout, allow refinement, and retain historical approvals until changes occur.
- At final review, “return to color”: go directly to color and recheck/reconfirm affected downstream previews after changes.
- Reject V03 and restore the previous version: show V02; restore its valid approval only if upstream context is unchanged, otherwise reconfirm.
- Change only English line spacing: retain Chinese and review English layout effects before confirmation.
- Soften shadows after delivery: retain the old package and confirm a new finishing revision before saving a new package.
- Silence or stop: never auto-approve or continue generating.

These are test inputs and expected behavior, not evidence of completed runs. Full poster trials, token/time comparisons and classmate trials require separate execution and records.
