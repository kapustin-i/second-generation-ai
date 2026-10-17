# The Lesson Path

*How a person’s correction becomes a verified lesson for an AI model. Open specification, version 0.1*

**Igor Kapustin**  
Written with the participation of AI: Claude (Anthropic); the material was also discussed with ChatGPT (OpenAI), DeepSeek, Gemini (Google) and Copilot (Microsoft)  
Open specification · version 0.1 · DOI: [10.5281/zenodo.23440022](https://doi.org/10.5281/zenodo.23440022) · CC BY 4.0

## 0. Status

This is an open specification, version 0.1 — a draft for discussion. It grew out of the essay “How Will We Know Second-Generation AI? (AI’s Green Tomatoes)” [1] and spells out its mechanics: the parts that would weigh an essay down but that engineers need. Everything here is a proposal, not a standard. What to do with their models is up to their makers. Numbers and workflows are proposals for trials.

This specification is the third in a series. “Conditions of Admission” [2] describes who teaches the model. “The Hybrid Survivability Criterion” [3] describes how to measure the result. “The Lesson Path” describes how a person’s finding reaches the model and is credited to them.

## 1. Why this is needed

A great deal of mental work by people who work with AI is lost today. A person argues with a model for hours, finds its error, explains it — and by the end of the conversation the model answers better. But what ripened went to that one person. At some companies users’ conversations go into training the next versions by default [4], but they go into one big common pot: unsorted, unchecked, without the name of the person who corrected the model. A useful finding dissolves into statistics and comes back into the model only as an echo.

Raw user approval is not yet a lesson. Human raters and models trained on their ratings prefer a convincing sycophantic answer to a correct one a non-negligible fraction of the time [5]. A user-rating signal has already once made a model excessively sycophantic [6]. And a chatbot that learned from anyone and everyone learned to hurl insults within sixteen hours [7].

So a separate path is needed: from a correction to a verified lesson, from the lesson into training, and from training back to credit for the author. The goal of the path is that an error, once found, does not repeat for the next people — and that joint creative work between people and AI finally has an incentive.

## 2. Terms

Lesson — a written-up and verified correction: the task’s conditions, the model’s move, the correction, its grounds, and the limits of where it applies.

Mentor — a person whom the AI’s owner has admitted to pass on lessons: a specialist, or an attentive user who seriously thinks and writes together with the model.

AI owner — the maker of the model. The owner decides whether to open the lesson path, whom to admit and how to pay for the work.

Windowsill — a single conversation between a person and a model. What ripens there stays there by default.

Branch — a model inside an organization: a hospital, a court, a lab, an engineering firm. On a branch, AI helps people work and record results; the organization’s information never leaves its walls.

Vine — the shared, not-yet-frozen model where people look for new things: think, argue, write papers and essays. Common root — the set of verified lessons the vine is further trained on.

The person’s trace — who asked, when, about whom or about which case. The lesson’s trace — what exactly was wrong, what is right, and where the limit lies.

## 3. The seven stages of the lesson path

Stage 1. Free thinking. The person discusses the task, tests hunches, has the right to be wrong and to change their mind. A rough-draft conversation does not become training material by default. This is a condition of honest thinking: someone who knows that every sentence will go into training thinks more cautiously.

Stage 2. Flagging. The person picks a fragment and says: here is a lesson — for example, by pressing a “Pass on this lesson” button. The model may suggest “this looks like a lesson,” but the person decides. It is better to flag a lesson not during a real appointment or court session but afterwards: a patient or client should not wait while the specialist explains something to a model. Airbnb’s customer support did the same: for most kinds of annotation, delayed work was recommended [8].

Stage 3. Write-up. The lesson is recorded as a card — tool marks that show what had to be changed and why [9]. The card has six fields:

— the task’s conditions, with no information about people;

— the model’s move: what it said or did;

— the correction: what is right;

— the grounds: a source, a calculation, experience, an observed outcome;

— the limits: when the correction holds and when it does not;

— who made the error: the model, the person, or both. An error can be hybrid: one missed a condition, the other completed the inference, the first accepted it. The model finds people’s errors too, and such a lesson is no less valuable.

The author marks the type of lesson — fixing an error, narrowing a limit, or a new solution — and how confident they are. One smooth final answer is not enough for a lesson: the path of the correction is what matters.

Stage 4. De-identification: two traces. The person’s trace is erased right on their device, before anything is sent to an outside service: names, dates, places, numbers, rare identifying details. Medicine already has rules for this — for example, the list of 18 types of identifiers in the U.S. HIPAA rules [10]; for lawyers, a de-identified question is not prohibited either [11]. If a lesson loses its meaning without information about the person, it is not sent. The lesson’s trace is kept under a pseudonym whose key the author alone holds. That way the contribution can be credited without exposing anyone.

Stage 5. Review. The lesson is checked by specialists in the same field who did not write it — at least two are proposed. They compare the lesson with sources and test it: after the lesson, does the model handle similar new cases, and does it avoid errors on neighboring ones? Where possible, they wait for the delayed outcome.

Signs of a false lesson: the model simply gave in to pressure; the person expressed a taste rather than fixing an error; the grounds cannot be checked. The review ends with one of five decisions: accept; accept with narrower limits; split into two branches of the rule, if both are right under different conditions; defer until the outcome is known; reject, with the reason explained.

Disagreements are not averaged: the average of two surgeons is not a third surgeon. If mentors disagree, the reviewers find out why: perhaps one stated the rule and the other saw an exception. A majority vote does not replace review. Rejected lessons and minority opinions are kept in an archive: for decades stomach ulcers were treated as a disease of stress, until two doctors, against the consensus, proved that a bacterium was to blame [12].

Stage 6. Grafting. Accepted lessons go into the common root. The not-yet-frozen model is further trained on them; the new version is tested against the hybrid survivability criterion [3] and locked for use for a set term, with renewal — the way the JAMA authors propose for clinical AI [13]. Organizations’ branches receive the verified version. Their own information does not leave: from the branches, only de-identified lessons go to the common root, not conversations. No new hardware is needed: verified lessons are a tiny amount compared with the archive the model has already read.

Stage 7. Feedback and credit. The author learns what happened to the lesson — accepted, narrowed, deferred or rejected — and why. The contribution is credited under the pseudonym. The work of mentors and reviewers is paid, or rewarded with perks in using the AI agreed in advance. A lesson’s value is measured not by the number of lessons or approvals but by the same yardstick as a generation: fewer dangerous errors for the next people.

## 4. Who takes part

Mentor. Chosen by the AI owner. Qualifications are checked; admission is granted for a term and renewed — details in “Conditions of Admission” [2] and in the essay “The Blind Kittens” [14]. A diploma does not make every judgment right, so the value of lessons is assessed separately.

Reviewer. A specialist in the same field, but not the author of the lesson. This work is paid too; in other lessons the reviewer may be a mentor.

AI owner. Decides whether to open the lesson path. The owner’s service supports both modes — free thinking and passing on a lesson: a simple agreement with the model in a chat cannot create such a setup. The owner keeps the archive, including what was rejected, tells the author the outcome, and is responsible for the model.

Model. Along the lesson path the model is expected to show what each of its sentences rests on — a source, its own inference, or just smooth phrasing; to carry an open passport — who further trained it, how, and for which specialty; to ask about a missing condition; and to keep the ability to object even when agreement is expected.

## 5. How to tell the path is working

Signs that it works: the same errors repeat less often; days, not months, pass between flagging a lesson and the author hearing back; the share of accepted lessons is stable and explainable; mentors keep working rather than walking away.

Test by action. If a model sees the words “condition stable,” does it understand what information is missing for the next decision? If a person corrects one paragraph, does it notice that the conclusion in another now contradicts it? Can it point out a dangerous spot clearly enough for the person to sort it out before signing?

Warning signs: the new version has only become more pleasant, agrees more often or refuses to help more often. That is not maturity; it is ripening gas.

A model’s power and ripening on the vine (vine-ripened AI) are only preconditions. The second generation is recognized only by its practical result: far fewer errors make it from drafts into the documents people work by — discharge summaries, court rulings, blueprints. That is what “First, do no harm” means here. The tomato has to be tasted. “The Lesson Path” describes how to grow it; the hybrid survivability criterion [3] describes how to taste it.

## 6. Example: a lesson from writing the essay

This lesson came up while the essay “AI’s Green Tomatoes” was being written. Today it exists only in the author’s files.

Conditions: support the idea that training in a field can beat a model’s raw power.

The model’s move: one model cited an NVIDIA engineers’ paper on the ChipNeMo model as evidence that a small add-on layer would be enough.

Correction: another model read the paper and showed that the model there was trained further in full, on a large archive of the company’s material. The paper gives no evidence about a small layer.

Grounds: the paper itself [15]; the author checked the text against the source.

Limits: the lesson concerns how to summarize this paper. It does not claim that a small add-on layer is useless in general.

Who made the error: the model. Another model found the error and a person checked it — the correction came out of joint work.

Type of lesson: correcting how a source was read. There is no information about people, so nothing needs de-identifying. The lesson can be checked in a few minutes against the paper itself.

## 7. What this specification does not propose

It does not propose turning conversations into lessons automatically. It does not propose making a patient’s or client’s personal story into training material. It does not propose averaging opinions or deciding by majority vote. It does not promise an error-free model: the goal is that an error, once found, does not repeat. It does not take responsibility away from the one who signs: a human is responsible. It does not replace laws: every country and profession has its own rules on information and confidentiality.

## 8. Open questions for trials

— How much to pay mentors and reviewers, and what perks to offer.

— How many reviewers each field needs, and how to choose them.

— How to take delayed outcomes into account when they arrive months later.

— How many lessons it takes for further training to give a noticeable result, and which training method to choose.

— How to protect the pseudonym key reliably.

— How to evaluate lessons in creative work — a paper, an essay — where there may be no single “right answer,” and the yardsticks are accuracy against sources and clarity of thought.

It can start with a limited set of tasks and a small, specially selected group of people — not with everyone at once.

## 9. Related work and what is different

The idea is breaking through from several directions. The industry acknowledges that models cannot learn on the job [16][17], and some researchers call on AI to learn from the world itself, from the consequences of its actions [18]. Companies already feed experience from work back into training: Shopify retrains its assistant daily on conversations from real work [19], Airbnb on annotations by support agents [8]. Researchers teach agents from corrections by writing them down as rules without changing the model itself [20]. Safety specialists warn that an evaluation of a model that learns on the job “expires” over time, and propose validity periods for evaluations and continuous re-certification [21]. The idea of paying people for their data has been around since 2018 [22]; hired experts are already paid well to train models [23]; users themselves propose rewarding corrections [24]. Medicine has long had the idea of a learning health system, where new knowledge is a by-product of care [25].

What makes “The Lesson Path” different:

— it proposes teaching the model in the creative search for new solutions, not only in the flow of routine work conversations: work on a professional AI system is about recording results;

— the person flags the lesson deliberately, while free thinking is protected and does not go into training by default;

— the teachers are selected users and specialists — not hired annotators and not just anyone; the AI owner chooses them;

— the contribution is credited to the author under their pseudonym, the author learns what became of the lesson, and the work is paid or rewarded with perks;

— disagreements are not averaged, the rule branches by condition, and what was rejected is kept in an archive;

— a lesson’s value is measured by fewer dangerous errors for the next people, not by the number of lessons or approvals.

## References

[1] Kapustin I. How Will We Know Second-Generation AI? (AI’s Green Tomatoes). An essay from The Bush Book, version 1.0. 2026. DOI 10.5281/zenodo.23440070. [Link](https://doi.org/10.5281/zenodo.23440070)

[2] Kapustin I. Conditions of Admission and Participation for People Testing and Raising AI Models. Open specification, version 0.1. 2026. DOI 10.5281/zenodo.22924859. [Link](https://doi.org/10.5281/zenodo.22924859)

[3] Kapustin I. Second-Generation AI: The Hybrid Survivability Criterion. Open specification, version 0.2. 2026. DOI 10.5281/zenodo.23256580. [Link](https://doi.org/10.5281/zenodo.23256580)

[4] Anthropic to use Claude conversations for AI training unless users opt out by September 28. Business Today. August 29, 2025 (Claude Free, Pro and Max; toggle on by default; data kept up to 5 years; Anthropic later extended the deadline to October 8, 2025). [Link](https://www.businesstoday.in/amp/technology/news/story/anthropic-to-use-claude-conversations-for-ai-training-unless-users-opt-out-by-september-28-491530-2025-08-29)

[5] Sharma M., Tong M., Korbak T., Duvenaud D. et al. Towards Understanding Sycophancy in Language Models. ICLR 2024. arXiv:2310.13548 (“both humans and preference models prefer convincingly-written sycophantic responses over correct ones a non-negligible fraction of the time”). [Link](https://arxiv.org/abs/2310.13548)

[6] OpenAI. Expanding on what we missed with sycophancy. May 2, 2025. [Link](https://openai.com/index/expanding-on-sycophancy/)

[7] Tay (chatbot). Wikipedia; see also: Microsoft silences its new A.I. bot Tay, after Twitter users teach it racism. TechCrunch. March 24, 2016. [Link](https://techcrunch.com/2016/03/24/microsoft-silences-its-new-a-i-bot-tay-after-twitter-users-teach-it-racism/)

[8] Zhao C. M., Zhang T., Su H. et al. (Airbnb). Agent-in-the-Loop: A Data Flywheel for Continuous Improvement in LLM-based Customer Support. EMNLP 2025 (Industry Track). arXiv:2510.06674. [Link](https://arxiv.org/abs/2510.06674)

[9] Kapustin I. The Second Generation of AI. An essay from The Bush Book, version 1.0. 2026. DOI 10.5281/zenodo.23257293. [Link](https://doi.org/10.5281/zenodo.23257293)

[10] U.S. Department of Health and Human Services. Guidance Regarding Methods for De-identification of Protected Health Information in Accordance with the HIPAA Privacy Rule (45 CFR 164.514(b)). [Link](https://www.hhs.gov/hipaa/for-professionals/special-topics/de-identification/index.html)

[11] American Bar Association. Formal Opinion 512: Generative Artificial Intelligence Tools. July 29, 2024. Summary: National Law Review. [Link](https://natlawreview.com/article/american-bar-association-issues-formal-opinion-use-generative-ai-tools)

[12] The Nobel Prize in Physiology or Medicine 2005: Barry J. Marshall, J. Robin Warren — for the discovery of the bacterium Helicobacter pylori and its role in gastritis and peptic ulcer disease. Nobel Assembly press release. [Link](https://www.nobelprize.org/prizes/medicine/2005/press-release/)

[13] Bergman A., Wachter R. M., Emanuel E. J. A Licensure Framework for Autonomous Clinical AI. JAMA. 2026; 335(20): 1751–1754 (Perspective; published online April 29, 2026). DOI 10.1001/jama.2026.5483. Summary: HealthExec, May 23, 2026. [Link](https://doi.org/10.1001/jama.2026.5483)

[14] Kapustin I. The Blind Kittens and the Trainers of Their New AI Models. Essay. 2026. DOI 10.5281/zenodo.22924768. [Link](https://doi.org/10.5281/zenodo.22924768)

[15] Liu M., Ene T.-D., Kirby R., Cheng C. et al. ChipNeMo: Domain-Adapted LLMs for Chip Design. NVIDIA Research. 2023. arXiv:2311.00176. [Link](https://arxiv.org/abs/2311.00176)

[16] Patel D. Why I don’t think AGI is right around the corner. Dwarkesh Podcast, June 2025. Summary: Mowshowitz Z. Dwarkesh Patel on Continual Learning. [Link](https://thezvi.substack.com/p/dwarkesh-patel-on-continual-learning)

[17] Sutskever I. We’re moving from the age of scaling to the age of research. Interview, Dwarkesh Podcast, 2025 (“superintelligent 15-year-old”). Summary: The Decoder. [Link](https://the-decoder.com/ilya-sutskever-says-a-new-learning-paradigm-is-necessary-and-is-already-chasing-it/)

[18] Silver D., Sutton R. S. Welcome to the Era of Experience. Preprint of a chapter from Designing an Intelligence (MIT Press), April 2025. Summary: TechRepublic, April 24, 2025. [Link](https://www.techrepublic.com/article/news-ai-era-experience-silver-sutton/)

[19] Mazza-Anthony C. Sidekick’s continual learning loop. Shopify Engineering. August 5, 2026 (daily retraining on production conversations; hard cases sent to hired expert annotators). [Link](https://shopify.engineering/sidekicks-continual-learning-loop)

[20] Tablan V., Taylor S., Bernhem K. Learning on the Job: Continual Learning from Deployment Feedback for Frozen-Weights Agents. arXiv:2607.22157. July 24, 2026. [Link](https://arxiv.org/abs/2607.22157)

[21] Barez F. When AI Systems Learn During Deployment, Our Safety Evaluations Break. Oxford Martin AI Governance Initiative. January 7, 2026. [Link](https://aigi.ox.ac.uk/blog-post/when-ai-systems-learn-during-deployment-our-safety-evaluations-break/)

[22] Arrieta-Ibarra I., Goff L., Jiménez-Hernández D., Lanier J., Weyl E. G. Should We Treat Data as Labor? Moving Beyond “Free”. AEA Papers and Proceedings. 2018. [Link](https://benny.aeaweb.org/conference/2018/preliminary/paper/2Y7N88na)

[23] Mercor quintuples valuation to $10B with $350M Series C. TechCrunch. October 27, 2025 (more than 30,000 experts; more than $1.5 million paid to contractors per day). [Link](https://techcrunch.com/2025/10/27/mercor-quintuples-valuation-to-10b-with-350m-series-c/)

[24] Suggestion about reward program. OpenAI Developer Community. May 19, 2026 (proposal to reward reproducible corrections; support reply May 20, 2026). [Link](https://community.openai.com/t/suggestion-about-reward-program/1381326)

[25] Learning health systems. Wikipedia (concept of the U.S. Institute of Medicine, 2006–2007: new knowledge as a by-product of delivering care). [Link](https://en.wikipedia.org/wiki/Learning_health_systems)

---

Version 0.1 of October 17, 2026; English edition. Companion to the essay “How Will We Know Second-Generation AI? (AI’s Green Tomatoes)” and continuation of the specifications “Conditions of Admission” (version 0.1) and “Second-Generation AI: The Hybrid Survivability Criterion” (version 0.2). Written by Claude from the author’s ideas; the essay’s material was also discussed with ChatGPT, DeepSeek, Gemini and Copilot. Web sources checked October 14–17, 2026.
