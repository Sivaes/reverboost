# ReSkate Revert Boost

A small patch for [ReSkate](https://github.com/Dingo-Shenanigans/ReSkate) (GPL-3.0). Land an unfinished spin
(the game's auto revert) and gain forward speed; chain reverts to keep building it. Slider and toggle in
Insert > SKATER > BOOSTS. Off until you turn it on.

This repository holds only the patch (`patches/revert-boost.patch`), the files for the Thunderstore package
(`thunderstore/`) and the workflows that build it. ReSkate's source is fetched from the ReSkate project when
you build, so nothing of theirs is copied here.

## Build it
1. Actions > **Build Revert Boost** > Run workflow.
2. `upstream_ref`: a ReSkate release tag such as `v1.0.9` (or `main`). `mod_version`: this mod's version.
3. Leave **publish** off for a zip to test or send to a friend; download it from the run's Artifacts.
4. Tick **publish** to create a GitHub release whose launcher updates players automatically.

If the **Apply the patch** step fails, ReSkate changed a file the patch edits and the patch needs updating.

Not affiliated with EA, Full Circle or the ReSkate developers.
