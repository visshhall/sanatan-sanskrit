# SKT — Pending Tasks Tracker (Living Document)

| Field | Value |
|---|---|
| Project | SKT — Sanatan Sanskrit Learning App |
| Tracker version | 1.1 |
| Matches reference doc | SKT_REFERENCE.md v1.2 |
| Last updated | 14 November 2026 |

Status key: ⏳ Waiting on owner · 🔄 To do (Claude) · ✅ Done

---

## 1. Waiting on the owner
| # | Item | Ref |
|---|---|---|
| O7 | Create an **empty private repo** named `sanatan-sanskrit` on GitHub (no README, no licence, no .gitignore), then tell Claude. This Claude session cannot create new repos, but once the empty repo exists it can push to it. | REF header, D9 |

## 2. Phase 0 — remaining work (Claude)
| # | Task | Status |
|---|---|---|
| P0-1 | Sanskrit Wikisource: check whether accented Taittirīya Saṃhitā and Vājasaneyi Saṃhitā exist; record page licences (site rate-limited the first check) | 🔄 |
| P0-2 | Find a licence-clear accented **Atharvaveda Śaunaka** (TITUS restricted; check other copies) | 🔄 |
| P0-3 | Inspect GRETIL Sāmaveda file: accents present? licence header? | 🔄 |
| P0-4 | Choose digital sources for Griffith (SV, White YV, AV), Keith (Black YV), Whitney (AV); record licence of each digital copy | 🔄 |
| P0-5 | Confirm Pt. Jaidev Sharma's death year → copyright status of his Hindi bhāṣya | ⏸ Parked (Hindi later) |
| P0-6 | Hindi sources: parked (D5: English first). Revisit before the Hindi layer; Satwalekar is public domain from 1 Jan 2029 | ⏸ Parked |
| P0-7 | Draft permission-request emails to TITUS and sanskritdocuments.org (Yajurveda / Atharvaveda gap). Owner sends them; Claude does not send anything. Hindi publishers later. | 🔄 |
| P0-8 | Confirm DCS licence at source | 🔄 (can wait for Phase 2) |
| P0-9 | Push docs to `sanatan-sanskrit` (local repo with first commit is ready) | ⏳ (after O7) |
| P0-10 | Phase 0 sign-off: all Layer 1 sources ✅ or consciously deferred | 🔄 |

## 3. Later phases (parked, not started)
| # | Task | Phase |
|---|---|---|
| L0 | **Phase 1a:** design proposal (verse-screen mock-ups and the animations in REF §5.1) for owner approval before any code | 1a |
| L1 | Font rendering test: Noto Serif Devanagari vs Tiro Devanagari Sanskrit vs Shobhika on real svara text | 1 |
| L2 | Accented Devanagari padapāṭha source | 1 |
| L3 | Metre (chandas) and ṛṣi data from a sourced anukramaṇī index | 1 |
| L4 | Layer 2 (Upaniṣads) licence research, then review sample | Before Layer 2 |
| L5 | Layer 3–5 licence research (incl. BORI critical editions, Gita Press) | Before each layer |

## 4. KB ideas log
*(Ideas prefixed "KB idea:" in the SKT chat are copied here for the Knowledge Bank project. No KB work is done from SKT.)*

| Date | Idea |
|---|---|
| — | None yet |

## 5. Done
| Date | Item |
|---|---|
| 14 Nov 2026 | Open Decisions D1–D3 answered and recorded |
| 14 Nov 2026 | Licence register v1 built from source headers (VedaWeb, GRETIL, Monier-Williams, Vidyut, fonts) |
| 14 Nov 2026 | Content review sample 01 (Ṛgveda 1.1.1) prepared |
| 14 Nov 2026 | Decisions D4–D9 recorded (personal/free forever; English first; Griffith; sample accepted; Electron .exe; repo approved) |
| 14 Nov 2026 | Animated/interactive requirement captured (REF §5.1) |
| 14 Nov 2026 | Local git repo initialised with docs (first commit) |
