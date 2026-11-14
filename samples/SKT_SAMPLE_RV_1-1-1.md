# SKT — Content Review Sample 01
## Ṛgveda 1.1.1 (Layer 1 — Four Vedas)

| Field | Value |
|---|---|
| Purpose | Owner review **before** any Layer 1 content is imported |
| Status | ✅ Accepted by owner, 14 Nov 2026 (to be presented animated and interactive; see REF §5.1) |
| Prepared | 14 November 2026 |
| Data pulled from | VedaWeb TEI dataset (University of Cologne), Cologne Digital Sanskrit Dictionaries |

> This is a **content** sample, not a design mock-up. It shows every layer of data the app would hold for one verse, with the source of each line. Final visual design comes in Phase 1.

---

### 1. Location
**ऋग्वेदः · मण्डलम् १ · सूक्तम् १ · मन्त्रः १**
Ṛgveda · Maṇḍala 1 · Sūkta 1 · Mantra 1

| | | Source |
|---|---|---|
| Devatā (addressee) | Agni | VedaWeb — "Addressees" dataset (CC BY 4.0) |
| Ṛṣi group | Hymns of Madhucchandas | VedaWeb — "Addressees" dataset (CC BY 4.0) |
| Chandas (metre) | *Not yet attached* — will come from a sourced index in Phase 1, not from memory | — |

---

### 2. Saṃhitā-pāṭha — Devanagari with Vedic svaras

> **अ॒ग्निमी॑ळे पु॒रोहि॑तं य॒ज्ञस्य॑ दे॒वमृ॒त्विज॑म् ।**
> **होता॑रं रत्न॒धात॑मम् ॥**

Source: *Ṛgveda-Saṁhitā*, Detlef Eichler; edited by Daniel Kölligan, VedaWeb (Cologne), 2020 — CC BY-NC-SA 4.0

Svara marks shown: horizontal line **below** (॒) = anudātta; vertical stroke **above** (॑) = svarita; udātta is left unmarked (standard Ṛgveda convention).

---

### 3. Transliteration (IAST, accented)

> agním īḷe puróhitaṁ yajñásya devám r̥tvíjam
> hótāraṁ ratnadhā́tamam

Source: *Ṛgveda-Saṃhitā*, input by B. A. van Nooten and G. B. Holland, revised by D. Eichler; via GRETIL → VedaWeb, 2020 — CC BY-NC-SA 4.0

---

### 4. Pada-pāṭha (word-by-word split)

> agnim · īḷe · puraḥ-hitam · yajñasya · devam · r̥tvijam · hotāram · ratna-dhātamam

> अग्निम् । ईळे । पुरःऽहितम् । यज्ञस्य । देवम् । ऋत्विजम् । होतारम् । रत्नऽधातमम् ॥

Source: *Ṛgvedasaṃhitā, Padapāṭha*, Sansknet Project; via GRETIL → VedaWeb, 2020 — CC BY-NC-SA 4.0
Note: the source gives the padapāṭha in **Latin script without accents**. The Devanagari line above was converted from it by script (not typed by hand, not AI-written). An accented Devanagari padapāṭha is a Phase 1 follow-up (candidate: Sanskrit Wikisource).

---

### 5. Word-by-word meaning and grammar

| Word | Stem / root | Grammar | Meaning (Monier-Williams, abridged) |
|---|---|---|---|
| agním | agní- | Acc. sg. masc. | fire; sacrificial fire; the god of fire |
| īḷe | √īḍ (Vedic √īḷ) | 1st sg. present indicative, middle | to implore; to praise |
| puróhitam | puróhita- | Acc. sg. masc. | placed in front, appointed; a family priest |
| yajñásya | yajñá- | Gen. sg. masc. | worship, devotion, praise; offering, sacrifice |
| devám | devá- | Acc. sg. masc. | heavenly, divine; a deity, god |
| r̥tvíjam | r̥tvíj- | Acc. sg. masc. | sacrificing at the proper time; a priest |
| hótāram | hótar- | Acc. sg. masc. | offerer of an oblation; the priest who invokes the gods |
| ratnadhā́tamam | ratnadhā́tama- | Acc. sg. masc. | greatest distributor of riches |

Sources:
- Stem and grammar: VedaWeb — University of Zurich morphological annotation (Lubotsky text; Widmer and Scarlata) — CC BY 4.0
- Meanings: Monier-Williams, *A Sanskrit-English Dictionary* (1899); Cologne digital edition © The Sanskrit Library and Thomas Malten — CC BY-NC-SA 3.0. The app will show full entries; this table shortens them for review.

---

### 6. English translations

**Griffith (Benares, 1890 edition; public-domain text)**
> I Laud Agni, the chosen Priest, God, minister of sacrifice, The hotar, lavishest of wealth.

Source: R. T. H. Griffith, *The Hymns of the Rigveda*; digital text via VedaWeb — CC BY-NC-SA 4.0

**Oldenberg (1897, public-domain text) — more literal alternative**
> I magnify Agni, the Purohita, the divine ministrant of the sacrifice, the Hotri priest, the greatest bestower of treasures.

Source: H. Oldenberg, *Vedic Hymns* (Sacred Books of the East, vol. 46); digital text via VedaWeb — CC BY-NC-SA 4.0
Note: Oldenberg translated only some hymns; Griffith covers the whole Ṛgveda. The source text has footnote numbers ("1 I magnify 2 Agni…"). They are hidden here, and the app would show them as tappable notes.

---

### 7. Hindi translation

> ⏳ **Pending.** No usable Hindi translation has been confirmed yet. Options are in SKT_REFERENCE.md §4.2 (part C) and Open Decision D5, and need your decision. Nothing is shown here instead, because the app never shows a translation without a confirmed source.

---

### Questions for the owner on this sample
1. Is this level of detail right for every verse (svaras, padapāṭha, word table, two English translations)?
2. Main English translation: **Griffith** (whole Ṛgveda, slightly old-fashioned verse style), with Oldenberg as an optional second where available. Approve?
3. Is anything missing that you expect to see on a verse page?
