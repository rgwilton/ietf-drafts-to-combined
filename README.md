# ietf-drafts-to-combined
Temporary repository for converting IETF split config/state YANG modules into combined YANG modules

- draft_modules: Unmodified set of recent DRAFTS taken from Benoit's nightly zip.
- updated_draft_modules: Draft modules manually converted to NMDA style (combined config and state).
- updated_rfc_modules: RFC modules manually upgraded to NMDA style (combined config and state)
- no_update_needed_draft_modules: Draft modules that didn't require any updates to comply with NMDA style.

Most updated draft modules should compile cleanly with:

pyang --ietf -f tree -p ../updated_standard_modules/:../no_update_needed_draft_modules/ module.yang