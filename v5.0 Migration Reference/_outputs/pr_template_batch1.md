# PR: Migrate Core System Prompt to Suno v5

## Summary
Introduces the new Suno v5 system prompt, establishing concise high-signal prompting, reliable exclusion/negative control, and stem-driven iterative workflow. Legacy v4.5 system prompt is bannered (not deleted) for historical traceability.

## Files Changed
| File | Action | Notes |
|------|--------|-------|
| Knowledge/v5.0/01_Core_Knowledge/00_00_AI_Assistant_System_Prompt.md | Add | New authoritative v5 system prompt |
| Knowledge/v4.5/01_Core_Knowledge/00_00_AI_Assistant_System_Prompt.md | Modify | Legacy banner only |
| Knowledge/v5.0/_quality/report.md | Update | Added QA entry |
| v5.0 Migration Reference/_outputs/migration_change_log.md | Add | Logged migration actions |

## Canonical Facts Referenced
v5_global_migration_rules, v5_exclusion_guidance, v5_tagging_markup, v5_prompt_grammar, v5_editing_best_practices, v5_troubleshooting_framework, v5_paradigm_shift, v5_negative_prompting, v5_boomy_bass_fix, v5_stems_mixing, v5_three_layers_control.

## Verification
- Structural QA: PASS
- Regex scan (manual review) for residual legacy tokens: PASS
- Fact mapping: PASS
- Clarity & brevity: PASS

## Rationale
Reduces cognitive load in prompting; aligns assistant persona with v5 obedience & exclusion reliability; establishes iterative stems-first edit culture.

## Follow-Up (Next Batch Plan)
1. 10_10_Core_Principles.md (update → v5)
2. 20_20_Prompt_Syntax_Guide.md (split legacy + new v5 syntax)
3. AI Instructions_ Suno AI v4.5_ Songwriting Co-Pilot.md (convert to v5 Assistant Operations Guide)
