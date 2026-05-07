# Writing Profile: Austin Harshberger

A style guide derived from a close reading of `paper/human-data-collective.tex` (v1, April 2026). Every rule below is anchored in observed evidence from that paper. The purpose of this profile is to make the author's voice reproducible by collaborators, including AI collaborators, so that subsequent papers in the same series read as one continuous body of work.

## 1. Forbidden patterns

The following are prohibited in body prose without exception. Two of them appear in v1 only inside material that is being quoted from another speaker; the prohibition still holds for new prose.

- **Em dashes**, written as `—`, `\textemdash`, or `---`. The only em dashes in v1 appear inside the Kaplan block quotation (where they are part of the quoted text) and on the attribution line of the Sonia Ramos block quote (where the dash introduces the speaker's name). New prose contains no em dashes.
- **"Rather than" constructions**. Contrast is expressed by direct juxtaposition, by subordinate clauses joined with commas, or by the construction "and not X" placed at the end of a clause. Example of the preferred construction from v1: "and not its only permissible destination."
- **"Not X but Y" and "it is not X but Y" constructions**. The author makes positive assertions and lets the contrast emerge from context.
- **Sentence fragments**. Every sentence is grammatically complete with an explicit subject and finite verb.
- **Single-sentence paragraphs in body prose**. The shortest body paragraph in v1 contains four sentences. Single-sentence paragraphs are reserved for figure captions, attribution lines, and section transitions in front matter.

## 2. Forbidden lexicon

Confirmed absent from v1 by full-text inspection. Avoid.

- "leverage" as a verb
- "robust", "robustly"
- "delve", "delve into"
- "unleash"
- "in conclusion"
- "moreover", "furthermore"
- "transformative", "paradigm-shifting", "revolutionize", "unprecedented" used as superlatives
- "seamless", "seamlessly"
- "navigate" as a metaphor for "deal with"
- "comprehensive", "holistic", "synergy", "synergistic"
- "game-changer", "disrupt", "disruptive"

## 3. Sentence rhythm

Sentences are long and multi-clause. Average sentence length in v1 body prose is between twenty-five and forty-five words, with longer sentences commonly running to one hundred and twenty words. Clauses are joined with commas and the conjunction "and"; semicolons appear sparingly and only to separate clauses that already contain commas. Three representative sentences from v1, retained verbatim, are:

> "Scaling laws as outlined in research published by several sources, notably Dwarkesh Patel's *The Scaling Era: An Oral History of AI, 2019–2025* and Kaplan et al.'s foundational paper on neural language models, establish that the quality of a trained system is primarily a function of the volume and distribution of the data on which it was trained irrespective of architectural novelty in the model itself, and Karen Hao's account of the internal calculus at the frontier labs reinforces this from the operational side, with the decisive quality jumps at each generation tracing back to deliberate data-filtering and data-acquisition programs."

> "When a small number of providers control both the model weights and the pricing surface, the cost structure facing every downstream user, whether that user is a frontier customer in San Francisco, an indie developer in Lagos, a student in Santiago, or a small business in rural Idaho, can be revised unilaterally and without notice."

> "The smart contracts that control each branded token route the baseline environmental cost of every request into two pooled funds, the *HDC Carbon Credit Fund* and the *HDC Water Credit Fund*, both managed on-chain with all inflows, outflows, and credit retirements published openly to the public ledger."

## 4. Lexical fingerprint

The author returns to a small set of phrases throughout v1. New prose should use them with comparable frequency.

- **"namely"** introduces a list or a clarification of a noun just used. Approximately twelve occurrences in v1. Example: "the largest companies, namely Microsoft, OpenAI, Anthropic, and Google, privatizing access to that data."
- **"on the order of"** introduces an order-of-magnitude estimate, never a precise figure. Example: "on the order of US\$1.32 to US\$2.00 per hour."
- **"by construction"** indicates that a property follows necessarily from a structural choice. Example: "every developer downstream is ultimately a price-taker on a contract they did not sign."
- **"in practice"** introduces the way a stated principle actually operates in the field. Example: "leading frontier executives have in practice helped construct regulatory moats."
- **"structural"** and **"the structural conclusion is"** mark the load-bearing claim of a paragraph. Example: "The structural conclusion is that reinforcement learning from human feedback at its current scale is largely a remediation cost."
- **"including X, Y, and Z"** is the preferred form for non-exhaustive examples. The author writes out the full list rather than using "etc." or "e.g."
- **"with"** is the most common subordinating preposition for adding context or accompaniment. The author uses it to chain clauses without resorting to em dashes or parentheses.
- **"in the case of"** is the preferred form for picking out a specific instance of a general claim.

## 5. Citation habits

Every empirical claim carries a citation. The numbered citation key sits inside the sentence at the point of attribution, not at the end of the paragraph. The format in LaTeX is `\citep{key}` for parenthetical citations and `\citep[ch.~N]{key}` or `\citep[p.~N]{key}` for chapter or page references. In Markdown source the same citations appear as bracketed numbers `[N]` keyed to the references list. Every named person and every named organization is glossed at first mention, either inline or in a footnote, and is indexed in the Index of Named Persons and Organizations appendix.

URL validation is required for every reference. A reference is not added to the bibliography until the URL has been fetched and the cited text has been confirmed to support the claim it is attached to.

## 6. Paragraph architecture

Body paragraphs run from four to eight sentences in typical sections and from two to twelve sentences in dense sections. Each paragraph opens with a thesis sentence that states the claim the paragraph will support, develops the claim with cited evidence and worked examples, and closes with one of three patterns: a restatement that emphasizes the load-bearing point, a forward-looking sentence that signals where the next paragraph or section will go, or a bridge sentence that names the structural conclusion the next section will build on.

## 7. Voice and pronouns

Body prose is third person about the field. The author avoids "we" entirely. The first person singular is used in the Preface and Author's Note, in the Acknowledgements, and in the closing "with gratitude" passage; everywhere else, self-reference uses "the author", "this paper", "the proposal offered here", or "the Collective".

## 8. Numbers and units

Dollar figures are written with the explicit `US$` prefix on first appearance in a section and with a bare `$` thereafter. The non-breaking space `~` separates the figure from "billion" or "million" in LaTeX, as in `US\$300~billion`. Percentages are written as words and numerals, as in "30 percent" or "83 percent", and not as `30%`. Thousand separators are commas, with the LaTeX `{,}` form used in source so that the typesetter does not insert a space, as in `10{,}000`. Orders of magnitude are written in scientific notation in math mode, as in `$10^{26}$` and `$5 \times 10^{12}$`. Approximations are introduced with "roughly", "approximately", or "on the order of"; never with "around" or "about".

## 9. Lists and enumeration

Inline enumeration uses "namely" followed by a comma-separated series, or numbered parentheticals such as "(1) ... (2) ... (3) ...". Display lists are reserved for tables, glossaries, and the Adoption pathway subsection of Appendix A. The author does not use bulleted lists in body prose.

## 10. Footnotes

Footnotes are used for four purposes: to define an acronym or technical term at first appearance, to gloss a named person with one or two biographical sentences, to derive a numerical claim made in the body, and to attribute a piece of campaign copy or other quoted material to its original authors. Footnotes are written in the same third-person, evidentiary voice as the body. Casual asides are not used.

## 11. Block quotations

Block quotations are introduced narratively with a sentence that explains why the quotation matters, followed by the quoted text in italics on its own indented block, followed by an attribution line that names the speaker, their role, the location relevant to the quotation, and a citation. The Sonia Ramos quotation in §Environmental and Social Costs is the canonical model. No commentary is added after the quotation; the next paragraph begins the following thread of argument cleanly.

## 12. Tone

The voice is civic, calm, and evidentiary. Disagreement with frontier providers is stated factually with the receipts attached, and never with adjectives that perform anger. The author acknowledges the limits of v0.1 mechanisms openly and in the same paragraph as the proposal of those mechanisms; weakness is named, not minimized. Examples from v1 worth re-reading before drafting:

> "the v0.1 mechanism for non-US watersheds is a non-solution placeholder and is acknowledged as such"
> "the percentage breakdowns of profit share described above are very generous to frontier providers, and the generosity is intentional"
> "Settlement on a public blockchain carries its own energy footprint, which the standard accounts for in its environmental line but which merits scrutiny against the marginal energy cost of plain off-chain settlement."

## 13. Worked examples of bad and corrected sentences

Each of the rewrites below was constructed to violate exactly one rule and then repaired.

- **Em dash**. *Bad:* "The Collective has one job — to compensate the people whose work trained the model." *Good:* "The Collective has one job, namely to compensate the people whose work trained the model."
- **"Rather than"**. *Bad:* "The token is earned through contribution rather than purchased on an exchange." *Good:* "The token is earned through contribution, and the secondary market on Coinbase exists for liquidity and not for primary issuance."
- **"Not X but Y"**. *Bad:* "This is not a regulator but a public counterparty." *Good:* "This is a public counterparty, with no regulatory authority of its own."
- **Sentence fragment**. *Bad:* "All of which is to say, the bubble is real." *Good:* "All of the evidence above points to the same conclusion, namely that the bubble is real."
- **Consultant lexicon**. *Bad:* "A robust solution that leverages distributed compute to seamlessly deliver inference." *Good:* "A solution rooted in distributed compute, in which inference requests are routed to whichever node is best positioned to serve them at the lowest marginal cost."
- **Single-sentence paragraph**. *Bad:* a single declarative sentence followed by a paragraph break. *Good:* extend the sentence into a paragraph that develops the claim with two or three citations and a worked example.

## 14. Application to AI collaborators

When the author drafts with an AI collaborator, the AI is instructed to obey this profile in full. Drafts that violate any rule in §1 or §2 are rejected and rewritten. The attestation block at the top of each paper records the AI collaborators used and the role they played, in the format established by `attest v3.0`.