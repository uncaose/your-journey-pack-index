# Your Journey — public pack index

Public catalog for Your Journey in English community content packs.

Catalog URL: https://raw.githubusercontent.com/uncaose/your-journey-pack-index/main/packs.json

## Current status

The catalog is operational and intentionally empty. No pack has completed the public licensing and quality publication gate yet. This does not remove the application’s bundled basic learning packs. No application source, personal data, recordings, credentials or model weights are hosted here.

In existing app builds, open the community pack catalog settings and enter the catalog URL above. Automatic default selection is pending application integration; creating this repository does not update installed apps.

## Add or update a pack

Submit a pull request editing `packs.json`. The root is a JSON array. Every entry has `id`, `name` (language-to-label object), `repo` (HTTPS Git repository URL), `tag` (semantic version), `levels`, `ui_langs`, `license`, `badges` (structure/rules/quality), `size` (bytes), and `updated` (ISO date). IDs are unique; maximum 1,000 entries / 1 MiB catalog / 50 MiB per pack.

Before merging, the maintainer runs the application’s shared yj-pack static validator, AI review and independent cross-review against the exact tagged pack. Confirm redistribution rights, content restrictions and the evidence behind every badge. Do not set a passing badge from an unverified author claim. Releases and installed learning progress must remain tied to stable item IDs.

## Operations

- Changes use pull requests and explicit maintainer approval. Never replace a published tag with different content.
- Report an unsafe pack through GitHub Issues, with pack ID and evidence. Avoid posting personal data.
- Remove a confirmed unsafe entry from the catalog; removal does not delete a user’s installed copy.
- Revert a bad catalog commit to restore the previous list.
- Scheduled daily scans, automated review, signed-off pack releases and catalog snapshots remain pending. No Actions workflow or paid AI service is enabled by this initial setup.
- A list can be served from another HTTPS host. Existing app catalog caches and bundled fallback continue to work during network failures.

Maintainer: GitHub account `uncaose`. This catalog does not establish a license for third-party packs; each pack must declare and substantiate its own license.
