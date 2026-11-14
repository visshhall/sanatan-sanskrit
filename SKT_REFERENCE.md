# SKT — Sanatan Sanskrit Learning App
## Reference Document (Living Document)

| Field | Value |
|---|---|
| Project code | **SKT** |
| Sister project | **KB** — Knowledge Bank app (separate chat, separate repo, never mixed) |
| Current version | SKT v0.0 — Phase 0 (sources & licensing) in progress, no code written yet |
| Document version | 1.2 |
| Last updated | 14 November 2026 |
| Owner | Vishal Singh |
| Repository | `sanatan-sanskrit` (private GitHub), approved by owner. Must be created on GitHub by the owner (this Claude session cannot create new repos); local repo with docs is ready to push |

> **How to use this document in a new chat:** Upload this file and SKT_PENDING.md at the start of the SKT chat and say: *"This is the SKT reference document. Read it fully, then continue from SKT_PENDING.md."* Everything needed to continue is in here.

---

## 1. Why this project exists (origin)

- The owner wanted a single app containing the **four Vedas, the Upanishads and everything related to Sanātana Dharma texts**, together with the ability to **learn Sanskrit** from them.
- He searched for existing apps that could **show and do all of this**, and never found a proper one. Existing apps are typically partial: one text only, no word-level meaning, poor Devanagari/Vedic accent rendering, unverified content, or ads and clutter.
- This app is being built to fill that gap: **one trustworthy, complete, respectful home for the scriptures, with real Sanskrit learning built in.**
- The idea emerged on 14 November 2026 during a brainstorm for brand-new personal projects (separate from the Ākāra business, LumenSutra, the Cosmic Odyssey game and the stock-market app).

## 2. What the app is (one paragraph)

A scripture library and Sanskrit learning app. Every verse is shown in its original Devanagari (with correct Vedic accent marks where they apply), with transliteration, word-by-word meaning, grammar, and sourced translations in **English and Hindi**. On top of the library sits a learning layer: a structured Sanskrit course, daily verse, memorisation and recitation practice, and progress tracking. It also has powerful search across the entire corpus. It is a **Windows desktop app** (installable `.exe`) that works fully offline. It is **animated and interactive**, not a page of plain text, so that reading the scriptures and learning Sanskrit feels alive and rewarding. It is **personal and free forever**: never sold, no ads.

## 3. Guiding principles (non-negotiable)

1. **Authenticity over volume.** Every text comes from verified, scholarly digital editions. Nothing is AI-generated and presented as scripture.
2. **Source on every verse.** Each verse and each translation shows where it came from.
3. **Respect.** The content is sacred to the owner. Presentation must be dignified: no cartoonish visuals, no gimmicks, no ads. Animation is welcome and expected (see §5.1), but it must serve the text: calm, purposeful motion that never distracts from or trivialises a verse.
4. **Owner review before content goes in.** Before each content layer is added, a sample is shown to the owner for review (same process used for deity iconography in the Cosmic Odyssey project).
5. **Honesty about limits.** Where something cannot be done properly (e.g. synthetic voice for Vedic svaras), we say so instead of faking it.
6. **Licensing respected.** Original Sanskrit texts are ancient and free, but many modern translations **and many digital editions** are copyrighted or licensed. Only public-domain or properly licensed material is used, and its licence is recorded in §4.2 before import.
7. **No empty slots filled by guesswork.** If a translation or data field has no confirmed source, the app shows it as missing rather than inventing it. *(Added in v1.1.)*

## 4. Content scope (built in layers, in this order)

| Layer | Content | Notes |
|---|---|---|
| 1 | **Four Vedas**: Ṛgveda, Yajurveda (Śukla and Kṛṣṇa), Sāmaveda, Atharvaveda | Include svara (accent) marks and padapāṭha (word-split text) where available |
| 2 | **Upaniṣads**: principal Upaniṣads first, then the full 108 (Muktikā canon) | |
| 3 | **Bhagavad Gītā, Vālmīki Rāmāyaṇa, Mahābhārata** | Mahābhārata is very large (~100,000 verses), so it is imported in parts |
| 4 | **18 Purāṇas, stotras, Sūtras, Vedāṅgas** | |
| 5 | **Monier-Williams Sanskrit–English dictionary** integrated | Powers tap-a-word meaning |

