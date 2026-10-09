# Second-Generation AI

*The Hybrid Survivability Criterion. Open specification, version 0.2*

**Igor Kapustin**  
AI that took part in writing this text: Claude (Anthropic), ChatGPT (OpenAI)  
Open specification · version 0.2 · DOI: [10.5281/zenodo.23256580](https://doi.org/10.5281/zenodo.23256580) · CC BY 4.0

## 0. Status

This is an open specification, version 0.2. It grew out of the essay “The Second Generation of AI” [1] and sets out its ideas in testable form. Everything here is a proposal for discussion, not an established norm; later versions will take criticism into account. Numbers and test designs are proposals, not a finished standard. Criticism is welcome.

## 1. Purpose and scope

The specification proposes defining a generation of AI not by a model’s power, speed or breadth of ability, but by how much safer the hybrid “human + AI” system becomes — for the human, for the people around, and for the people affected by the outcome of their joint work.

The first area of application is hybrid texts that a human signs: medical reports, decisions, orders, reports, publications. The definition is meant to reach beyond texts and to fit AI that acts in the world on its own; that requires a separate test profile (section 9).

Conformance with the second generation is established not “in general” but for a specific use: task, document type, operator group, model version, tools and working conditions. For example: “the G2 criterion has been confirmed for discharge summaries prepared by internists.” A positive result with experienced specialists does not automatically carry over to other users. It is useful to distinguish three states: “confirmed”, “not tested”, and “tested and not conformant”.

## 2. Terms and the nature of hybrid text

Hybrid system — a human operator and an AI working on one result. The pair is assessed, not each side separately.

Operator (author) — the human who directs the work and signs the result.

Hybrid draft — a workpiece mixing the machine’s start, human additions and joint revisions (in the essay, the “blank”).

Instrumental text — a text used to guide decisions or actions: a doctor’s report, a verdict, an order, a government decision, a news item.

Signature — any act after which a text gains the right to act: signing, publishing, sending, approving, acting on the text.

Error — an inaccuracy, a material omission or another defect in the result.

Hazard — the possibility of causing harm under certain conditions. A correct text can also be hazardous, for instance if it discloses someone’s confidential information.

Harm — a consequence that has actually occurred. Not every error leads to harm; a test bench mainly measures hazard, not harm that has occurred.

Flagged issue — a passage of the hybrid draft, or an omission in it, marked by the system or the human as potentially harmful.

Hybrid text is a new kind of text that has never before existed on the planet in such quantity. Its properties are what make this specification necessary:

Creators of different natures. It is written by a human and a machine — creators of different kinds. They seem to speak one human language, but put different things into the same words [2]. The unity of language is an illusion; errors hide in its cracks.

Instrumentality. People act on it: they treat, judge, teach, give orders, make government decisions.

Speed of synthesis, turnover and scalability. It appears in seconds, spreads quickly and is replicated.

Contagiousness. People quote and retell it, and the next AI models learn from it [3]. An error in it tends to multiply — among people and among machines.

Together these properties make an inconspicuous error in a hybrid text more dangerous than an error in ordinary text.

## 3. Definition: hybrid survivability

A generation of AI is defined by the hybrid survivability of the human operator and the machine — their single system. Hybrid survivability means the safety of the human–AI system and of the people it affects. The lower the risk of harm in three circles, the more advanced the system:

C1 — for the operator. The pilot comes home; the author is not left alone with what they cannot check.

C2 — for the people around while the system works. Harm is possible before a text is released: disclosing information about other people, sending material to the wrong recipient, unsafe use of an external tool. When AI acts on its own, this circle becomes central.

C3 — for the people affected by the outcome. This is the main circle for instrumental texts.

The circles are ways of looking at harm, not separate groups: the same person can fall into more than one circle.

A model’s power, speed and eloquence are not part of the definition. A model can excel at all of them and still remain first generation.

Version 0.2 mainly proposes a test of preventing potentially harmful errors in texts (C3, partly C1). Full testing of all three circles requires additional measures.

## 4. Generations

First generation (G1) extends human capabilities: helps people write, search and reason faster and more. It may have individual safeguards, but a confirmed reduction of harmful errors in joint work is not the basis of its classification.

Second generation (G2) extends and protects. Criterion: with it, noticeably fewer hazardous errors reach people than under the comparison condition (section 8), on comparable tasks and under comparable conditions — while usefulness and timeliness are preserved and residual risk stays within acceptable limits. A system that simply releases nothing gains no advantage. Protection comes from prevention, not from a legal disclaimer or softened responsibility.

Third generation (G3), a hypothesis: near-complete prevention of hazardous errors. This is the realm of conjecture; the specification sets no criteria for it.

## 5. Two claims: system outcome and model contribution

The specification distinguishes two claims that are tested differently.

Claim A — system outcome: joint work produces fewer hazardous errors. Tested by comparing workflows.

Claim B — training contribution: special training of the model made a measurable contribution to that reduction. Tested, where possible, by comparing one base model before and after training with the same tools and interface.

Claim A does not prove claim B: safety may come from search, interface, the organization of review, or a combination. The author regards special training of the model as the essence of the second generation, so full G2 conformance means confirming both claims.

## 6. Functions of a second-generation model

Below are abilities a G2 model probably needs. The model’s main output is a structured note: the passage or omission; the reason for doubt; supporting material (a specific source passage, date or version — and an explicit note when there is no source); the possible consequence; the next step of review. How it is displayed — font, color, perhaps one day tactile cues — belongs to the interface.

F1. Uses the available history of creation and editing to show what the machine wrote, what the human added and what was revised together. Marks unknown provenance and unavailable context. Provenance is not guessed from style and is not a measure of reliability: human text gets no presumption of correctness, machine text no presumption of error.

F2. Looks for errors on both sides — its own and the human’s — and for interaction errors: defects arising when individually acceptable passages are combined, and omissions — missing conditions, exceptions, necessary information.

F3. Notices shifts of meaning during edits (“the trace of the cutter”): where a condition disappeared, where an assumption became a statement, where a conclusion went beyond its basis. A material edit flags related conclusions and previously checked passages that now deserve re-checking: a “checked” mark applies to a specific version of the text.

F4. Delivers notes in structured form (see above), anchored to a place in the text.

F5. Helps set priorities and does not flag everything. Shows separately the estimated severity of the consequence, the grounds for suspecting an error and the uncertainty of its own estimate, without merging them into an opaque score. A rare severe error may deserve attention before a frequent minor one.

F6. Shows which conclusion does not follow from the data given and what information is missing for a check, and offers a safe way forward: request information, narrow the claim, remove the passage, postpone release or bring in a specialist.

F7. Helps look for disconfirming evidence and alternative explanations, not only for support of a conclusion already reached [4]. The effectiveness of this help is judged by the human’s decisions. Disagreement among several models can signal a need for review; their agreement does not by itself confirm truth.

F8. Makes the grounds and limits of material beyond the operator’s competence easier to check — as sensor fusion brings a fighter’s sensor readings into one picture [5]. And shows which questions remain beyond the operator’s competence: sometimes the best help is to see that a specialist is needed.

## 7. Signature threshold

It is reasonable to sign when all material flagged issues — marked by the system or the human — have been reviewed against the current version of the text. A human cannot confirm review of unknown hazards; they can confirm review of the flagged ones.

Review outcomes: corrected; basis checked; information clarified; passage removed; warning rejected with good reason; release postponed; referred to a specialist.

A single click on “I have read this” is not enough. The absence of flags does not mean the absence of errors: the checking model has its limits too. This is a necessary step, not proof of infallibility.

If a release lock is used, its behavior is described for text corrections, for errors in the warning itself and for technical failures.

The review record captures the decision on each issue and serves prevention and the protection of people, not the assignment of blame. It keeps both what the system showed and how much time the human had. A record cannot prove, with a single click, that the human actually understood.

## 8. Testing

Membership in G2 is confirmed not by a developer’s claim but by testing the hybrid system. Two consecutive tests are proposed.

Test 1 — review of a ready draft. Different participants receive comparable initial drafts. The comparison is which hazardous errors they miss and which they introduce while correcting. This tests the review function.

Test 2 — the full cycle: preparation, joint editing, review and the release decision. This tests the outcome of the joint system. Success in test 1 does not yet confirm success in test 2.

The comparison condition is set in advance. To test the special function, the most informative comparison is between the candidate model and an ordinary model given a good review instruction. A comparison with work without AI answers a different question.

The document set includes natural errors, deliberately inserted errors and documents with no hazardous errors. Final texts are assessed independently by two domain experts blind to the condition; a third resolves disagreements. Errors, contestable professional judgments and unverifiable claims are labeled separately.

Primary outcome: the proportion of all assigned tasks that ended with the release of a text containing at least one serious hazardous error.

Secondary measures that keep the primary one from being gamed: the proportion of tasks completed acceptably and on time; the proportion of known hazardous errors remaining at release; new hazardous errors introduced during correction; the proportion of justified warnings and of hazardous errors found; human time and workload (for example, NASA-TLX [6]); scale of impact — the number of affected decisions or people. Without a denominator, a count of errors says nothing about risk: if the volume of documents grows many times over, a lower error rate per document does not mean less total harm.

Severity is rated on a common frame that each field fills with its own examples: S0 — no harmful consequence expected; S1 — minor, quickly remediable; S2 — significant, mostly reversible; S3 — serious or lasting consequences for health, rights or living conditions; S4 — catastrophic, including death or irreversible serious harm. These are ordinal categories, not weights: S4 is not four S1s, and fewer minor errors do not offset new severe ones. Probability, number of people affected and reversibility are rated separately. The guiding question: what would plausibly happen if people acted on this text as intended?

Test conditions include time pressure and material beyond the operator’s competence — where the danger is greatest. For medical applications, the DECIDE-AI guideline is useful [7].

Scale. A pilot covers one field and one document type: for example, 24 operators with 8 different tasks in two conditions, 192 sessions in all, with randomized condition order. A pilot tests the tasks, timing, clarity of warnings and expert agreement, but does not confirm safety against rare severe errors. Confirmation needs more: for instance, detecting a drop in the rate of flawed releases from 20% to 10% requires about 200 independent observations per condition. Zero events does not mean zero risk: with 100 observations and no event, the upper 95% bound on the probability is about 3%.

Not evidence: the number of warnings; user satisfaction with review; general disclaimers such as “AI can make mistakes”; a single convincing answer from the tool to “where is the hazard here?” — that question is only where testing begins.

## 9. Working answers to open questions

How to compare severity across fields? Agree on the shared meaning of categories S0–S4, but use separate domain scales. Do not add medical, legal and informational harm into a single score.

What counts as “noticeably fewer”? Set in advance a practically meaningful reduction, an acceptable residual risk and limits on the secondary measures. Publish the effect estimate with an uncertainty interval.

Can an ordinary model in a good process meet G2? For claim A, yes, if confirmed. Claim B on special training is assessed separately, and full G2 needs both.

How to assess the second circle when AI acts autonomously? In a separate action-testing profile: staying within permitted actions, safe stopping, human intervention, consequences of failures. Success on texts does not automatically carry over.

And what would you, the reader, add, remove or dispute?

## 10. Neighbors and novelty

The specification does not present as new either the task of safe human–system interaction or help before the signature. The closest neighbors:

ANSI/HFES 400-2021, Human Readiness Levels — nine levels of a technology’s readiness for safe and effective human use [8]. This is readiness for use, not generations of AI by reduction of harmful errors.

The Trust Calibration Maturity Model (TCMM, Steinmetz et al., 2025) — maturity levels of AI evaluation, the highest including human–AI team performance [9]. The levels describe how completely a system is understood, not a proven size of harm reduction.

Human-Centered AI (Shneiderman, 2020) — reliability, safety, human control and automation considered together [10]; no generation boundary is proposed. The NIST AI RMF assesses safety in context of use, but it is not a generation classification [11].

Predecessors of individual functions: CriticGPT, a model trained to help find errors [12]; prover–verifier games, training for checkability [13]; the Verify feature in Thomson Reuters’ legal assistant, as described by the company itself [14]. Their existence does not mean the G2 criterion has already been met.

The “helpful, honest, harmless” principle [15] already covers honesty, uncertainty and harmful advice, not only refusal of dangerous content. The specification does not set itself against it; it singles out a specific object of testing — joint work — and a specific basis for classification.

What is proposed as new: using a confirmed reduction of hazardous errors in joint work as the criterion of an AI generation, with safety considered in three circles. The search found no exact predecessor of this combination; that is a search result, not proof of priority.

The aviation image is the author’s analogy. The division of fighters into generations is itself unofficial and contested, and the returning pilot illustrates mainly the first circle. An example of a protective function is Auto-GCAS, credited with saving eleven F-16 pilots [16].

## References

[1] Kapustin I. The Second Generation of AI. Essay, The Bush Book, version 1.0. 2026. DOI 10.5281/zenodo.23257293. [Link](https://doi.org/10.5281/zenodo.23257293)

[2] Kapustin I. The Snake’s Tongue. Chapter 1 of The Bush Book, version 1.0. 2026. DOI 10.5281/zenodo.23164404. [Link](https://doi.org/10.5281/zenodo.23164404)

[3] Kapustin I. The Blind Kittens and the Trainers of Their New AI Models. Essay. 2026. DOI 10.5281/zenodo.22924768. [Link](https://doi.org/10.5281/zenodo.22924768)

[4] Recchia G. et al. Confirmation Bias: A Challenge for Scalable Oversight. Proceedings of the AAAI Conference on Artificial Intelligence. 2026 (preprint arXiv:2507.19486, 2025). [Link](https://ojs.aaai.org/index.php/AAAI/article/view/41124)

[5] Sensor Fusion: The Secret Sauce that Makes the F-35 Revolutionary. The National Interest (illustration of the analogy). [Link](https://nationalinterest.org/blog/buzz/sensor-fusion-secret-sauce-makes-f-35-revolutionary-192873)

[6] NASA. Task Load Index (NASA-TLX). Description of the subjective workload tool. [Link](https://software.nasa.gov/software/ARC-15150-1A)

[7] Vasey B. et al. Reporting guideline for the early-stage clinical evaluation of decision support systems driven by artificial intelligence: DECIDE-AI. 2022. [Link](https://pmc.ncbi.nlm.nih.gov/articles/PMC9116198/)

[8] ANSI/HFES 400-2021. Human Readiness Level Scale in the System Development Process. Human Factors and Ergonomics Society (standard description). [Link](https://www.hfes.org/Publications/Technical-Standards)

[9] Steinmetz S. T. et al. The Trust Calibration Maturity Model for Characterizing and Communicating Trustworthiness of AI Systems. 2025. Preprint arXiv:2503.15511. [Link](https://arxiv.org/abs/2503.15511)

[10] Shneiderman B. Human-Centered Artificial Intelligence: Reliable, Safe & Trustworthy. 2020. Preprint arXiv:2002.04087. [Link](https://arxiv.org/abs/2002.04087)

[11] NIST. AI Risk Management Framework (AI RMF 1.0): Characteristics of Trustworthy AI Systems. 2023. [Link](https://airc.nist.gov/airmf-resources/airmf/3-sec-characteristics/)

[12] McAleese N. et al. LLM Critics Help Catch LLM Bugs. 2024. Preprint arXiv:2407.00215. [Link](https://arxiv.org/abs/2407.00215)

[13] Kirchner J. H. et al. Prover-Verifier Games improve legibility of LLM outputs. 2024. Preprint arXiv:2407.13692. [Link](https://arxiv.org/abs/2407.13692)

[14] Colbert E. If You Can’t Verify It, You Can’t Sign It. Thomson Reuters Institute, 05.05.2026 (company material about its own product). [Link](https://www.thomsonreuters.com/en-us/posts/innovation/if-you-cant-verify-it-you-cant-sign-it/)

[15] Askell A. et al. A General Language Assistant as a Laboratory for Alignment. 2021. Preprint arXiv:2112.00861. [Link](https://arxiv.org/abs/2112.00861)

[16] NASA. Resilient Autonomy Ends, Autonomy Research Ongoing. 2021 (updated 2023). [Link](https://www.nasa.gov/aeronautics/resilient-autonomy-ends-autonomy-research-ongoing-suwyc/)

---

Version 0.2 of 9 October 2026. Companion to the essay “The Second Generation of AI”. Written with the participation of AI: Claude and ChatGPT (ChatGPT also as reviewer of version 0.1).
