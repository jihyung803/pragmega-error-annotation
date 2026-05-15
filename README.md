# PragMega Error Taxonomy Annotation

This directory contains a static, browser-only blind annotation interface for
the PragMega error taxonomy validation subset.

## Files

- `index.html`: self-contained annotation UI.

The interface embeds the 40 blind error cases and does not include model
identity keys or OpenAI labels.

## How to Use

Open `index.html` in a browser, annotate each case, then click
`Export annotations CSV`.

Please send the exported CSV to the jihyung803@utexas.edu for agreement analysis.

## Annotation Labels

- `literal_surface_bias`: Anchors on literal wording or surface semantic
  compatibility when context calls for non-literal pragmatic interpretation.
- `missed_communicative_intent`: Fails to recover the speaker/listener's
  pragmatic goal, such as politeness, avoidance, deception, indirect request,
  complaint, or social positioning.
- `unsupported_or_overextended_inference`: Over-reasons from weak cues, invents
  assumptions not licensed by the prompt, or post-hoc rationalizes an incorrect
  answer.
- `coherence_bridge_error`: Misjudges whether an implicit causal, temporal, or
  discourse bridge between events is warranted.
- `figurative_or_humor_mapping_error`: Fails to map figurative language, jokes,
  punchlines, or humorous incongruity to the intended interpretation.
- `context_or_option_misread`: Misses a concrete fact, reference, option
  mapping, or answer extraction detail rather than pragmatic inference itself.

Use `unclear / cannot judge` if the output is too malformed or the case is too
ambiguous.
