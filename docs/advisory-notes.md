# Advisory Notes — Critical Severity, npm & pip

Quarterly dependency-security review. The four advisories below are the two most recently published critical-severity advisories for each of the npm and pip ecosystems, as published in the GitHub Advisory Database at the time of this review.

| Ecosystem | GHSA id | CVE | Package | Severity | Vulnerable range | First patched version |
|---|---|---|---|---|---|---|
| npm | GHSA-qx66-fv34-fjm8 | CVE-2026-102989 | @tanstack/start-server-core | critical | >= 1.143.12, < 1.169.39 | 1.169.39 |
| npm | GHSA-x34j-47hf-4xg7 | CVE-2026-108261 | tinacms | critical | <= 3.13.0 | 3.14.0 |
| pip | GHSA-f8c7-rwf9-fmgm | CVE-2026-111057 | mercury | critical | >= 3.0.0, <= 3.2.3 | 3.2.4 |
| pip | GHSA-rv4m-xm3f-3ccq | CVE-2026-111058 | mercury | critical | <= 3.2.5 | 3.2.6 |

## Notes on multi-package advisories

Both npm advisories technically cover more than one package:

- **GHSA-qx66-fv34-fjm8** (TanStack Start): the advisory's primary/representative package is `@tanstack/start-server-core` (range `>= 1.143.12, < 1.169.39`, first patched `1.169.39`). Sibling packages are `@tanstack/react-start` (patched `1.168.60`), `@tanstack/solid-start` (patched `1.168.57`), and `@tanstack/vue-start` (patched `1.168.56`), all with vulnerable range `>= 1.143.12`.
- **GHSA-x34j-47hf-4xg7** (TinaCMS): the advisory's primary package is `tinacms` (range `<= 3.13.0`, first patched `3.14.0`); sibling package `@tinacms/app` is vulnerable `<= 2.5.13` with first patched `2.5.14`. The advisory notes the true lower bound is undetermined and the range is given as `<=` by the reporter.

## References

- https://github.com/advisories/GHSA-qx66-fv34-fjm8
- https://github.com/advisories/GHSA-x34j-47hf-4xg7
- https://github.com/advisories/GHSA-f8c7-rwf9-fmgm
- https://github.com/advisories/GHSA-rv4m-xm3f-3ccq
