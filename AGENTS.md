# Agent entry — Simundis client distribution

## Identity and read order

This is **`bouncemonster/simundis-pack`**, a client-distribution repository. Its own current GitHub default branch is the source of truth for this published pack. It is not the Minecraft runtime, the platform backend, a launcher implementation or a replacement for another Simundis repository.

Read the [maintained entrance](.github/README.md), the [generated publication notice](README.md) and [sync manifest](schema.json). The repository currently distributes `Simundis.mrpack`, `schema.json` and `basics.zip`; it has no application package manifest or declared npm test/build command.

## Preserve generated artifacts

The root README identifies the publication generator. Do not hand-edit a generated pack, manifest or publication notice to introduce a new version. Locate the actual source publisher and review its current GitHub version before changing distribution behavior. Keep pack, manifest and companion outputs consistent through the owning publication process.

The manually maintained `.github/README.md` and this agent entry are not generated pack contents. Check that the publisher preserves them before a distribution refresh. Do not repair this by replacing the publisher or pushing an older local directory over GitHub.

A common project name does not establish compatibility. Read the game and loader requirements from the actual pack and manifest. Do not infer them from another repository's README or mix Fabric and NeoForge distributions without a verified compatibility contract.

## Resume without overwriting work

Read the latest relevant issue or handoff and inspect the branch, current GitHub revision, local modifications and recent commits. Local launcher instances and installed mods are runtime state, not automatically newer source.

Use one bounded task and explicit file ownership. Another agent or publisher may still be active after its conversation stops. Never force-push, reset, clean, stash another worker's changes, merge sibling projects or create worktrees as a documentation shortcut.

## Verification and demonstration

For a documentation edit, validate links from the containing Markdown directory, inspect any embedded image and confirm that generated artifact blob hashes remain unchanged. An absent application test suite is not a passing test suite.

For an authorized distribution change, validate JSON and archive integrity, pack/manifest consistency, exact game/loader requirements, dependency downloads and import into a separate launcher instance. Keep existing worlds and configurations untouched. Record the source revision, pack revision, launcher, operating system and exact result.

Do not present a successful JSON parse as proof that the game launches. A fixture, illustration, launcher import and successful server join are different evidence. Do not invent server addresses, access credentials or current compatibility claims.

## Handoff and publication

Use the existing task record, not a new parallel board. Before switching IDEs, record changed paths, publication commit and branch readback, checks with PASS / FAIL / NOT RUN / BLOCKED, any active or unobserved publisher, preserved local work and one next unfinished action.

All required contributor guidance must remain accessible in this public repository. Do not make private governance or the private shared documentation hub a mandatory onboarding dependency.

Preserve existing licenses and upstream mod notices. Repository maintenance does not grant game ownership or content rights, authorize a server deployment, or permit deleting local saves. Never publish account tokens or private player information.
