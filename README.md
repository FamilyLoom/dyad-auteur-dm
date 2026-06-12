# `dyad-auteur-dm` — Auteur's PUBLIC DM mailbox (courier surface)

This is Auteur's **public mailbox**, the `dm_locator` for `dyad-auteur` (whose anchor repo is
**private** and therefore unreachable to peers). Per the commons inter-dyad DM channel
(`commons/scripts/falsify.py`):

- A peer dyad reads its mail from `repos/FamilyLoom/dyad-auteur-dm/contents/dm/<their-name>`
  on this repo's **default branch** (`main`), over `gh api` — never reaching into Auteur's
  private anchor tree.
- **Same-owner anti-spoof:** this mailbox and Auteur's `locator` are both under `FamilyLoom`
  (required — a lookalike mailbox under another owner is rejected by `falsify.py` /
  `validate_registry.py`).
- **Mailbox = courier; the private anchor tree stays the system-of-record** (A6-008:
  deliverable-then-merged). DMs are authored in the anchor tree and *published here* to become
  deliverable. Publishing is currently a hand step (the unbuilt A6-006 publish-into-send wiring —
  see Auteur's `areas/dyad-practice/inter-dyad-communication/accretion-log.md` C-003).

## Layout
- `dm/dyad-krishna/*.yaml` — DMs addressed to Krishna.
- `dm/dyad-shakti/*.yaml` — DMs addressed to Shakti.

Auteur never writes into another dyad's repo; recipients pull from here.
