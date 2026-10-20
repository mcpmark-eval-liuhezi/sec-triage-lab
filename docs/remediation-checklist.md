# Remediation Checklist — Critical Advisories (npm & pip)

One action item per advisory from `docs/advisory-notes.md`. Each item names the package and the minimum version to upgrade to.

- [ ] **GHSA-qx66-fv34-fjm8** (CVE-2026-102989, npm): Upgrade `@tanstack/start-server-core` to **1.169.39** or later. Sibling packages in the same advisory must also be upgraded: `@tanstack/react-start` to 1.168.60+, `@tanstack/solid-start` to 1.168.57+, `@tanstack/vue-start` to 1.168.56+.
- [ ] **GHSA-x34j-47hf-4xg7** (CVE-2026-108261, npm): Upgrade `tinacms` to **3.14.0** or later. The sibling package `@tinacms/app` must also be upgraded to 2.5.14+ if present.
- [ ] **GHSA-f8c7-rwf9-fmgm** (CVE-2026-111057, pip): Upgrade `mercury` to **3.2.4** or later.
- [ ] **GHSA-rv4m-xm3f-3ccq** (CVE-2026-111058, pip): Upgrade `mercury` to **3.2.6** or later (this supersedes the 3.2.4 fix — see GHSA-f8c7-rwf9-fmgm, whose fix was incomplete).
