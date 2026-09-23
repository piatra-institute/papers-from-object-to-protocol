# Audit

Dated log of editorial passes and verification runs. Newest first.

## 2026-09-23 — structured-evidence migration

Structured-evidence migration (references and claims).
- references.yaml: 36 CSL entries, all entered by hand (no legacy DOIs; Crossref matches for this bibliography were book reviews or unavailable). Two carry DOIs (bourdieu1996, strathern1988). Web sources retrieved 2026-09-23 (Whitney artport, Serpentine, Sotheby's auction page, El País, Federal Register, Art Blocks, fxhash, PromptBase); MoMA and SFMOMA pages refused automated retrieval and carry no URL.
- Changes: El País article attributed to its author, Pablo G. Bejerano (id bejerano2025; citation now "(Bejerano 2025; PromptBase n.d.)"); LeWitt documentation entry split into sfmomand and whitneynd; vasari1550 added for the 1550 edition named in the text; Illuminations publisher Schocken -> Harcourt, Brace & World (1968 first edition); Whitney citation for xhairymutantx entered as whitney2024 (the legacy entry listed the artists as authors of the Whitney page). Benjamin, Greenberg, Weiner and Young carry original dates and render as "[1936] 1968" etc.
- Citations added where legacy entries were uncited: Ono (suppress-author at "Grapefruit"), Young (the quoted score), MoMA (Fluxus documentation sentence), SFMOMA and Whitney (LeWitt documentation sentences), Weiner (Statement of Intent), Art Blocks and fxhash (documentation sentences), PromptBase (prompt-marketplace sentence).
- claims.yaml: 16 claims (5 source, 4 definition, 4 interpretation, 1 assumption, 2 normative). Source claims checked against the retrieved documents: Copyright Office guidance on prompts and on selection/arrangement (Federal Register text), Whitney page on xhairymutantx, Serpentine page on The Call (fifteen choirs, Data Trust), El País on prompt volatility after Midjourney updates.
- Not bound: the Botto sentence (Sotheby's page confirms the October 2024 sale but not the attribution to Klingemann, ElevenYellow and the BottoDAO); MoMA, SFMOMA and Whitney documentation statements (pages not retrievable); Art Blocks and fxhash documentation wording; Galanter's definition; book-length sources (Belting, Gell, Strathern, Bourdieu, Danto, Dickie, LeWitt, Cage, Cohen).
- No simulation; metadata claims_target: none -> claim-ledger.

## 2026-09-23 — prose revision

Prose revised against the house standards. Headings: Abstract; 1. Introduction; 2. Images before the autonomous object; 3. Formation of the object configuration; 4. Conceptual and score-based art; 5. Generative code art; 6. Latent score art; 7. Definition of a protocol; 8. Legal, market, and aesthetic consequences (8.1 Legal authorship; 8.2 Market structure; 8.3 Aesthetic ontology); 9. Limitations: opacity, substrate drift, and platform persistence; 10. Conclusion.
Tic counts before -> after: 'rather than' 19 -> 0; inline ', not X' 5 -> 0; 'this paper/the paper' 8 -> 0; 'That is/This is' sentence starts 5 -> 0; exactly/precisely 1 -> 0; merely/simply 1 -> 0. Abstract about 430 -> 259 words.
Corrections: section 7 attributed the instruction "draw a straight line and follow it" to a Brecht event score; it is La Monte Young's Composition 1960 #10 (as section 4 already stated). Corrected.
Removed the reference to "the deep-research survey that informed this paper" (unpublished origin material) and the description of the institute's own Prism studio as an illustrative case; the world-generation kit is kept as an explicitly hypothetical example, and the closing paragraph about the institute's practice is removed.
Citations: Benjamin (1936), Cage (1961), Brecht (1963), Cohen (1995), Danto (1981), Dickie (1974), Gell (1998), Strathern (1988), Zylinska (2020) were listed but uncited; each is now cited at a point it supports. Greenberg (1960), Krauss (1986), Manovich (2018) now carry years. References section unchanged.
Not changed: the text calls Weiner's text "Statement of Intent" while the bibliography lists "Declaration of Intent"; both titles are in use for the 1969 text.
No simulation; no numerical results to audit.

## 2026-06-13 — voice reform

Voice-reform pass for AI-writing tells.

Syntax warns fixed:
- §2 negate-pivot "Pre-object regimes are not for romanticizing. They were embedded in…" → "These regimes invite no nostalgia. They were embedded in social orders we would now reject: …"
- §7 inline-contrastive "the license sits inside the ontology, not outside it as paratext" → "…a constituent of the work rather than paratext around it."
- §10 two negate-pivots ("is not only a thing on the wall; it is also a license"; "is not only the artifact; it is also the protocol") rewritten as positive declaratives.
- Remaining warn ("realized, not realized, or realized differently") left intact: a genuine three-way enumeration of Weiner's realization permissions, not a contrastive pivot.

Structure: deleted the §1 roadmap paragraph ("The paper proceeds in four registers… Section 9… Section 10 is a register of objections"), which the heading set already covers and which mislabeled its own numbering. Retitled the bolt-on "9. Limits and Counter-Cases" → "9. Where the Migration Strains: Opacity, Drift, and Dead Platforms". The formulaic-skeleton structure advisory now clears. Section is substantive (five named counter-cases), so retitled rather than folded; numbering unchanged, cross-reference in §6 ("return to both in section 9") still resolves.

Density (closing section): broke the reflexive triad "in a rule rather than in a brushstroke, in a license rather than in a frame, in a protocol rather than in an object" to a pair.

Lexical-density advisory: before signature carries/carry 5, precisely 1; tricolon proxy 63. After carries/carry 5, precisely 1; tricolon proxy 62. (The five "carry" uses are literal and varied, not the metaphorical pet-cluster sense; left in place.)

Verify: voice 0 errors (1 warn, the kept enumeration); structure advisory cleared; refs unchanged (pre-existing "author-year not reliably detected" advisory, no citation altered); build OK, 0 missing-character warnings; check => PASS.

## 2026-05-29 — upgrade pass (Group D)

Baseline: voice 0 errors, refs advisory, 15 pages. Strong and well-structured;
the pass is surgical voice + one genealogical gap + one citation fix.

Scope contract:
1. Voice tells: §1 "The historical record presents a different picture"
   contrasting-frame announcer; §5 "newly explicit and newly tradable" hedge;
   §9 five "The Nth limit is …" openers → clean bold leads (the numbered-
   consequence cadence voice.md discourages).
2. Research (named gap): engage Duchamp's readymade in §4 — the early-twentieth-
   century precedent for the work-as-designation that the genealogy jumps over
   (object → Cage 1952) — with a scholarly anchor (de Duve, 1996).
3. Citation: add Greenberg, named in §8.3 ("in the line of Greenberg, Krauss,
   and Manovich") but absent from the bibliography.

Next-pass candidates (logged): prune genuinely uncited background refs (Dickie,
Zylinska) or engage them; sharpen the latent-score-vs-static-AI contrast with a
named artwork on each side.

Verification: voice 0 errors; refs advisory; build clean; check => PASS.