### 4.1 How licences were checked (Phase 0 method)
- Licences were read from the **source files themselves** (TEI headers, dictionary headers, repository metadata) wherever possible, not from third-party summaries.
- Copyright term used for translations: **India — author's lifetime + 60 years, counted from 1 January of the year after death** (Copyright Act 1957, s.22). A translation is a separate work from the ancient text.
- **Important:** an old translation can be public domain while the **digital edition** of it carries its own licence (e.g. Griffith's 1890 text is free, but the VedaWeb digitisation is CC BY-NC-SA 4.0). The register records both.
- Claude is not a lawyer. This register is careful research, not legal advice.

### 4.2 Licence register

**Status key:** ✅ Verified and usable · 🟡 Usable once a stated check is done · 🔴 Not usable without written permission · ⏳ Not yet researched (later layer)

#### A. Sanskrit texts

| # | Source | What it has | Licence (as stated in source) | Checked on | Status |
|---|---|---|---|---|---|
| S1 | **VedaWeb** (University of Cologne), repo `VedaWebProject/vedaweb-data` | Ṛgveda complete: accented Devanagari (Eichler), accented IAST (van Nooten & Holland), padapāṭha (Latin, unaccented), metrically restored text | **CC BY-NC-SA 4.0** for each text version (read from `vedaweb_corpus.tei` header) | 14 Nov 2026 | ✅ **Primary Ṛgveda source** |
| S2 | VedaWeb, University of Zurich annotation | Word-level stem + grammar for every Ṛgveda word | **CC BY 4.0** | 14 Nov 2026 | ✅ Powers the word table for Ṛgveda |
| S3 | **GRETIL** (Göttingen) | RV, RV padapāṭha, RV Khilāni, Atharvaveda Paippalāda, Sāmaveda (Kauthuma, input A. Pandey), principal Upaniṣads, epics, Purāṇas | TEI files carry **CC BY-NC-SA 4.0**, plus a "provided in good faith" note (confirmed in a sample GRETIL TEI file) | 14 Nov 2026 | 🟡 Check the header of **each file** at import |
| S4 | **TITUS** (Frankfurt) | Accented Atharvaveda Śaunaka, Taittirīya Saṃhitā, Vājasaneyi Saṃhitā, Maitrāyaṇī, Kāṭhaka | GRETIL describes these as "restricted download / proprietary format" | 14 Nov 2026 | 🔴 Needs permission |
| S5 | **Sanskrit Wikisource** | Taittirīya Saṃhitā (an unaccented "विस्वरः" version found), RV padapāṭha in Devanagari; accented Yajurveda still to be checked | Wikimedia standard: **CC BY-SA 4.0 + GFDL** | 14 Nov 2026 (partial, site rate-limited) | 🟡 Check accents and page licences in the next Phase 0 session |
| S6 | **sanskritdocuments.org** | Many accented texts (Taittirīya material, Upaniṣads, sūktas) | "For personal study and research… not to be copied or reposted… or for commercial purpose **without permission**" | 14 Nov 2026 | 🔴 Needs written permission to bundle |
| S7 | **Ambuda** (`ambuda-org/texts`) | Curated GRETIL texts, rare Upaniṣads (Adyar manuscripts) | Per-text licence in each TEI header; project aims for CC0 | 14 Nov 2026 | 🟡 Check per text |

**Gap found: the Yajurveda.** No source has yet been confirmed that is both accented and licence-clear for the **Taittirīya Saṃhitā** (Kṛṣṇa) or the **Vājasaneyi Saṃhitā** (Śukla). GRETIL only points to TITUS (restricted). Next steps are in SKT_PENDING.md (Wikisource check; permission requests to TITUS and sanskritdocuments.org). The accented **Atharvaveda Śaunaka** has the same problem.

#### B. English translations

| # | Translation | Translator died | Text status (India) | Digital edition | Status |
|---|---|---|---|---|---|
| E1 | Ṛgveda: R. T. H. Griffith (1890 ed.) | 1906 | Public domain | VedaWeb, CC BY-NC-SA 4.0 | ✅ **Main English RV (D6 approved)** |
| E2 | Ṛgveda (selected hymns): H. Oldenberg, SBE 46 (1897) | 1920 | Public domain | VedaWeb, CC BY-NC-SA 4.0 | ✅ Optional second translation |
| E3 | Ṛgveda (selected hymns): Max Müller, Macdonell | 1900 / 1930 | Public domain | VedaWeb, CC BY-NC-SA 4.0 | ✅ Optional |
| E0 | Ṛgveda: S. W. Jamison & J. P. Brereton (OUP, 2014), the modern scholarly standard | Living authors | **Copyrighted** | — | 🔴 Not usable. Recorded so the choice of Griffith is understood: it is the best **complete, usable** English Ṛgveda, not the most modern one. |
| E4 | Sāmaveda, White Yajurveda, Atharvaveda: Griffith | 1906 | Public domain | Source of digital text still to be chosen | 🟡 |
| E5 | Black Yajurveda (Taittirīya): A. B. Keith (1914) | 1944 | Public domain | Still to be chosen | 🟡 |
| E6 | Atharvaveda: W. D. Whitney, revised by C. R. Lanman (1905) | 1894 / 1941 | Public domain | Still to be chosen | 🟡 |
| E7 | Upaniṣads: Max Müller, SBE 1 & 15 | 1900 | Public domain | Still to be chosen | 🟡 (Layer 2) |

#### C. Hindi translations (the hard part)

| # | Translation | Coverage | Text status (India) | Status |
|---|---|---|---|---|
| H1 | **Swami Dayananda Saraswati**, Veda-bhāṣya (Sanskrit + Hindi) | Ṛgveda **partial** (stops in Maṇḍala 7); Yajurveda (Mādhyandina) full; no Sāma or Atharva | Public domain (died 1883) | 🟡 Text is free. Best digital copy (vedicscriptures.in, Aryasamaj Chennai) is login-only with no stated licence, so it **needs permission** or a different digital copy. **Interpretation note:** Arya Samaj reading (e.g. Agni often read as the Supreme Being), which differs from the traditional Sāyaṇa line. |
| H2 | **Pt. S. D. Satwalekar**, Subodh Bhāṣya (Hindi) | All four Vedas | Copyrighted **until 31 Dec 2028**; public domain from **1 Jan 2029** (died 31 July 1968) | 🔴 now · ✅ from 2029 |
| H3 | Pt. Shriram Sharma Acharya (Gayatri Pariwar) | All four Vedas, 108 Upaniṣads | Copyrighted (died 1990) | 🔴 Needs permission from Gayatri Pariwar |
| H4 | Pt. Jaidev Sharma (Hindi bhāṣya, all four Vedas) | All four Vedas | Death year **not yet confirmed**, so status unknown | ⏳ Research |
| H5 | Gita Press Hindi editions | Gītā, Rāmāyaṇa, Mahābhārata, Purāṇas, Upaniṣads | Copyrighted | 🔴 Needs permission (Layer 2+) |

**Honest summary:** there is **no Hindi translation of the four Vedas today that is complete, licence-clear and already digitised.**
**Owner decision (D5):** launch with **English first**; add Hindi later as licence-clear sources become available (Satwalekar enters the public domain on 1 Jan 2029; permission requests can run in parallel). Until then, the Hindi slot shows as "not yet available", never filled by guesswork (principle 7).

#### D. Dictionary, language tools and fonts

| # | Resource | Use | Licence (as stated) | Status |
|---|---|---|---|---|
| D1 | **Monier-Williams 1899**, Cologne digital edition (© The Sanskrit Library & Thomas Malten) | Tap-a-word meanings | **CC BY-NC-SA 3.0** (read from `mwheader.xml`); credit must be shown "exactly as described" | ✅ |
| D2 | Digital Corpus of Sanskrit (DCS), Oliver Hellwig | Grammar data beyond the Ṛgveda (Phase 2) | CC BY 4.0 (per Ambuda's DCS mirror) | 🟡 Confirm at source in Phase 2 |
| D3 | **Vidyut** (Ambuda), Rust toolkit | Sandhi splitting, morphology, transliteration (Phase 2) | **MIT** (read from `Cargo.toml`) | ✅ |
| F1 | **Noto Serif Devanagari** | Main Devanagari font | SIL OFL 1.1; covers the Vedic Extensions block | ✅ Rendering test in Phase 1 |
| F2 | Tiro Devanagari Sanskrit | Alternative scholarly font | SIL OFL; extended with Vedic signs | ✅ Rendering test in Phase 1 |
| F3 | Shobhika (IIT Bombay) | Alternative scholarly font | SIL OFL 1.1 | ✅ Rendering test in Phase 1 |

### 4.3 What "NC" (Non-Commercial) means for SKT
Almost every high-quality source above (S1, S3, D1, and the digital English texts) is licensed **CC BY-NC-SA**. In practice:
- **BY**: the app must credit each source; the source label on every verse already does this.
- **NC**: the app (or any bundle containing these texts) **can never be sold, carry ads, or be used commercially.** This matches principle 3 (no ads), but it is a lifelong constraint.
- **SA**: if the text data is ever shared with others, it must be shared under the same licence.
- If SKT stays a **personal app**, or is only ever given away free, these sources are fine.
- **Owner decision (D4, 14 Nov 2026): SKT stays personal and free forever and will never be sold.** All NC sources are therefore usable.

## 5. Planned features

### 5.1 Presentation and interaction (owner requirement, 14 Nov 2026)
The owner does not want plain text in any language (Sanskrit, English or Hindi). Every screen should be animated and interactive so that reading holds attention and invites exploration. Design rules:
- Motion must **reveal meaning**, not decorate: every animation should teach something (structure, sound, meaning, connection).
- Calm and dignified (principle 3): smooth easing, no bouncing, flashing, confetti or cartoon effects on scripture.
- Every animation can be paused, and a "reduce motion" setting is provided for long study sessions.
- Animations must run smoothly offline on an ordinary Windows laptop.

Candidate ideas (to be shown as a design proposal for owner approval in Phase 1, before code):
1. **Verse unfolding**: a mantra appears pāda by pāda; the saṃhitā text then visibly separates into its padapāṭha words (sandhi "unjoining" shown as motion).
2. **Living svaras**: udātta / anudātta / svarita drawn as a gentle pitch line above the text that traces the recitation melody, syllable by syllable.
3. **Tap-a-word cards**: tapping a word lifts it out of the verse into a card with meaning, root, grammar, and other verses where it appears.
4. **Script morph**: switching Devanagari ⇄ IAST ⇄ other scripts animates letter by letter, so the correspondence between scripts is visible.
5. **Translation reveal**: English (later Hindi) slides in beside the Sanskrit, with each English phrase linked to the Sanskrit words it translates (highlight both on hover or tap).
6. **Alphabet course**: Devanagari letters drawn stroke by stroke; mouth-position diagrams for pronunciation.
7. **Context panels**: devatā, ṛṣi and chandas shown as small animated info panels; a map of a sūkta's verses as a navigable structure.
8. **Progress**: a calm visual (e.g. a mandala or lotus that fills in as texts are read) rather than points or badges.

### Reader
- Devanagari with correct Vedic accent rendering
- Switch script: Devanagari / IAST / Hindi and other Indian scripts
- Navigate by text → book/chapter → verse
- Source label on every verse and translation
- English and Hindi translations shown side by side or one at a time *(v1.1)*

### Meaning
- Tap any word → dictionary meaning + grammatical form
- Sandhi splitting (separating joined words)

### Learning
- Structured Sanskrit course: alphabet → pronunciation → grammar → reading real verses
- Daily verse
- Memorisation and recitation practice
- Progress tracker

### Search
- Search the whole corpus by word, topic or concept (e.g. "every mention of Agni", "verses on dharma")

### Audio
- Authentic human recitations where licensing allows
- **Limitation:** synthetic text-to-speech cannot render Vedic svaras correctly, so Vedic audio will never be faked with synthetic voice

## 6. Roadmap

| Phase | Name | What gets done | Status |
|---|---|---|---|
| 0 | Sources & licensing | Identify, verify and record the licence of every source; finalise platform and tech stack | **In progress.** Register v1 done; Yajurveda, Atharvaveda and Hindi gaps open |
| 1 | Reader | **Step 1a:** interaction and visual design proposal (mock-ups of the verse screen and the animations in §5.1) for owner approval. **Step 1b:** text display, scripts/transliteration, navigation, source labels, first animations | Not started |
| 2 | Meaning | Word-tap dictionary, grammar info, sandhi splitting | Not started |
| 3 | Learning | Sanskrit course, daily verse, memorisation, progress | Not started |
| 4 | Search | Full-corpus search by word/topic/concept | Not started |
| 5 | Audio | Licensed authentic recitations | Not started |
| — | Release | Windows installer (`.exe`) | Not started |

## 7. Decisions

### 7.1 Decided
| # | Decision | Answer | Date |
|---|---|---|---|
| D1 | Platform | **Windows desktop only** | 14 Nov 2026 |
| D2 | Translation language | **English and Hindi** | 14 Nov 2026 |
| D3 | Repository name | **`sanatan-sanskrit`** (private) | 14 Nov 2026 |

| D4 | Commercial use? | **Never.** Personal and free forever; never sold, no ads | 14 Nov 2026 |
| D5 | Hindi path for the Vedas | **English first; Hindi added later** as licence-clear sources become available | 14 Nov 2026 |
| D6 | Main English Ṛgveda | **Best usable translation**, owner has no specific preference → **Griffith** (complete), with Oldenberg / Müller / Macdonell as optional extras where they exist | 14 Nov 2026 |
| D7 | Content level per verse (sample 01) | Accepted, with the added requirement that it be presented **animated and interactive** (§5.1) | 14 Nov 2026 |
| D8 | Tech stack | **Electron**, packaged as a Windows `.exe` installer | 14 Nov 2026 |
| D9 | Repository | **Approved.** Private repo `sanatan-sanskrit` | 14 Nov 2026 |

### 7.2 Open (owner to answer)
| # | Question | Why it matters |
|---|---|---|
| — | None at the moment. The next decision will be the Phase 1 design proposal (§5.1). | |

## 8. Technical notes

- **Fully offline**: the entire text corpus is small (tens of MB); audio is the only large component.
- **Stack: Electron** (D8 approved), packaged as a Windows `.exe` installer. Chosen because the platform is Windows only (D1) and it matches the owner's other desktop apps. The animation library is chosen in Phase 1a and recorded here.
- Source data arrives as **TEI-XML** (VedaWeb, GRETIL, Ambuda) and plain text. Phase 1 will convert it once, at build time, into a local database bundled with the app. Every row keeps its source ID so the source label is automatic.
- **Vedic accents** use the Unicode Devanagari stress signs (U+0951 ॑, U+0952 ॒) and the Vedic Extensions block (U+1CD0–1CFF). Candidate fonts: Noto Serif Devanagari, Tiro Devanagari Sanskrit, Shobhika (all SIL OFL). Real rendering tests in Phase 1.
- Transliteration between scripts will be done by code (e.g. Vidyut or an equivalent library), never by AI.
- Known conversion detail: some sources write Vedic ḷ (ळ) as "l̥" or "ḷ"; the converter must map it to ळ, not ऌ. Found while building sample 01.

## 9. How we work on this project

- **Separate chat** for SKT only. Code name in messages: **SKT**.
- **Separate private GitHub repo.** Every version saved there.
- Living documents in the repo: **SKT_REFERENCE.md** (this file) and **SKT_PENDING.md** (task tracker), both updated after every change. Content review samples live in `samples/`.
- If an idea for the Knowledge Bank comes up in the SKT chat, prefix it **"KB idea:"**. It is logged in SKT_PENDING.md §4 for KB, and no KB code is touched from the SKT chat.
- Untagged, ambiguous requests → Claude asks which project before changing anything.
- When a chat gets long, Claude updates this document and the work continues in a fresh chat.

### Session routine
1. Read SKT_REFERENCE.md and SKT_PENDING.md
2. Confirm what this session will do
3. Build and test (real execution tests, not just syntax checks)
4. Update both documents, bump the version
5. Save to the SKT repo

## 10. Code commenting standard (mandatory, every file)

Every piece of code must be commented so that anyone can understand it without asking:

- **File header**: what this file is, why it exists, what it connects to (which files call it / which it calls), and when it runs.
- **Every function / component**: what it does, how it does it, why it is needed, when it is called, who calls it, what it calls, inputs, outputs, and side effects.
- **Inline comments**: on any line whose purpose or reasoning is not obvious.
- **Standalone code** is explicitly marked as "not connected to other modules."
- Comments are updated whenever the code changes; outdated comments count as bugs.
- Every code file is delivered complete: nothing missing, no "rest unchanged" placeholders.

## 11. Future goals

- Complete coverage of the major Sanātana texts in layers 1–5
- Become the "proper app" the owner could never find: trustworthy, complete, ad-free
- Full Hindi coverage of the Vedas as licences allow (Satwalekar enters the public domain on 1 Jan 2029)
- Further goals to be added as they are decided

## 12. Change log

| Date | Version | Change |
|---|---|---|
| 14 Nov 2026 | Doc 1.0 | Initial reference document created from the planning discussion. No code yet. |
| 14 Nov 2026 | Doc 1.1 | Decisions D1–D3 recorded (Windows only; English + Hindi; repo `sanatan-sanskrit`). Phase 0 started: licence register (§4.1–4.3) built from source headers; Yajurveda, Atharvaveda Śaunaka and Hindi gaps identified; principle 7 added; new open decisions D4–D9; tech notes updated (Electron proposed, fonts, ḷ mapping). Review sample 01 (Ṛgveda 1.1.1) created. No code yet. |
| 14 Nov 2026 | Doc 1.2 | Decisions D4–D9 recorded: personal and free forever (all NC sources usable); English first, Hindi later; Griffith as main English Ṛgveda (Jamison & Brereton noted as copyrighted); sample 01 content accepted; Electron with `.exe` installer; repo approved. New §5.1: animated, interactive presentation requirement with candidate ideas; principle 3 extended to cover dignified motion; Phase 1 split into 1a (design proposal) and 1b (build). Repo could not be created from this session, so a local repo is ready and the owner creates the empty GitHub repo. No code yet. |
