# Focalboard Fork Maintenance Notes

This repository is a fork of `mattermost-community/focalboard`.

The fork is maintained for safe downstream maintenance and future patches. It is not an upstream Mattermost release, and changes made here should not imply endorsement by Mattermost, Inc.

## Licensing Hygiene

- Preserve `LICENSE.txt`, `NOTICE.txt`, copyright headers, and upstream attribution.
- Do not describe this fork as MIT-only.
- Treat source builds, source-built binaries, and downstream modifications as subject to the upstream source license terms in `LICENSE.txt`.
- Mattermost-produced compiled versions may be covered by terms shipped with those compiled artifacts; that does not make this source fork MIT-only.
- Do not remove or weaken upstream license notices, dependency notices, trademark guidance, or attribution.
- If a future patch requires editing `LICENSE.txt`, `NOTICE.txt`, copyright headers, branding, trademarks, or similar sensitive material, stop and perform an explicit legal/maintainer review before making the change.

## Source Availability Reminder

Do not create releases, Docker images, hosted deployment instructions, or public distribution instructions from this fork unless the accompanying documentation includes source-code availability notes consistent with the upstream source license terms.

At minimum, public distribution or deployment notes should identify:

- the exact source branch, tag, or commit used;
- where recipients can obtain the corresponding source code;
- any local modifications or patches applied on top of upstream;
- the continued applicability of `LICENSE.txt` and `NOTICE.txt`.

## Patch Tracking

Fork-specific changes should be recorded in `CHANGES.md` under `Unreleased` until they are grouped for a downstream maintenance milestone.

For each future patch, record:

- the affected area;
- whether the patch changes source, build, packaging, deployment, or documentation behavior;
- any upstream issue, pull request, commit, or rationale;
- whether license, notice, copyright, or trademark-sensitive files were reviewed.

Keep upstream synchronization work separate from fork-specific maintenance patches when practical.
