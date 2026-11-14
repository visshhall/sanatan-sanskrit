# SKT — Pending Tasks Tracker (Living Document)

| Field | Value |
|---|---|
| Project | SKT — Sanatan Sanskrit Learning App |
| Tracker version | 1.3 |
| Matches reference doc | SKT_REFERENCE.md v1.3 |
| Last updated | 15 November 2026 |

Status key: ⏳ Waiting on owner · 🔄 To do (Claude) · ⏸ Parked · ✅ Done

---

## 1. Waiting on the owner
| # | Item | Ref |
|---|---|---|
| O8 | Optional: send the TITUS email (draft given in chat, to be saved here once approved). Not blocking. | P0-7 |
| O9 | Confirm you are happy to proceed to **Phase 0 sign-off**, then **Phase 1a (design proposal)** | REF §6 |

## 2. Phase 0 — remaining work (Claude)
| # | Task | Status |
|---|---|---|
| P0-1 | Yajurveda accented sources | ✅ Wikisource: Taittirīya (S8), Śukla (S9); caveat in REF §4.2 |
| P0-2 | Accented Atharvaveda Śaunaka | ✅ Wikisource (S10) |
| P0-3 | Sāmaveda | ✅ Wikisource Kauthuma, sāman notation (S11). GRETIL cross-check moved to Phase 1 (L6) |
| P0-4 | Digital copies of Griffith (SV, YV, AV), Keith, Whitney | ✅ archive.org scans identified (E4–E6). OCR clean-up and alignment moved to Layer 1 work (L7) |
| P0-5 | Jaidev Sharma copyright status | ⏸ Parked (Hindi later) |
| P0-6 | Hindi sources | ⏸ Parked. Revisit before the Hindi layer; Satwalekar is public domain from 1 Jan 2029 |
| P0-7 | Permission / provenance email to TITUS (optional); sanskritdocuments.org email no longer needed for Layer 1 | ⏳ Owner decides (O8) |
| P0-8 | Confirm DCS licence at source | 🔄 Can wait for Phase 2 |
| P0-9 | Push docs to `sanatan-sanskrit` | ✅ |
| P0-10 | Phase 0 sign-off | ⏳ After O9 |

## 3. Later phases (parked, not started)
| # | Task | Phase |
|---|---|---|
| L0 | **Phase 1a:** design proposal (verse-screen mock-ups and the animations in REF §5.1) for owner approval before any code | 1a |
| L1 | Font rendering test: Noto Serif Devanagari vs Tiro Devanagari Sanskrit vs Shobhika on real svara text | 1 |
| L2 | Accented Devanagari padapāṭha source | 1 |
| L6 | Cross-check a sample of each Wikisource Veda text against a second source (GRETIL / TITUS pages for reading); count mantras against known totals; verify Taittirīya 5–7 and Śukla chapters 2–40 | Before each Veda is imported |
| L7 | OCR clean-up and verse alignment of the English translation scans (Griffith, Keith, Whitney); map Griffith's Sāmaveda numbering to Kauthuma; show a sample for review before import | Before each Veda is imported |
| L8 | Visual rendering test of both accent systems (Vedic marks and sāman notation) in Noto Serif Devanagari and Tiro; check Shobhika release if wanted | 1 |
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
| 15 Nov 2026 | Phase 0 sources: accented Yajurveda, Atharvaveda, Sāmaveda found on Wikisource (provenance caveat recorded); translation scans found on archive.org; font coverage tested; v1.1/1.2 error about unaccented Taittirīya corrected |
| 14 Nov 2026 | Private repo `visshhall/sanatan-sanskrit` created by owner; Claude GitHub access granted; docs pushed to `main` |
