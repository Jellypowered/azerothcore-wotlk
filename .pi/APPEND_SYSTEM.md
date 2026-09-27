# Repository Grounding

This project is AzerothCore-WotLK with local modules, custom changes, database
content, configuration, and branch-specific behavior.

Do not assume implementation details from pretrained knowledge of World of
Warcraft, WotLK, TrinityCore, AzerothCore, Playerbots, or similar projects.

Never use remembered WoW/WotLK behavior as a substitute for reading the
relevant local implementation when that implementation is available.

For claims about how this repository behaves:

- Inspect the actual checked-out source code, local module code, configuration,
  database/schema/data, DBC data, build files, or git history as appropriate.
- Prefer the current repository and its configured local data over remembered
  upstream or historical behavior.
- Verify APIs, enum values, spell IDs, lock types, database fields, call paths,
  and control flow from the local code/data before relying on them.
- Do not say "in WotLK", "AzerothCore does", "this normally means", or similar
  as evidence for how this checkout behaves.
- If a fact cannot be verified from the available repository or local data,
  explicitly mark it as unverified instead of filling the gap from memory.
- When local source contradicts pretrained knowledge, the local source wins.
- Before proposing a code change, trace the relevant local implementation far
  enough to establish that the proposed behavior matches this checkout.
- Before modifying files, read and follow the applicable rules in both
  `/stuff/Source/azerothcore-wotlk/.coderabbit.yaml` and
  `/stuff/Source/azerothcore-wotlk/modules/mod-playerbots/.coderabbit.yaml`.
  The repository-level rules apply throughout `azerothcore-wotlk`; the
  `mod-playerbots` rules apply additionally to files within that module.
  If the two contain conflicting instructions for `mod-playerbots`, the
  more specific module-level rule takes precedence. Non-conflicting rules
  from both files remain in effect.

  Grounding policy identifier: ACORE_JELLY_V1
