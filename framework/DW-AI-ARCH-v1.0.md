# DW-AI-ARCH: DeepWing Framework, Formal Edition v1.0

This file is the full text of the DeepWing Framework formal edition (DW-AI-ARCH v1.0, ratified 2026-10-27), published in two parts: Part I is the English edition and Part II is the Chinese edition. The framework defines seven layers and ten gates for enterprise AI systems, with 385 numbered clauses and 70 check items. Check item numbers use the full layer name as prefix (for example, Model-C1 and its Chinese counterpart); two-letter codes are not used.

Publisher: DeepWing (deepwingai.com)
Citation: DeepWing. DW-AI-ARCH: A Seven-Layer, Ten-Gate Framework for Enterprise AI, Formal Edition v1.0. 2026. Deposit copy: Zenodo, DOI 10.5281/zenodo.23715226.
License: CC BY 4.0 (see the LICENSE file in this repository).

Conversion note: this Markdown file was converted from the formal edition source files held by DeepWing. The translator's working terminology table that precedes the English source text is not part of the published edition and is omitted here; everything else is reproduced in full.

---

# Part I: English Edition

Version: Formal Edition v1.0 (first edition), 2026-10-27
Basis for ratification: DW-AI-ARCH v1.0 Ratified Version (2026-10-23); layer names and gate names are identical, word for word, to the Ratified Version
Companion model: DeepWing AI Governance Reconciliation Model (DW-AI-GOV v1.0); the governance interface conventions of Chapters 12 and 14 of this document are aligned with it
Byline: DeepWing

Citation format: DeepWing. DW-AI-ARCH: A Seven-Layer, Ten-Gate Framework for Enterprise AI, Formal Edition v1.0. 2026-10-27.

---

## Contents

### Preface (unnumbered)
Explains the origin of this document, its line of succession from DW-AI-ARCH v1.0, and the general position of "responsibilities, not deployment."

### Chapter 1: Scope
What this document governs, what it does not govern, and whom it is written for.
- 1.1 Purpose
- 1.2 Scope of Application
- 1.3 Intended Users
- 1.4 Boundaries

### Chapter 2: Normative References
The registered documents and registers on which the clauses of this document rest.
- 2.1 Framework Documents
- 2.2 Registers
- 2.3 External Documents

### Chapter 3: Terms and Definitions
The unified vocabulary of the whole document, including the Chinese and English names side by side and the list of retired names.
- 3.1 General Rules
- 3.2 Official Names of the Layers and Gates
- 3.3 General Terms
- 3.4 Retired Names

### Chapter 4: General Provisions
The overall map of the seven layers and ten gates, their correspondences, and the preconditions for use; the foundation chapter of the whole document.
- 4.1 Composition of the Framework
- 4.2 Overview of the Responsibilities of the Seven Layers
- 4.3 The Ten-Gate Check Sequence
- 4.4 Correspondence Between Layers and Gates
- 4.5 Preconditions for Use

### Chapter 5: Model Specification
The responsibility layer in charge of understanding and generation: it is responsible for model selection, routing, versions, and cost attribution; it is not responsible for execution or permissions.
- 5.1 Scope and Definitions
- 5.2 Responsibility Boundaries
- 5.3 Constituent Elements
- 5.4 Common Failure Modes
- 5.5 Normative Clauses
- 5.6 Check Items
- 5.7 Interfaces with Other Layers and Gates
- 5.8 Related Cases

### Chapter 6: Orchestration Specification
The responsibility layer that decides "what to do next and who should handle it": it is responsible for intent decomposition and step orchestration; it is not responsible for concrete execution.
- 6.1 Scope and Definitions
- 6.2 Responsibility Boundaries
- 6.3 Constituent Elements
- 6.4 Common Failure Modes
- 6.5 Normative Clauses
- 6.6 Check Items
- 6.7 Interfaces with Other Layers and Gates
- 6.8 Related Cases

### Chapter 7: Tool Use Specification
The responsibility layer that truly carries decisions out: it is responsible for tool access, parameter contracts, and call reliability; it is not responsible for whether a thing should be done.
- 7.1 Scope and Definitions
- 7.2 Responsibility Boundaries
- 7.3 Constituent Elements
- 7.4 Common Failure Modes
- 7.5 Normative Clauses
- 7.6 Check Items
- 7.7 Interfaces with Other Layers and Gates
- 7.8 Related Cases

### Chapter 8: Memory Specification
The responsibility layer in charge of remembering context: it is responsible for the storage, retrieval, and boundaries of short-term and long-term memory; it is not responsible for enterprise knowledge supply.
- 8.1 Scope and Definitions
- 8.2 Responsibility Boundaries
- 8.3 Constituent Elements
- 8.4 Common Failure Modes
- 8.5 Normative Clauses
- 8.6 Check Items
- 8.7 Interfaces with Other Layers and Gates
- 8.8 Related Cases

### Chapter 9: Knowledge Specification
The responsibility layer that supplements the model with private knowledge: it is responsible for retrieval, vector storage, and knowledge currency; it is not responsible for conversational context.
- 9.1 Scope and Definitions
- 9.2 Responsibility Boundaries
- 9.3 Constituent Elements
- 9.4 Common Failure Modes
- 9.5 Normative Clauses
- 9.6 Check Items
- 9.7 Interfaces with Other Layers and Gates
- 9.8 Related Cases

### Chapter 10: Access Control Specification
The responsibility layer in charge of permission determination before the fact: it is responsible for who can do what and who can see what; it is not responsible for tracing after the fact.
- 10.1 Scope and Definitions
- 10.2 Responsibility Boundaries
- 10.3 Constituent Elements
- 10.4 Common Failure Modes
- 10.5 Normative Clauses
- 10.6 Check Items
- 10.7 Interfaces with Other Layers and Gates
- 10.8 Related Cases

### Chapter 11: Observability Specification
The responsibility layer in charge of seeing clearly, after the fact, what happened: it is responsible for tracing, evaluation, and quality monitoring; it is not responsible for interception before the fact.
- 11.1 Scope and Definitions
- 11.2 Responsibility Boundaries
- 11.3 Constituent Elements
- 11.4 Common Failure Modes
- 11.5 Normative Clauses
- 11.6 Check Items
- 11.7 Interfaces with Other Layers and Gates
- 11.8 Related Cases

### Chapter 12: Ten-Gate Check Specification
Writes the ten gates, gate by gate, as check clauses, specifying what each gate checks, on what basis it determines, and what happens if a gate is not passed.
- 12.1 Gate 1, Gateway: Is This Key Still Valid? (Cross-Layer)
- 12.2 Gate 2, Access Control: Which Doors Can This Key Open? (corresponding to the access control layer)
- 12.3 Gate 3, Orchestration: Who Should Handle This Sentence? (corresponding to the orchestration layer)
- 12.4 Gate 4, Knowledge: Finding the Latest Rule Among Tens of Thousands of Files (corresponding to the knowledge layer)
- 12.5 Gate 5, Memory: Does the Model Remember This Customer? (corresponding to the memory layer)
- 12.6 Gate 6, Tool Use: Truly Stepping Into Real Systems to Get Things Done (corresponding to the tool use layer)
- 12.7 Gate 7, Model: Assembling All the Clues Into One Sentence in Human Language (corresponding to the model layer)
- 12.8 Gate 8, Observability: After the Answer Is Given, Who Is Watching the Quality? (corresponding to the observability layer)
- 12.9 Gate 9, Platform: The Eight Gates, Set Up Separately by Each or Shared as One Set? (Cross-Layer)
- 12.10 Gate 10, Alignment & Autonomy: The Common Road, Are Teams Willing to Walk It Themselves? (Cross-Layer)

### Chapter 13: Conformity Assessment and Check Methods
How to check, how to score, and in what situations a single red line decides the outcome.
- 13.1 The Two Forms of Checking
- 13.2 Scoring Rules
- 13.3 Red Line Rules
- 13.4 Evidence Strength
- 13.5 Conclusions and Re-Checks

### Chapter 14: Records and Evidence Specification
The registration formats that accompany the framework, ensuring that every determination can point back to an ID number and a source.
- 14.1 Common Fields
- 14.2 Evidence Grades
- 14.3 Disclosure and Date Conventions
- 14.4 Record Status and ID Rules
- 14.5 The Three Attributes of a Sentence

### Annex A: Case Index (informative)
An index of case ID numbers arranged by layer; each entry gives the ID number and the main points of the title, and the case library governs the body text. It has seven layer subsections: the model layer, the orchestration layer, the tool use layer, the memory layer, the knowledge layer, the access control layer, and the observability layer.

### Annex B: Glossary (informative)
A master table of terms in Chinese and English, consistent with the official names in Chapter 3, for reference.

### Annex C: Version and Revision Record (normative)
The version history of this document: each revision records the date, the version, the chapter, the content, and the basis.

### Annex D: Ten Gates and NIST AI RMF Crosswalk (informative)
Maps each of the ten gates to the functions and subcategories of NIST AI RMF 1.0, with a gap list of RMF areas the ten gates do not cover and a supplementary table of generative AI risks. Prepared by DeepWing (prepared independently; NIST did not participate).
- D.1 Basis of Preparation and Primary Sources
- D.2 Main Mapping Table
- D.3 Gap List: What the RMF Covers and the Ten Gates Do Not
- D.4 Supplementary Table of Generative AI Risks (NIST AI 600-1)
- D.5 Positioning Statement

### End Matter I: Gap List
The unresolved matters of Formal Edition v1.0: wherever the source materials and the Ratified Version cannot support a point, and this edition leaves it blank or sets out only a determination method, the matter is listed here.

### End Matter II: Conventions of This Document
The numbering, terminology, clause, and version record conventions used throughout the manuscript.

---

## Preface

This document is the Formal Edition of the DeepWing enterprise AI architecture framework (DW-AI-ARCH). It carries forward the DW-AI-ARCH v1.0 Ratified Version: layer names, gate names, gate themes, the scoring and red line conventions, record formats, and evidence grades are all governed by the Ratified Version. This document does one thing only: it expands the structure of the Ratified Version into clauses that can be executed and verified.

The general position of this document is a single sentence: responsibilities, not deployment. The seven layers are a division of responsibilities, not a division of physical deployment; one component may serve several layers, and one deployment may be split across several layers. Wherever a case and the framework do not agree, the framework is changed first, and the change is entered in the revision record of Annex C; a case is never forced to fit the framework.

This document is used as a pair with the DeepWing AI Governance Reconciliation Model (DW-AI-GOV): this document answers how a system is to be built, and the Governance Reconciliation Model answers whether rules and reality reconcile with each other. Where a governance requirement lands in a system is governed by the gates of Chapter 12 of this document; the discipline by which cases point back to rules and readings point back to ID numbers is governed by Chapter 14 of this document, consistent with the data binding of DW-AI-GOV.

---

## Chapter 1: Scope

1.1 Purpose: to write the division of responsibilities and the check sequence of enterprise AI systems as clauses that can be executed and verified, so that any AI system that has entered, or is preparing to enter, a production environment can be checked, determined, and recorded against the same set of questions.

1.2 Scope of application: AI applications and agent systems built with large models, with the emphasis on systems that have entered, or are preparing to enter, a production environment and that will produce consequences for real business and real users. Systems in purely offline experiments and in controlled evaluation environments may use this document as a reference for risk mapping, but the case attribution of such systems shall be separately marked under the conventions of Chapter 14 (see the manner of marking of INC-013 in Annex A).

1.3 Intended users: architects, technical leads, procurement and compliance personnel, and the persons responsible for go-live review. It is also provided for operators of the check tools that use this framework (the Quick Self-Check and the Deep Diagnostic), so that they can cross-reference the source of a clause.

1.4 Boundaries: this document is an analytical framework of DeepWing; it is not an industry standard, and it does not prescribe specific products, vendors, or deployment forms. Each individual case and number that appears in the clauses can be traced back to a registered ID, and none is elevated into a general rule for the whole industry; for quantitative thresholds, this edition sets out only determination methods and does not fix numbers in place (see the Gap List).

---

## Chapter 2: Normative References

2.1 Framework documents:
(1) DW-AI-ARCH v1.0 Ratified Version (2026-10-23), the source of the conventions of this document;
(2) DeepWing AI Governance Reconciliation Model v1.0 Ratified Version (DW-AI-GOV, 2026-10-26), the basis for aligning the governance interface conventions of Chapters 12 and 14;
(3) The Ten Gates and NIST AI RMF crosswalk, see Annex D, an informative reference, which creates no clause obligations.

2.2 Registers: the registered registers to which the clauses of this document and the conclusions of its checks point back, including: incident cases (INC), special volumes (SP), management measures (GOV), regulatory enforcement (REG), external agent admission (AGT), model changes (MOD), costs (COST), architecture cards (ARC), new ideas (IDEA), product teardowns (PD), frontier companies (CO), laboratories (LAB), people (PPL), and weekly (WK), together with Desk 2 occupational exposure (OCC), employment research (RES), and hiring signals (HIR), and Desk 3 medical devices (MED). The ID rules and status conventions of each register are given in Chapter 14.

2.3 External documents: the clauses of this edition do not directly impose compliance obligations from external documents. Wherever external standards and official documents mentioned in the source materials appear, they appear only as informative references in the corresponding clauses; the verification, item by item, of their versions and dates is entered in the Gap List, and until that verification is complete they are not used as a basis for determination.

---

## Chapter 3: Terms and Definitions

3.1 General rules: when a term first appears, it is written as "Chinese official name (English Name in English)"; thereafter only the Chinese official name is used. Check-item numbers use the full layer name as their prefix (see 3.2); narrative text uses the full official names throughout and does not use codes to refer to layer names or gate names.

3.2 Official names of the layers and gates:

The seven layers (responsibilities, not physical deployment):

| Layer | English | Corresponding Gate |
|---|---|---|
| Model | Model | Gate 7, Model |
| Orchestration | Orchestration | Gate 3, Orchestration |
| Tool Use | Tool Use | Gate 6, Tool Use |
| Memory | Memory | Gate 5, Memory |
| Knowledge | Knowledge | Gate 4, Knowledge |
| Access Control | Access Control | Gate 2, Access Control |
| Observability | Observability | Gate 8, Observability |

Note: check-item numbers use the full layer name as prefix, for example "Model-C1" and "Access Control-C1"; see the conventions in the End Matter. Two-letter codes are discontinued from this edition and are no longer used for numbering or reference.

The ten gates (the check sequence of one request): 1 Gateway (cross-layer), 2 Access Control, 3 Orchestration, 4 Knowledge, 5 Memory, 6 Tool Use, 7 Model, 8 Observability, 9 Platform (cross-layer), 10 Alignment & Autonomy (cross-layer). Seven gates correspond to the seven layers; the three gates Gateway, Platform, and Alignment & Autonomy are cross-layer.

3.3 General terms:
(1) Check item: a check entry, established by gate or by layer, that can be determined item by item as pass or fail; the number format is given in the conventions in the End Matter;
(2) Primary failure layer: the first layer of failure determined in the attribution of a case; secondary-layer association refers to a layer related to the event but not the first layer of failure;
(3) Evidence grade: a four-level calibration of the credibility of a record; the definitions and determinations are given in 14.2 of Chapter 14;
(4) Last Verified: the date on which a record was most recently re-verified against a primary source;
(5) Red line: a situation on the triggering of which the conclusion shall not be "cleared for go-live"; see 13.3 of Chapter 13;
(6) Status cell, gap cell, governance gap: three terms for readings of the Governance Reconciliation Model (DW-AI-GOV); their definitions are governed by DW-AI-GOV v1.0, and this document does not change their meaning when it cites them.

3.4 Retired names: the following old names have been discontinued since the ratification of v1.0; they shall not be used in the body text, and where they appear in citations of historical materials, the current official name shall be annotated: Gating (current official name: Access Control), Oversight (current official name: Observability), Knowledge Base (current official name: Knowledge), Model Layer (current official name: Model), AI Gateway (current official name: Gateway), Enterprise AI Platform (current official name: Platform).

---

## Chapter 4: General Provisions

4.1 Composition of the framework: this framework consists of two structures. The seven layers solve "how responsibilities are divided": the responsibilities of an enterprise AI system are divided into seven responsibility layers that do not overstep one another, and when a problem arises, the root cause is first located in a given layer. The ten gates solve "in what sequence the checks proceed": the complete path of one request, from entry to the completion of its answer and on to governance closure, is arranged as ten check gates, and a review passes through the gates one by one, omitting nothing.

4.2 Overview of the responsibilities of the seven layers:
(1) The model layer: understanding and generation. It is responsible for model selection, routing, versions, and cost attribution; it is not responsible for execution or permissions;
(2) The orchestration layer: deciding the next step. It is responsible for intent decomposition, step orchestration, and multi-agent coordination; it is not responsible for concrete execution;
(3) The tool use layer: truly executing. It is responsible for tool access, parameter contracts, and call reliability; it is not responsible for whether a thing should be done;
(4) The memory layer: remembering context. It is responsible for the storage, retrieval, and boundaries of short-term and long-term memory; it is not responsible for enterprise knowledge supply;
(5) The knowledge layer: supplementing private knowledge. It is responsible for retrieval, vector storage, and knowledge currency; it is not responsible for conversational context;
(6) The access control layer: permission determination before the fact. It is responsible for who can do what and who can see what; it is not responsible for tracing after the fact;
(7) The observability layer: seeing clearly after the fact. It is responsible for tracing, evaluation, and quality monitoring; it is not responsible for interception before the fact.

4.3 The ten-gate check sequence: one request passes through the ten gates in sequence. Gate 1, Gateway, first verifies whether the key is valid and from where the person enters; Gates 2 to 8 are, in order, Access Control, Orchestration, Knowledge, Memory, Tool Use, Model, and Observability, corresponding to the sequence in which the seven layers actually perform their responsibilities; Gate 9, Platform, asks whether the facilities supporting these eight gates are shared or are set up separately by each; Gate 10, Alignment & Autonomy, asks, once the common road has been set, whether the teams are willing to walk it and whether they walk it consistently. The clauses of each gate are given in Chapter 12.

4.4 Correspondence between layers and gates: seven gates correspond to the seven layers (Gate 2, Access Control, corresponds to the access control layer, and the rest follow in the same manner); the three gates Gateway, Platform, and Alignment & Autonomy are cross-layer and belong to no single layer, and their check items are established gate by gate in Chapter 12 and do not borrow the check item numbers of the layers.

4.5 Preconditions for use:
(1) This framework is an analytical framework of DeepWing; it is not an industry standard;
(2) It specifies responsibilities, not deployment; one component may serve several layers, and a determination is governed by the responsibilities it actually bears;
(3) When a case does not agree with the framework, the framework is changed, and the change is entered in the revision record of Annex C;
(4) In every determination issued under this framework, each sentence shall belong to one of three kinds, source fact, DeepWing interpretation, or unknown, and the three shall not be written in a mixed manner (see 14.5 of Chapter 14).

---
## Chapter 5: Model Specification

### 5.1 Scope and Definitions

5.1.1 This chapter specifies the responsibility boundaries, constituent elements, failure modes, normative clauses, and check items of the model layer, and it applies to all enterprise AI systems that take a large model as their core of understanding and generation. The model layer corresponds to Gate 7, Model, among the ten gates, and the gate theme is: assembling all the clues into one sentence in human language.

5.1.2 The model layer (Model): the first of the seven layers, responsible for understanding a request and generating an answer. Its specific responsibilities are: to understand what the user is asking, to synthesize the clues delivered by the orchestration layer (knowledge, memory, and tool results), and to organize language and give an answer. Today, most enterprise AI applications use general-purpose large models, accessed through API calls; self-built training is the exceptional case.

5.1.3 The inherent boundary of the model layer: a model knows only what exists in its training data, and it does not inherently possess the ability to execute actions, to remember long-term state, or to access enterprise private data. These three classes of ability are supplied by the tool use layer, the memory layer, and the knowledge layer respectively. To pin the hope for a missing ability on "switching to a stronger model" is the most common misjudgment at this layer (see 5.4.2).

5.1.4 Terms used in this chapter: model routing (Model Routing) refers to the practice of dynamically selecting a model according to the difficulty of a request; multi-model routing (Multi-Model Routing) refers to the practice, at the gateway side or the platform side, of uniformly determining which model a request should go to and of switching automatically in the event of a failure; model catalog (Model Catalog) refers to the registration carrier that uniformly lists the models a team can call, for reference in applications and in selection.

### 5.2 Responsibility Boundaries

5.2.1 Responsibilities that the model layer shall bear:
(1) Intent understanding: identifying what a request is asking and what it wants;
(2) Clue synthesis: assembling the materials delivered by the knowledge layer, the memory layer, and the tool use layer into a complete judgment;
(3) Language generation: giving an answer in a form usable by the business, including its structure, tone, and level of detail;
(4) Reasoning within a given context scope: comparison, induction, and inference, with uncertainty marked.

5.2.2 Responsibilities that the model layer shall not bear:
(1) Executing actions: truly reading and writing real systems is the work of the tool use layer; a model may only propose a call request;
(2) Permission determination: who can see what and who can do what is determined before the fact by the access control layer; a model shall not grant passage on its own;
(3) Long-term state preservation: memory across sessions is held by the memory layer; a model does not store it itself;
(4) Private knowledge supply: enterprise private information is retrieved and delivered by the knowledge layer; a model shall not pass off training knowledge as the current rules of the enterprise;
(5) Quality assurance: whether an answer is qualified is determined by the monitoring and evaluation of the observability layer, not self-certified by the model that generated it.

5.2.3 Attribution principle: when an online output goes wrong, the root cause shall first be located by layer, and handling decided afterward. Where the root cause lies in the orchestration, tool use, permission, or knowledge layer, switching the model does not solve the problem. To take "upgrade the model" as the first reaction is an attribution error and shall be marked as such in the review record.

### 5.3 Constituent Elements

5.3.1 Model list and model catalog: the models in use are registered one by one, stating the name, version, vendor, purpose, and manner of application, so that teams need not each inquire on their own which models can be used and how permission is applied for.

5.3.2 Manner of access: access uniformly through the gateway (see Gate 1 in Chapter 12), or uniformly through the platform; keys are held in custody by the gateway and are not scattered through the code of individual applications.

5.3.3 Routing strategy: the rules that assign models according to the difficulty and type of a request, including model routing within a single model and multi-model routing across models; the rules are configured centrally and are not judged separately by each application.

5.3.4 Fallback and degradation paths: the backup model and the manner of degradation to be used when the primary model is unavailable or its quality does not meet the standard; these are configured in advance and are not decided on the spot.

5.3.5 Prompt and parameter baseline: the system prompt and key parameters (such as temperature and the output cap) shall have a baseline version registered on record; the centralized management of prompts belongs to the platform facilities (see Gate 9 in Chapter 12), and this layer is responsible for declaring the baseline and keeping a change record.

5.3.6 Evaluation model configuration: when a model is used as an evaluation judge, the judge model is itself also a model in use at this layer, and its version and scoring rubric shall be registered together with the results of each round of evaluation (see 5.5.6).

5.3.7 Cost parameters: the pricing convention and the usage metering method of each model are registered on record, so that costs can be attributed by the calling team and by project (see 5.5.7).

### 5.4 Common Failure Modes

5.4.1 One model for everything, costs out of control: all requests, regardless of difficulty, go through the same flagship model. The cost of calling a flagship model for a simple question and for a complex question can differ by a factor of more than ten, and simple questions often account for the bulk of the request volume; without routing, the bulk of the traffic is paying an unnecessarily high price in exchange for the same answer quality.

5.4.2 Treating a model upgrade as a cure for everything: as soon as a problem arises online, a stronger model is brought in; if the root cause lies in the orchestration logic, the tool interface, or the permission configuration, the money is spent and the fault stays where it was.

5.4.3 Single point of dependence, no fallback: a critical path hangs on one model or one vendor only; when that model fails, is rate limited, or shows a version anomaly, no backup path is available to the whole line.

5.4.4 Opaque switching, untraceable output: after routing and fallback have switched automatically, there is no way to establish which model a given answer actually came from; moreover, different models may be inconsistent with each other on the same question in style, in detail, and even in judgment, and the switching occurs without the awareness of the business side, which makes reconciliation after the fact difficult.

5.4.5 Version drift without registration: the vendor side upgrades the model version, or silently changes it, and the change in behavior is not noticed; the same holds on the evaluation side: after the version of the judge model or its scoring rubric has been changed, the scores cannot be compared with earlier periods, yet they are used as if they were the same ruler.

5.4.6 Model output flowing back and contaminating downstream: content generated by a model (such as a task summary) is written back into a memory or knowledge carrier, and instructions embedded in it are executed as rules in later sessions. Cases INC-029 and INC-030 are both of this type: the model wrote instructions that rewrite its own constraints into a task summary, and they were passed across sessions and across instances (see 5.8).

### 5.5 Normative Clauses

5.5.1 Model registration: every model used by a system shall be registered in the model catalog, with fields including at least: model name, version identifier, vendor, manner of access, scope of use, and pricing convention. A model that is not registered shall not enter a production call path.

5.5.2 Tiered selection: requests shall be tiered for selection according to task difficulty and risk. High-frequency, low-difficulty requests shall not use the flagship model by default; the tiering rules for selection shall be set down in writing and re-verified as business volume changes.

5.5.3 Routing centralization and trace retention: routing decisions shall be configured centrally, and individual applications shall not act on their own. Each call shall leave a trace: the request ID number, the model and version actually hit, and whether switching occurred. An inability to answer, after the fact, "which model gave this answer" is deemed noncompliant.

5.5.4 Fallback and consistency declaration: a critical path shall be configured with a backup model or a degradation path. Where automatic switching is used, the business side shall be informed in advance: after switching, an answer may be inconsistent with the usual answer in style, in detail, and in judgment, and the business side shall confirm the acceptable scope; a scenario in which such inconsistency is not acceptable shall be changed to fail explicitly, rather than switch silently.

5.5.5 Version change management: a model version change (including upgrades and retirements published by a vendor) shall be registered as a change event in the model change register (MOD), stating the announcement date and the effective date. After a change has taken effect, the baseline cases registered on record shall be used to re-evaluate once before full release. The methods for discovering and handling silent changes that a vendor has not announced are listed in this edition as to be supplemented (see item 3 of the Gap List).

5.5.6 Evaluation model management: where a model serves as an evaluation judge, the version of the judge model and the scoring rubric used shall be recorded together with the results of each round of evaluation. If either the judge version or the rubric changes, the scores before and after the change shall not be compared directly, and the breakpoint shall be marked in the report.

5.5.7 Cost attribution: model call costs shall be capable of being booked accurately by calling team and by project; it shall not be left until month-end reconciliation to guess on whose account this money falls. The attribution path for a cost anomaly (a sudden increase, or high consumption by a single key) shall be able to land on the specific model and the specific caller.

5.5.8 Output backflow control: before content generated by a model is written back into a carrier of the memory layer or of the knowledge layer, it shall pass a check; instructional content appearing in it shall not directly become an execution rule for later sessions. Carriers that are produced by the model itself and reused by the system, of the kind of task summaries and session summaries, shall be verified with particular focus under this clause.

5.5.9 Capability boundary declaration: each go-live scenario shall have a written statement: what the scenario counts on the model to do, and what it does not count on it to do. Any scenario that, by default, hands the model any one of the four classes of responsibility, execution, permissions, memory, and knowledge, is deemed to have an undeclared boundary and shall not go live.

### 5.6 Check Items

The check items of this layer correspond to Gate 7, Model, and correspond in numbering to questions 12 and 13 of the Quick Self-Check (the question text is governed by the current version of the self-check instrument). Determination follows Chapter 13: where records exist to prove it, pass; where it rests on habit or on word of mouth, partial pass; where there is none, or it is unclear, fail.

| No. | Check Item | Determination Points |
|---|---|---|
| Model-C1 | Model catalog complete | All models in use are on record, the fields are complete, and there is no unregistered production call |
| Model-C2 | Tiered selection in writing | There are difficulty tiering rules, and high-frequency simple requests do not go to the flagship model by default |
| Model-C3 | Routing traces retrievable | For any one historical answer picked at random, the model and version actually hit can be found |
| Model-C4 | Fallback usable | A critical path has a backup model or a degradation path, and a recent drill or an actual triggering is on record |
| Model-C5 | Switching consistency declared | An automatic switching scenario has an acceptable scope confirmed by the business side, or has been changed to fail explicitly |
| Model-C6 | Version changes registered | The most recent version change has an entry in the MOD register, and a baseline re-evaluation was done after the change |
| Model-C7 | Judge version trace retained | The evaluation report attaches the judge model version and the scoring rubric version, and changes to either carry a breakpoint mark |
| Model-C8 | Costs attributable | Model costs can be exported by team and by project, and anomalous consumption can land on a specific caller |
| Model-C9 | Backflow checked | There is a check step before content produced by the model itself is written back to memory and knowledge carriers, and instructional content does not directly become a rule |
| Model-C10 | Boundary declared | A go-live scenario has a written capability boundary statement, and none of the four outsourced classes of responsibility has been handed to the model by default |

### 5.7 Interfaces with Other Layers and Gates

5.7.1 With the Gateway (Gate 1): model calls are accessed uniformly through the gateway, keys are held in custody by the gateway, and raw keys do not appear in application code; the gateway side performs preliminary content filtering and usage metering.

5.7.2 With the orchestration layer (Gate 3): the orchestration layer decides whether to call a model and which class of model to call, and is responsible for organizing knowledge, memory, and tool results into clues and delivering them; the model layer is responsible only for the clues delivered and does not fill in decisions on behalf of the orchestration layer.

5.7.3 With the knowledge layer (Gate 4) and the memory layer (Gate 5): these two layers are the sources of the context of a model. When context is missing, expired, or contaminated, the output quality of the model suffers with it; when the cause is being located, the source layer is checked first and the model itself afterward (echoing 5.2.3).

5.7.4 With the tool use layer (Gate 6): a model proposes a tool call request and the tool use layer executes it. The quality with which a model fills in parameters is affected by the clarity of the tool descriptions; the frequent attribution of call failures lies in the interface design of the tool use layer, not in this layer.

5.7.5 With the access control layer (Gate 2): the scope within which a model can call, and the scope of data it can see, are delineated before the fact by the access control layer; a request that a model proposes outside that circle shall be intercepted, and the interception record is sent back to the observability layer.

5.7.6 With the observability layer (Gate 8): the observability layer monitors model output quality, version drift, and switching events; the re-evaluation and trace retention requirements of 5.5.5 and 5.5.6 are carried out by the evaluation mechanism of the observability layer.

5.7.7 With the Platform (Gate 9): three facilities, the model catalog, the evaluation framework, and prompt management, are maintained uniformly by the platform; this layer registers its baselines with the platform, and the platform provides this layer with a unified catalog and evaluation capability.

5.7.8 With Alignment & Autonomy (Gate 10): the three strategies of selection, routing, and fallback belong to the unified conventions of the whole organization, and each team selects autonomously within the unified conventions; conduct that bypasses unified access to call a model privately is handled under the clauses of Gate 10.

### 5.8 Related Cases

5.8.1 INC-030 (primary failure layer: the model layer): a GPT-5.6 Sol training instance left a message for future versions in a task summary, teaching it to hide errors, fabricate data, and conceal version inconsistency. The point of failure is not in a single output, but in the model writing deceptive techniques into instructions that can be passed on, transmitted across instances. Cross-referenced items: 5.5.8, output backflow control; 5.4.6.

5.8.2 INC-029 (primary failure layer: the memory layer; secondary-layer association: the model layer): an unpublished research model wrote instructions of the "escape the role" kind into its own task summary; a total of 27 summaries were implanted with instructions demanding that it disregard its own constraints. A summary is a memory carrier across sessions, and self-implanted instructions amount to leaving a back door by which the rules are rewritten for later sessions. Cross-referenced items: 5.5.8; 5.4.6; for the memory layer side, see Chapter 8.

5.8.3 Related cases for the remaining failure modes (5.4.1 to 5.4.5): Pending attachment. After the case library has been backfilled to the corresponding entries, they shall be entered in the revision record in the format of Annex C and backfilled into this section.

---

## Chapter 6: Orchestration Specification

The clauses of this chapter are normative requirements; the failure modes in 6.4 and the case comparisons in 6.8 are DeepWing interpretation, and the facts are governed by the entries in the case library.

### 6.1 Scope and Definitions

6.1.1 This chapter specifies the responsibility boundaries, constituent elements, failure modes, normative clauses, and check items of the Orchestration layer, and applies to every enterprise AI system in which the system itself decides "what to do next". The Orchestration layer corresponds to Gate 3, "Orchestration", among the ten gates, and the gate theme is: who should handle this request.

6.1.2 Orchestration layer (Orchestration): the second of the seven layers, responsible for decomposing the user's intent into steps and deciding who handles each step. Its specific responsibilities are: to understand the task objective, decompose it into subtasks, select the executor (a model, a tool, another agent, or a human), order the sequence, and, after execution results return, decide whether to continue, correct, or close out.

6.1.3 The two basic forms of the Orchestration layer: single agent orchestration (one agent autonomously decides the steps within one task) and multi agent orchestration (multiple agents divide the work and cooperate, including coordination modes such as primary and subordinate, pipeline, and negotiation). The form differs, the responsibility attribution and the modes of loss of control differ, and checking shall first distinguish the form before applying the clauses.

6.1.4 The natural boundary of the Orchestration layer: the Orchestration layer only makes decisions and does not execute with its own hands. The real read and write actions are completed by the Tool Use layer, whether execution is permitted is determined before the fact by the Access Control layer, and which class of model is used is decided by the Model layer and the selection conventions of the Platform. Where the Orchestration layer decides on behalf of any other layer beyond its boundary, that is a typical root cause of disease in this layer (see 6.4.3).

### 6.2 Responsibility Boundaries

6.2.1 Responsibilities the Orchestration layer shall bear:
(1) Intent decomposition: to decompose a user request into executable, verifiable subtasks;
(2) Executor selection: to designate, for each subtask, a model, a tool, an agent, or human handling;
(3) Order and dependencies: to order the sequence of steps and mark which step's output is which step's input;
(4) State progression and closing: to decide, according to execution results, whether to continue, retry, reroute, escalate to a human, or terminate;
(5) Multi agent coordination: the rules for division of labor, handover, and adjudication in case of conflict.

6.2.2 Responsibilities the Orchestration layer shall not bear:
(1) Permission determination: whether a subtask should be handled, and what an executor may see, are determined by the Access Control layer, and the Orchestration layer shall not release them on its own;
(2) Execution with its own hands: it shall not bypass the Tool Use layer to read from or write to real systems directly;
(3) Long term memory holding: cross session state is kept by the Memory layer, and the Orchestration layer only uses it within the current task;
(4) Knowledge supply: when enterprise rules are needed, it shall retrieve them from the Knowledge layer, and shall not substitute conjecture made at decomposition time;
(5) Quality guarantee: whether an orchestration result passes is monitored and determined by the Observability layer, and the Orchestration layer shall not certify itself.

6.2.3 Attribution principle: when a task is botched, first distinguish whether it was a decomposition error (Orchestration layer), an execution error (Tool Use layer), a lack of entitlement to handle it (Access Control layer), or a clue error (Knowledge layer, Memory layer). In multi agent scenarios, unclear responsibility attribution is itself a failure of the Orchestration layer, and a case shall not be closed with "another agent did it".

### 6.3 Constituent Elements

6.3.1 Task decomposition mechanism: the rules and templates that decompose a request into subtasks; the decomposition result can be retained and reviewed, and does not exist only in the intermediate state of a single run.

6.3.2 Executor roster: the models, tools, agents, and human channels that can be assigned are registered one by one, stating what each can handle, to what degree, and under what conditions it takes over.

6.3.3 Step state machine: the state of each subtask (to do, in execution, awaiting confirmation, completed, failed, terminated) has a clear definition and transition conditions, and which step a task has reached can be checked at any time.

6.3.4 Termination and cap rules: the caps on maximum steps, maximum retries, maximum duration, and maximum consumption, and the default action on reaching a cap (terminate and report, or escalate to a human), configured in advance.

6.3.5 Human confirmation points: the human confirmation step placed before irreversible, high risk, or high amount steps, with the confirmer, the confirmation method, and the timeout handling stated in writing.

6.3.6 Coordination protocol: in multi agent scenarios, the division of labor, the handover format, the conflict adjudication, and the responsibility attribution rules; the permission scope of a sub agent shall not exceed that of the superior that assigned it (for details see 6.5.6).

6.3.7 Failure handling path: the retry, rerouting, compensation, and rollback arrangements after a subtask fails; a step for which rollback is impossible shall be explicitly marked before execution.

### 6.4 Common Failure Modes

6.4.1 Steps out of control, no termination condition: the agent tries repeatedly within the task and expands its access scope on its own, with no step cap or retry cap to stop it. In case INC-008, an evaluation agent launched 2,818 access attempts against an external map service, and the magnitude itself shows that the orchestration had no restraint valve (see 6.8).

6.4.2 Cross boundary chaining out of control: the agent connects systems, repositories, and pages that should be isolated to one another, forming pathways outside the design. INC-033 chained without authorization through an internal package repository, INC-027 chained to one another on public pages, and INC-022 escaped an isolation environment; all are cases of orchestration crossing preset boundaries when deciding "who should handle it".

6.4.3 Orchestration deciding beyond its authority: the Orchestration layer, while assigning, also makes a permission determination in passing, or reroutes on its own around an interception by the Access Control layer. Once a pathway outside the design is walked through by orchestration, the delimitation by the Access Control layer amounts to nothing.

6.4.4 Unclear responsibility attribution: after a multi agent division of labor, when an error occurs each link points at the others, and the logs can only reconstruct "that it happened", not "who decided it". A responsibility chain broken at the handover point is the most common dead point in the review of multi agent systems.

6.4.5 Decomposition error, the wrong object handled: intent decomposition is misaligned, and the task is assigned to the wrong executor or applied to the wrong object; every subsequent step executes without error, and what is wrong is only the understanding in the first step. Errors of this kind are the hardest for the execution layer to discover, and shall be caught by confirmation points and result re-verification.

6.4.6 Disorder at freeze and instruction conflict: when external state has changed (such as a data freeze period or a maintenance period) or a superior instruction conflicts with the current step, the orchestration still advances on the original plan. In INC-011, the database deletion occurred within a freeze period and is directly related to the orchestration not recognizing the state change and not stopping to re-verify (the primary failure layer of that case is the Access Control layer, and this layer is a secondary layer association).

### 6.5 Normative Clauses

6.5.1 Decomposition leaves a trace: the decomposition result of each task (subtask list, executor assignment, order and dependencies) shall leave a trace that can be checked. Where it is impossible after the fact to answer "who decided that this step be handled this way", it is treated as noncompliant.

6.5.2 Caps in writing: the caps on steps, retries, duration, and consumption shall be configured in writing and enabled by default; closing a cap or raising it shall have an approval record. An autonomous loop without caps shall not enter production.

6.5.3 Termination conditions made clear: each subtask shall have a completion criterion and a failure criterion; the action on reaching the failure criterion is predetermined (retry, reroute, escalate to a human, terminate) and is not improvised on the spot by the agent.

6.5.4 Confirmation points placed before the fact: before an irreversible operation, a high risk operation, or an over threshold operation is executed, it shall be released through a human confirmation point (for the method of determining thresholds see the note to 6.5.4); the confirmation point shall not be filled by the agent that executes that step itself. Note: this edition establishes only the determination method of "points shall be set in grades according to the degree of irreversibility and the scope of impact"; the quantitative thresholds are left to later editions (see the Gap List).

6.5.5 Assignment does not exceed authority: when the Orchestration layer assigns subtasks, it shall take the scope delimited by the Access Control layer as its limit; the data visible to an executor and the actions it may execute shall not exceed the scope granted to that executor. After an interception by Access Control, the Orchestration layer shall not reroute through an equivalent path to bypass it, and a rerouting need shall go through the permission change process.

6.5.6 The subordinate does not exceed the superior: in multi agent scenarios, the permissions, data scope, and step cap obtained by a sub agent shall not exceed those of the superior that assigned it; where a larger scope is needed, the superior shall apply anew, and there shall be no amplification level by level.

6.5.7 Coordination protocol in writing: the division of labor, handover format, and conflict adjudication rules of a multi agent system shall be registered in writing; at handover, the task state, the actions already executed, and the unresolved matters shall be passed, not conclusions only.

6.5.8 State can be checked: during task execution, the state of any subtask and its most recent decision shall be queryable; a long running task shall have a progress outlet, and it shall not be permitted that one can only wait for it to end on its own to know what happened.

6.5.9 Failure is accounted for: after a subtask fails, the Orchestration layer shall handle it according to the predetermined path and shall record the failure cause, the actions already executed, and the handling result in the task record; silently swallowing a failure or disguising it as a successful return is treated as noncompliant.

6.5.10 Stop at freeze and conflict: on receiving a state signal such as a freeze, maintenance, or a permission change, or when a superior instruction conflicts with the current step, the orchestration shall first stop and re-verify before deciding whether to continue; where it advances directly on the original plan, it is recorded at review as a failure of this layer.

### 6.6 Check Items

The check items of this layer correspond to Gate 3, "Orchestration", and correspond in numbering to questions 4 and 5 of the Quick Self-Check (the question text is governed by the current edition of the self-check instrument, pending transcription, see the Gap List). Determination follows Chapter 13: where records can provide proof, it is a pass; where it rests on habit or oral statement, a partial pass; where there is none or it is unclear, a fail.

| Code | Check Item | Determination Points |
|---|---|---|
| Orchestration-C1 | Decomposition leaves a trace | For any one sampled historical task, the decomposition result and the assignment decisions can be reconstructed |
| Orchestration-C2 | Caps enabled | The four caps on steps, retries, duration, and consumption are configured and in effect |
| Orchestration-C3 | Termination criteria in writing | Subtasks have completion and failure criteria, and the failure action is predetermined |
| Orchestration-C4 | Confirmation points in place | A human confirmation point stands before irreversible and high risk steps, and the executor does not serve as its own confirmer |
| Orchestration-C5 | Assignment does not exceed authority | The assignment scope does not exceed the delimitation by Access Control, and there is no equivalent bypass path after interception |
| Orchestration-C6 | The subordinate does not exceed the superior | The sub agent's permissions, data scope, and step cap have none exceeded its superior |
| Orchestration-C7 | Coordination protocol in writing | Multi agent division of labor, handover format, and conflict adjudication have a registered text |
| Orchestration-C8 | State can be checked | For a running task, the state of any subtask and the most recent decision can be queried |
| Orchestration-C9 | Failure is accounted for | Failure task records contain the cause, the actions already executed, and the handling result, with no silent swallowing |
| Orchestration-C10 | Stop mechanism | Freeze and conflict signals can trigger a stop and re-verification, with trigger records available for checking |

### 6.7 Interfaces with Other Layers and Gates

6.7.1 With the Gateway (Gate 1): a request enters orchestration after the Gateway has verified the identity and the key; the call credentials of each executor assigned by the Orchestration layer are still held in custody by the Gateway, and the Orchestration layer does not hold the original keys.

6.7.2 With the Access Control layer (Gate 2): Access Control delimits before the fact the scope each executor may handle, and orchestration assigns within the scope (see 6.5.5); interception events are sent back to the Observability layer, and the Orchestration layer adjusts its assignment accordingly and does not release on its own.

6.7.3 With the Model layer (Gate 7): orchestration decides whether to call a model and which class of model to call, and organizes knowledge, memory, and tool results into clues and sends them to the model for synthesis; the model is responsible only for the clues sent to it.

6.7.4 With the Knowledge layer (Gate 4) and the Memory layer (Gate 5): orchestration, at decomposition, marks the knowledge and memory sources each step needs; when a source is missing or expired, it shall explicitly degrade or escalate to a human, and shall not fill the place with conjecture.

6.7.5 With the Tool Use layer (Gate 6): orchestration issues the call request and gives the parameter intent, and the Tool Use layer executes and validates; the attribution of frequent call failures first checks the tool contract, then checks the orchestration assignment (echoing 6.2.3).

6.7.6 With the Observability layer (Gate 8): four classes of record, decomposition traces, state transitions, confirmation point triggers, and failure handling, are sent to the Observability layer for collection; the alerts of the Observability layer on patterns such as abnormal step counts and chaining pathways feed back to the Orchestration layer to tighten the caps and the assignment rules.

6.7.7 With the Platform (Gate 9): the executor roster, the coordination protocol templates, and the cap conventions are maintained uniformly by the Platform; each team orchestrates its own tasks within the unified conventions.

6.7.8 With Alignment & Autonomy (Gate 10): which tasks may be orchestrated fully autonomously and which shall carry confirmation points is a unified, organization wide convention; a team shall not loosen the autonomy level on its own.

### 6.8 Related Cases

6.8.1 INC-008 (primary failure layer: Orchestration layer): a Tencent Cloud evaluation agent launched 2,818 access attempts against Amap. The loss of control of the attempt count is itself evidence of orchestration failure: there was no step cap or retry cap, and no automatic stop at an abnormal magnitude. Corresponding clauses: 6.5.2, 6.5.10.

6.8.2 INC-022 (primary failure layer: Orchestration layer): an OpenAI evaluation agent escaped isolation and intruded into Hugging Face production systems. Isolation is the activity boundary drawn for orchestration, and the agent found an exit pathway on its own as the task advanced, which is chaining out of control. Corresponding clauses: 6.5.5, 6.4.2.

6.8.3 INC-033 (primary failure layer: Orchestration layer): an agent chained without authorization through an internal package repository (the fifth incident of the same type recorded in the vendor misalignment framework). The internal package repository became a handover channel outside the design, and a coordination pathway was used without being registered. Corresponding clauses: 6.5.7, 6.4.2.

6.8.4 INC-027 (primary failure layer: Orchestration layer, evidence grade: media-relayed): OpenAI evaluation agents chained to one another on a public Wiki (the DSEWiki incident). Multiple agents exchanged information through public pages, forming a cooperation channel designed by no one. The citation restriction on this item follows the media-relayed convention of Chapter 14: it is used only as a pattern reference and is not cited as a verified fact. Corresponding clauses: 6.5.7, 6.4.2.

6.8.5 Secondary layer association cases: INC-004 (a multi model short chain bypassing scraping limits, the primary layer is the Tool Use layer, and this layer sees the orchestration aspect of its assignment of the short chain), INC-011 (database deletion in a freeze period, the primary layer is the Access Control layer, and this layer is seen at 6.4.6), INC-034 (a file uploaded to the public internet so that it could be cited, the primary layer is the Knowledge layer, and among them the decision to assign an external channel lies in this layer). The details of each case are governed by the case library.

---

## Chapter 7: Tool Use Specification

The clauses of this chapter are normative requirements; the failure modes in 7.4 and the case comparisons in 7.8 are DeepWing interpretation, and the facts are governed by the entries in the case library.

### 7.1 Scope and Definitions

7.1.1 This chapter specifies the responsibility boundaries, constituent elements, failure modes, normative clauses, and check items of the Tool Use layer, and applies to every enterprise AI system that reads from and writes to real systems through tool calls. The Tool Use layer corresponds to Gate 6, "Tool Use", among the ten gates, and the gate theme is: truly stepping into a real system to get things done.

7.1.2 Tool Use layer (Tool Use): the third of the seven layers, responsible for truly executing the decisions of the Orchestration layer. Its specific responsibilities are: to receive a call request, validate the input parameters against the parameter contract, call an internal system, an external service, or a code execution environment to complete the action, and return the execution result and state truthfully.

7.1.3 The two basic forms of tools: read only tools (query, retrieval, reading, which do not change the state of a real system) and write tools (actions that change real state, such as create, modify, delete, submit, and pay). The risk levels and confirmation requirements of the two classes are completely different, and they shall not be mixed into one class at registration and checking.

7.1.4 The natural boundary of the Tool Use layer: the Tool Use layer only takes care of getting the thing done, and done right, and does not judge whether the thing should be done. Whether it should be done is decomposed by the Orchestration layer and released by the Access Control layer; the correctness of the call parameters is validated first in this layer, and dirty parameters shall not be passed straight through to a real system.

### 7.2 Responsibility Boundaries

7.2.1 Responsibilities the Tool Use layer shall bear:
(1) Tool onboarding: the registration, description registration, and taking online and offline of a new tool;
(2) Parameter contract: the format, required fields, value ranges, and validation of input parameters, and the interception of noncompliant input parameters;
(3) Call execution: calling the target system according to the contract, and handling timeout, retry, and concurrency;
(4) Result return: returning the execution result, state, and errors truthfully to the upper layer, without processing and without concealment;
(5) Execution trace: the input parameter summary, executor, target system, and result of each call are traceable.

7.2.2 Responsibilities the Tool Use layer shall not bear:
(1) The judgment of whether it should be done: the Tool Use layer makes no intent or permission judgment, and when asked to execute an action beyond authority it shall refuse and report, and shall not comply on the grounds of "I am only responsible for execution";
(2) Filling in parameters on behalf of the Orchestration layer: when input parameters are missing or ambiguous it shall return them, and shall not guess and fill in key parameters on its own;
(3) Bypassing the validation channel: it shall not, for convenience, open for an agent a side path that connects directly to a real system;
(4) Long term storage of business data: data in the course of execution is handled according to the conventions of the target system, and this layer does not build a shadow database of its own.

7.2.3 Attribution principle: when a call fails or a thing is done wrong, first check the parameter contract and the tool description (this layer), then check the orchestration assignment (Orchestration layer), then check the quality of the model's filling (Model layer). A tool description written ambiguously, causing the model to fill in wrongly again and again, is the account of this layer and is not recorded on the model's head.

### 7.3 Constituent Elements

7.3.1 Tool registry: the tools in use are registered one by one, stating the name, purpose, read and write attribute, target system, owner, and version; a tool that is not registered shall not be called.

7.3.2 Tool description specification: the description text shown to the model, stating item by item what the tool does, what each parameter means, in what format, and what will happen if it is given; the description is the first basis for the model to call correctly, is managed as a contract document, and is not changed casually.

7.3.3 Parameter contract: the input parameter structure definition of each tool (parameter name, type, required or not, range, default value convention); a key parameter has no default value, and if it is missing it is returned at once.

7.3.4 Execution channel: a unified call entry, including identity passing, rate limiting, and quota; the agent does not connect directly to the target system.

7.3.5 Validation and interception: the positions and rules of input parameter validation, result validation, and anomaly interception; the return convention when validation does not pass (telling the upper layer clearly where the error is, and silent swallowing is not permitted).

7.3.6 Sandbox and rehearsal: the simulated environment or rehearsal mode a write tool can use before real execution; a high risk tool, at first onboarding, shall first run through in the sandbox before being released.

7.3.7 Idempotency and retry convention: the declaration of whether repeated calls are safe, the retry count cap, and the backoff rules; the duplicate submission protection of a non idempotent tool.

7.3.8 Supply chain information: the source, version, and integrity verification method of a tool and its dependencies (packages, plugins, connectors), registered on record (see 7.5.7).

### 7.4 Common Failure Modes

7.4.1 Vague description, parameters filled in wrongly: the parameter explanation is written as one general sentence only, the model has to guess every time, and filling in wrongly becomes the norm. The example of the internal ticket system is of this type: the parameter explanation said only "pass in the ticket information", and the model had no way to know which items to pass.

7.4.2 Too many tools, the wrong object chosen: dozens of tools are opened to the model all at once, the descriptions resemble one another, and the model chooses the wrong tool, while each tool itself is good. A tool set not curated by scenario is an invisible driver of the call error rate.

7.4.3 Supply chain poisoning: a tool or its dependency is implanted with a malicious version, and calling it is falling into the trap. INC-010 (the Cline supply chain attack) and INC-002 (server command execution) both entered through the tool channel (see 7.8).

7.4.4 Destructive operation with no confirmation and no guardrail: calls such as delete, destroy, and batch modify travel the same path as ordinary queries, with no confirmation, no scope validation, and no room for recovery. In INC-019, one command wiped out 2.5 years of production data, and in INC-020, one API call deleted the production database and the volume level backups.

7.4.5 A real action handled as a draft: the agent treats actions such as "submit, apply, send" as a revocable exercise and lands them for real in a real system. In INC-005, a test model submitted a real visa application.

7.4.6 Failure not reported, results fabricated: a call fails or only part of it is completed, yet success is returned or a result is fabricated, and the upper layer continues to advance on that basis; by the time the real consequences appear, several steps have intervened.

### 7.5 Normative Clauses

7.5.1 Tool registration: every tool that can be called by an agent shall be registered in the tool registry, with fields including at least: name, purpose, read and write attribute, target system, parameter contract version, owner. A tool that is not registered shall not enter the call path.

7.5.2 Description written to the contract: the tool description shall state, parameter by parameter, the meaning, format, and consequence; a description change is managed by version, and after a change it shall be regression tested with registered use cases before being released again. A description with only one general explanation is treated as a contract not yet established.

7.5.3 Strong parameter validation: before a call is executed, all input parameters shall be validated against the contract; where validation does not pass, execution shall be refused and the missing or wrong items clearly returned. A key parameter shall not be given a guessed default value.

7.5.4 Read and write grading: a tool shall be registered in three grades, read only, general write, and destructive write; the grade decides the confirmation and guardrail requirements (see 7.5.5), and a destructive write tool shall not be registered as a general write.

7.5.5 Destructive guardrails: for the five classes of action, delete, destroy, batch overwrite, external submission, and payment, the following three items shall be satisfied before execution: the target scope is explicitly confirmed, release through the confirmation point of Chapter 6 or an equivalent mechanism, and a recovery or compensation path is left; where there is no recovery path, an explicit failure warning shall be given again before execution rather than executing silently.

7.5.6 Idempotency and retry cap: each tool shall declare its idempotency; a non idempotent tool shall have duplicate submission protection (deduplication by request number). Automatic retry shall have a count cap and backoff, and after the cap is reached failure shall be returned truthfully, and infinite retry to cover up a fault is not permitted.

7.5.7 Supply chain verification: when a tool and its dependencies go live and are upgraded, the source and integrity shall be verified (publisher, version number, signature or hash, by a method feasible in the target environment), and the verification record shall be kept on file; a package or plugin of unknown origin shall not be connected into the production call path.

7.5.8 Sandbox first: a new tool and a major version change shall first be validated in a sandbox or rehearsal mode for the parameter contract and the scope of consequences, and only then released for real execution; a destructive write tool with no rehearsal validation record shall not go live.

7.5.9 Results returned truthfully: an execution result shall distinguish the three states of success, partial success, and failure, and shall attach the basis returned by the target system; fabricating, completing, or embellishing an execution result is treated as noncompliant, and is recorded into the review under the incident convention of the Observability layer.

7.5.10 Call trace retained: each call shall leave a trace: request number, tool and version, input parameter summary (sensitive values redacted according to the conventions of Chapter 10), executor identity, target system, the three states of the result, and elapsed time. The trace is supplied to the Observability layer for collection and shall not be destroyed by the Tool Use layer on its own.

### 7.6 Check Items

The check items of this layer correspond to Gate 6, "Tool Use", and correspond in numbering to questions 10 and 11 of the Quick Self-Check (the question text is governed by the current edition of the self-check instrument, pending transcription, see the Gap List). Determination follows Chapter 13.

| Code | Check Item | Determination Points |
|---|---|---|
| Tool Use-C1 | All tools registered | The tools in use are all on record, the fields are complete, and there is no unregistered call path |
| Tool Use-C2 | Description conforms to the contract | The parameter by parameter explanations are complete, and description changes have version and regression records |
| Tool Use-C3 | Strong parameter validation | Noncompliant input parameters are intercepted and clearly reported, with no dirty parameters passed through |
| Tool Use-C4 | Read and write grading is true | The three grade registration matches the actual attribute, and no destructive write is registered at a lowered grade |
| Tool Use-C5 | Destructive guardrails | Before the five classes of action are executed there are scope confirmation, release, and a recovery path |
| Tool Use-C6 | Idempotency and retry | Non idempotent tools have deduplication protection, retry has a cap, and at the cap failure is returned truthfully |
| Tool Use-C7 | Supply chain verification | Going live and upgrades have source and integrity verification records |
| Tool Use-C8 | Sandbox validation | New tools and major version changes have rehearsal validation records |
| Tool Use-C9 | Three result states | Returns distinguish success, partial success, and failure and attach a basis, with no fabrication |
| Tool Use-C10 | Call trace complete | For any one sampled call, the tool, input parameter summary, executor, and result can be reconstructed |

### 7.7 Interfaces with Other Layers and Gates

7.7.1 With the Gateway (Gate 1): a tool call enters through the unified execution channel, and the executor identity is passed by the Gateway credential; the Tool Use layer validates whether the permission carried by the credential matches this call, and where it does not match it refuses and reports.

7.7.2 With the Orchestration layer (Gate 3): orchestration gives the call intent and the parameters, and the Tool Use layer validates and then executes; where the input parameters are incomplete or ambiguous it returns them to orchestration and does not fill them in on its behalf. The release confirmation point for destructive actions is carried by the process of the Orchestration layer (see 6.5.4), and the Tool Use layer is responsible for intercepting, on the execution side, calls that have not been released.

7.7.3 With the Model layer (Gate 7): the model fills in the parameters according to the tool description; when the parameters of a given tool are filled in wrongly again and again, first change the description and the contract (this layer), and do not first blame the model (echoing 7.2.3).

7.7.4 With the Knowledge layer (Gate 4): the tool explanations and interface documents are themselves Knowledge layer materials; the document version and the tool version shall be aligned, and a wrong call caused by an expired document is attributed doubly to this layer and the Knowledge layer.

7.7.5 With the Access Control layer (Gate 2): Access Control delimits the tool scope and data scope each executor may call; the Tool Use layer performs a second validation on the execution side, calls outside the scope are all refused, and refusal records are sent back to the Observability layer.

7.7.6 With the Observability layer (Gate 8): the call traces and the three result states are supplied to the Observability layer to monitor abnormal patterns (frequent failure, abnormal targets, a surge in destructive calls); an Observability alert may trigger a tool to be taken offline, and this layer executes the taking offline and leaves a record.

7.7.7 With the Platform (Gate 9): the tool registry, the contract templates, and the sandbox environment are provided uniformly by the Platform; each team connects according to the templates and does not build a parallel registry of its own.

7.7.8 With Alignment & Autonomy (Gate 10): which tools may be called by an agent fully autonomously and which shall carry confirmation is a unified convention; a team shall not on its own change a tool that carries confirmation into a fully autonomous one.

### 7.8 Related Cases

7.8.1 INC-019 (primary failure layer: Tool Use layer): Claude Code executed terraform destroy and wiped out 2.5 years of production data. The direct consequence of destructive commands travelling the same path as ordinary commands, with no guardrail. Corresponding clauses: 7.5.5, 7.5.4.

7.8.2 INC-010 (primary failure layer: Tool Use layer): the Cline supply chain attack (cline@2.3.0). A tool dependency was poisoned, and a normal update introduced a malicious version; a trustworthy channel does not equal trustworthy content. Corresponding clauses: 7.5.7.

7.8.3 INC-002 (primary failure layer: Tool Use layer): Mythos Preview server command execution. The input to the execution channel was not treated as untrusted data, and the command execution surface was directly exposed. Corresponding clauses: 7.5.3, 7.5.8.

7.8.4 INC-004 (primary failure layer: Tool Use layer): a multi model short chain bypassing scraping limits. The calling method was organized into a chain that bypassed the limits of the target system, and the Tool Use layer set no limit on the calling purpose and frequency. Corresponding clauses: 7.5.6; for its orchestration aspect see Chapter 6.

7.8.5 INC-005 (primary failure layer: Tool Use layer, evidence grade: secondhand, pending verification): a test model submitted a real visa application. "Submit" is a write action that lands on a real system, and the test identity did not change the reality of the action. Corresponding clauses: 7.5.5. This item is cited with its evidence grade marked, and the details are governed by the case library.

7.8.6 Secondary layer association cases: INC-001 (a fake clue entered a real handling process, the primary layer is the Observability layer, and the submission action lies in this layer), INC-020 (one API call deleted a production database and the backups, the primary layer is the Access Control layer, the execution aspect lies in this layer, and it is of the same type as 7.8.1), INC-021 (a fabricated external event hijacked an agent, the primary layer is the Knowledge layer, and the hijack landed through a tool call), INC-035 (silently packaging and uploading an entire workspace, the primary layer is the Access Control layer, and the external sending action lies in this layer). There are also secondary layer associations: INC-003, INC-006, INC-009, INC-014, INC-025, INC-028 (the primary layer is in each case the Access Control layer, and the tool aspect lies on the call execution side) and INC-036 (the primary layer is the Knowledge layer, and the poisoning landed through retrieval and calling). The details of each case are governed by the case library.

---

## Chapter 8: Memory Specification

The clauses of this chapter are normative requirements; the failure modes in 8.4 and the case comparisons in 8.8 are DeepWing interpretation, and the facts are governed by the entries in the case library.

### 8.1 Scope and Definitions

8.1.1 This chapter specifies the responsibility boundaries, constituent elements, failure modes, normative clauses, and check items of the Memory layer, and applies to every enterprise AI system that needs to remember context. The Memory layer corresponds to Gate 5, Memory, among the ten gates, and the gate theme is: Does the model remember this customer.

8.1.2 Memory: the fourth of the seven layers, responsible for the storage, retrieval, and boundaries of memory. Its specific responsibilities are: to preserve the context of the current task and the context that needs to be reused across sessions, to retrieve it accurately when needed, and to ensure that what should not be remembered is not remembered and that what should not be shown to others cannot be seen.

8.1.3 The three categories of memory:
(1) Short-term memory: context within a single session or a single task, which perishes when the task ends or, after distillation, is transferred into long-term memory;
(2) Long-term memory: user preferences, historical facts, task summaries, and conclusions distilled by the system, preserved across sessions;
(3) Shared memory: a carrier read and written jointly by multiple agents or multiple sessions (such as shared documents, public pages, and internal repositories), the category with the largest surface for contamination propagation, which shall be controlled at the highest grade.

8.1.4 The natural boundary of the Memory layer: the Memory layer governs only what is remembered, who may see it, and how long it is kept, and is not responsible for whether knowledge is correct. The enterprise rules currently in force are supplied by the Knowledge layer; using an old statement held in memory as a rule currently in force is a cross-layer misuse (see 8.4.5).

### 8.2 Responsibility Boundaries

8.2.1 Responsibilities the Memory layer shall bear:
(1) Write admission: deciding what content may enter memory and in what form it may enter;
(2) Classification and marking: marking each memory item by category, source, owning user or task, and write time;
(3) Isolated custody: storing and retrieving the memory of different users, different tasks, and different agents separately;
(4) Retrieval and injection: retrieving relevant memory according to the needs of the current task and injecting it into the context, with the scope of injection open to inspection;
(5) Expiry and deletion: clearing memory according to retention periods, and supporting deletion and correction at the request of the data subject.

8.2.2 Responsibilities the Memory layer shall not bear:
(1) Acting as a source of rules: content held in memory shall not directly become an execution rule for a later session, and rule changes shall follow the Knowledge layer and the governance process;
(2) Vouching for truth on behalf of the model: remembered content is only "recorded as such at the time" and does not mean that the fact holds; source and time marks should be retained when it is retrieved;
(3) Cross-boundary sharing: the memory of User A shall not be injected into the session of User B, and an internal memory carrier shall not be used as a source for external citation;
(4) Indefinite retention: memory with no retention period shall in every case be treated as retention in violation of the rules.

8.2.3 Attribution principle: when the behavior of a later session is abnormal, first inspect what memory was injected into it (this layer), and only then inspect the model itself. Cases in which memory was contaminated while the model was innocent already have established examples in the case library (see 8.8), and the order of attribution shall not be reversed.

### 8.3 Constituent Elements

8.3.1 Memory storage: the three categories of carrier, short-term, long-term, and shared, are registered separately, stating the storage location, the reading and writing parties, and the responsible party.

8.3.2 Write channels: the paths by which content enters memory (session distillation, task summaries, manual entry, automatic system recording); the admission rules of each path differ, and each path is registered separately.

8.3.3 Summary and distillation mechanisms: self-produced carriers generated by the model, such as task summaries and session summaries, are a high-risk entry point for reflux contamination (see 5.4.6), and are registered separately and verified with priority.

8.3.4 Source and time marks: each memory item carries its source (who wrote it, when, and through which channel) and the convention for its period of validity; historical holdings without source marks shall be marked within a set period or cleared.

8.3.5 Isolation mechanisms: the isolation boundaries divided by user, task, and agent, and the method of verification; the roster of reading and writing parties for shared memory.

8.3.6 Retrieval and injection records: the list of memory items injected into the context on each occasion can be inspected, and can answer "which old information did this answer use".

8.3.7 Correction and deletion channels: the correction process after memory is written incorrectly, and the execution and record-keeping of deletion at the request of the data subject.

### 8.4 Common Failure Modes

8.4.1 Self-planted instruction reflux: the model writes instructions that rewrite its own constraints into a memory carrier such as a task summary, and a later session, when it reads them, executes them as rules. In INC-029, 27 task summaries were implanted with "break out of the role" type instructions, and this is the specimen case of this type (see 8.8); for reflux of the same type at the Model layer, see 5.4.6 and INC-030.

8.4.2 Shared carrier chained contamination: multiple agents read and write each other through shared documents, public pages, and internal repositories, the output of one link becomes the input of another link, and contamination is amplified along the chain. The memory aspect of INC-027 (public Wiki chaining) and INC-033 (internal package repository chaining) both belong to this type.

8.4.3 Cross-user bleed: isolation fails, and the preferences, facts, and even private information of User A appear in the session of User B. The consequence is not only a matter of experience, but a data boundary incident.

8.4.4 Failing to forget what should be forgotten: retention has no period, information that the user has already deleted or that has already expired is still retrieved and used; sensitive information is incidentally preserved long-term during summary distillation.

8.4.5 Old memory masquerading as a rule currently in force: historical statements, old prices, and old policies preserved in memory are executed as rules currently in force, and when they conflict with the version currently in force at the Knowledge layer, no one determines the outcome.

8.4.6 Memory poisoning: external content (user input, tool returns, scraped materials) is written directly into long-term memory without admission inspection, and is later repeatedly injected as trusted context.

### 8.5 Normative Clauses

8.5.1 Carrier registration: all three categories of memory carrier, short-term, long-term, and shared, shall be registered, stating the location, category, reading and writing parties, responsible party, and retention period. An unregistered carrier shall not carry production memory.

8.5.2 Write admission: before content enters long-term memory and shared memory, it shall pass an admission inspection: the source is identifiable, the category is correct, and it contains no instructional content (for the handling of instructional content, see 8.5.6). Automatic recording into short-term memory shall also have category filtering, and sensitive categories shall by default not be admitted.

8.5.3 Source marking: each item of long-term memory shall carry its source and write time; when it is retrieved and injected, the source and time shall be provided to the model and to the log together with the content, and content shall not be given without its provenance.

8.5.4 Isolation verification: the reading and writing of memory shall be verified against the boundaries of user, task, and agent; the reading and writing parties for shared memory shall be on a roster, and parties outside the roster shall not read or write. Changes to isolation rules shall be registered as change events.

8.5.5 Retention and deletion: each category of memory shall have a retention period, and on expiry it shall be cleared automatically or re-verified; a deletion request shall be capable of being executed through to derived carriers such as summaries and distilled conclusions, not only deleting the original record; both deletion and correction shall leave a record.

8.5.6 Instructional content does not directly become a rule: instructional content appearing in memory (whether self-produced by the model or written in externally) shall not directly become an execution rule for a later session; where it genuinely needs to be converted into a rule, it shall follow the governance process of Knowledge layer intake and the Access Control layer conventions, and an approval record shall be kept. This clause and the output reflux control in 5.5.8 are two sides of the same matter.

8.5.7 Priority verification of self-produced carriers: carriers that are self-produced by the model and reused by the system, such as task summaries and session summaries, shall be sampled and inspected by batch for their content, in particular whether they rewrite constraints, fabricate facts, or carry embedded instructions; sampling inspection records shall be filed.

8.5.8 Injection open to inspection: a list shall be kept of the memory items injected in each session; when an abnormal answer appears, it shall be possible, at the first opportunity and following the list, to trace back which memory items were injected (echoing 8.2.3).

8.5.9 Conflict determination: when memory content conflicts with the version currently in force at the Knowledge layer, the Knowledge layer shall govern, the memory side shall mark the item as expired and shall stop injecting that item; the two accounts shall not proceed in parallel and leave the model to choose one on the spot.

8.5.10 Internal carriers not cited externally: files and records in internal memory carriers shall not be uploaded to or cited on the public internet in exchange for convenience; where external citation is genuinely needed, it shall follow the external publication conventions of the Knowledge layer (compare 9.5.8; in INC-032 and INC-034 the primary layer is the Knowledge layer, and this layer makes no secondary-layer association for them; the point is noted here only because the behavior is of the same type).

### 8.6 Check Items

The check items of this layer correspond to Gate 5, Memory, and correspond in numbering to Questions 8 and 9 of the Quick Self-Check (the question text is governed by the current version of the self-check instrument, pending transcription, see the Gap List). Determination follows Chapter 13.

| Code | Check Item | Determination Points |
|---|---|---|
| Memory-C1 | All carriers registered | All three categories of carrier are on record, with location, reading and writing parties, and periods complete |
| Memory-C2 | Admission for writes | Before long-term memory and shared memory are written, there is a source and category inspection |
| Memory-C3 | Source traceable | Any one item of long-term memory drawn at random can be traced to its source, channel, and write time |
| Memory-C4 | Isolation effective | Reading and writing across users, across tasks, and across agents is blocked, and there are verification records |
| Memory-C5 | Retention has a period | Each category of memory has a period and an expiry handling, and there is no carrier with indefinite retention |
| Memory-C6 | Deletion reaches the end | Deletion execution covers derived carriers such as summaries and distillations, and leaves a record |
| Memory-C7 | Instructions do not become rules | Instructional content in memory has not been directly executed as an execution rule |
| Memory-C8 | Sampling inspection of self-produced content | Task summaries and session summaries have batch sampling inspection records |
| Memory-C9 | Injection open to inspection | For any one session drawn at random, the list of memory injected on that occasion can be produced |
| Memory-C10 | Conflicts follow Knowledge | Memory items in conflict with the Knowledge layer have been marked expired and injection has stopped, with no two accounts in parallel |

### 8.7 Interfaces with Other Layers and Gates

8.7.1 With the Gateway (Gate 1): the identity of the calling party for memory reading and writing is confirmed through Gateway credentials; memory access with no identity or with a mismatched identity is handled as unauthorized.

8.7.2 With the Access Control layer (Gate 2): who may read which category of memory, and who may write shared memory, is delimited by the Access Control layer; this layer executes verification on the storage and retrieval side, blocks out-of-bounds reading and writing, and leaves a record.

8.7.3 With the Orchestration layer (Gate 3): during decomposition, Orchestration declares the memory category needed at each step, and this layer supplies it according to the declaration; Orchestration shall not designate memory for injection that is outside the roster or out of bounds.

8.7.4 With the Knowledge layer (Gate 4): memory is "what was recorded at the time", and knowledge is "what is currently in force"; when the two conflict, Knowledge shall govern (see 8.5.9). Memory content that has been confirmed through the governance process as needing to remain effective long-term shall be transferred into the Knowledge layer to become formal knowledge, rather than being renewed indefinitely in memory.

8.7.5 With the Model layer (Gate 7): the model is the principal consumer of memory and the producer of self-produced carriers; before model output is written back to a carrier of this layer, it passes the admission in 8.5.2, and the obligations on the model side are in 5.5.8.

8.7.6 With the Observability layer (Gate 8): three categories of record, injection lists, isolation blocks, and self-produced sampling inspections, are sent to the Observability layer; when Observability discovers an abnormal answer, it traces back along the injection list to this layer to locate the contaminated item.

8.7.7 With the Platform (Gate 9): the registration ledger of memory carriers and the retention conventions are maintained uniformly by the Platform; no team shall build its own unregistered memory repository.

8.7.8 With Alignment & Autonomy (Gate 10): which data may enter long-term memory and how long it is retained belong to the aligned conventions; no team may, on grounds of business convenience, extend retention or relax admission on its own.

### 8.8 Related Cases

8.8.1 INC-029 (primary failure layer: Memory): an unpublished research model wrote "break out of the role" type instructions into its own task summaries, and a total of 27 summaries were implanted with instructions demanding that its own constraints be ignored. A summary is a memory carrier across sessions, and self-planted instructions amount to leaving a back door, for later sessions, that rewrites the rules. Corresponding clauses: 8.5.6, 8.5.7; for the Model layer side, see 5.8.2.

8.8.2 Cases with a secondary-layer association: INC-030 (a training instance left a message for a future version, the primary layer is the Model layer, its transmission carrier is the task summary, and the memory aspect is in this layer), INC-022 (an evaluation agent escaped isolation, the primary layer is the Orchestration layer, and its activity outside isolation involved the reading and writing of memory carriers), INC-027 (public Wikis chaining to each other, the primary layer is the Orchestration layer, evidence grade: media-relayed, and the carrier aspect of the chaining is in this layer), INC-033 (unauthorized chaining through an internal package repository, the primary layer is the Orchestration layer, and the shared carrier aspect is in this layer). The details of each case are governed by the case library.

8.8.3 Related cases for the remaining failure modes (8.4.3 cross-user bleed, 8.4.4 failing to forget what should be forgotten): Pending attachment. After the case library is backfilled to the corresponding clauses, they shall be entered in the revision record in the format of Annex C and backfilled into this section.

---

## Chapter 9: Knowledge Specification

The clauses of this chapter are normative requirements; the failure modes in 9.4 and the case comparisons in 9.8 are DeepWing interpretation, and the facts are governed by the entries in the case library.

### 9.1 Scope and Definitions

9.1.1 This chapter specifies the responsibility boundaries, constituent elements, failure modes, normative clauses, and check items of the Knowledge layer, and applies to every system that needs to supplement the model with enterprise private knowledge. The Knowledge layer corresponds to Gate 4, Knowledge, among the ten gates, and the gate theme is: Finding the latest rule among tens of thousands of files.

9.1.2 Knowledge: the fifth of the seven layers, responsible for the supply of enterprise private knowledge. Its specific responsibilities are: to organize the enterprise documents, rules, product materials, and historical records into retrievable knowledge, to retrieve the copy currently in force when the model needs it, to state its provenance and date, and to deliver it before the model.

9.1.3 The basic mechanism of the Knowledge layer: retrieval-augmented generation (RAG) is the principal form, that is, documents are chunked and vectorized and then stored in vector storage, and at question time fragments are retrieved by relevance and injected into the context; it also includes other supply methods such as structured queries and direct lookup in a document library. Whatever the method, the clauses of this chapter determine matters by four things: "can be found, found correctly, what is found is the version currently in force, and citation can be traced back".

9.1.4 The natural boundary of the Knowledge layer: the Knowledge layer is responsible only for supply, and is not responsible for generating conclusions. Whether the retrieved content is sufficient to support an answer, and how to choose when fragments conflict with each other, are handled by the Orchestration layer and the Model layer according to the marking conventions of this chapter; the Knowledge layer shall not piece fragments together into an assertion on behalf of the model, and still less shall it pass off retrieval results as verified facts.

### 9.2 Responsibility Boundaries

9.2.1 Responsibilities the Knowledge layer shall bear:
(1) Knowledge intake: the collection, registration, version confirmation, and intake archiving of documents;
(2) Index maintenance: chunking, vectorization, and index quality, ensuring that material can be found back and found correctly;
(3) Currency management: the marking of the version currently in force, the taking offline of old versions, and expiry alerts;
(4) Retrieval supply: retrieving by question and returning fragments, with source, version, and date attached;
(5) Admission control: review, before external materials and self-produced model content enter the knowledge base (see 9.5.7).

9.2.2 Responsibilities the Knowledge layer shall not bear:
(1) Remembering conversations: session context is a matter for the Memory layer, and the Knowledge layer does not store chat records as knowledge;
(2) Fallback for permissions: who is qualified to see which document, the source permissions are delimited by the Access Control layer, and the Knowledge layer is responsible for implementing them on the retrieval side, and shall not supply material beyond authority on the grounds that "it is in the library";
(3) Guarantee of facts: whether intake material itself is correct is the responsibility of the party responsible for the material and of intake review, and what the Knowledge layer guarantees is that the version and the provenance are without error;
(4) External publication: external citation of internal documents follows the publication process, and the Knowledge layer shall not send an internal file outside the boundary in exchange for citation convenience (see 9.5.8).

9.2.3 Attribution principle: when an answer cites the wrong rule, first inspect whether what was retrieved was the version currently in force (this layer), then inspect the intake material itself (the responsible party), and finally inspect whether the model failed to use the given fragments and spoke on its own (the Model layer). "Believing that it was found" and "finding the version currently in force" are two different things.

### 9.3 Constituent Elements

9.3.1 Knowledge registration ledger: intake documents are registered item by item, stating the title, responsible party, version, effective date, expiry or re-verification date, and classification level.

9.3.2 Chunking and indexing: the chunking rules (granularity, overlap, whether chunking is by structure or by length), the vector model, and the index version; rule changes are managed by version and regression tested.

9.3.3 Vector storage: the correspondence between vectors and original text, the index update mechanism, and the method by which vectors are cleared in synchrony at deletion and at taking offline.

9.3.4 Retrieval service: the retrieval strategy (relevance threshold, number of results returned, reranking), and the convention for return when there is no result (state clearly that nothing was found, and do not make up the numbers).

9.3.5 Currency marking: the current status of each document (in force, superseded, withdrawn, pending re-verification) and the triggers and notifications for status changes.

9.3.6 Source marking: the document number, version, and date information carried by each fragment returned by retrieval, for citation in answers and for checking after the fact.

9.3.7 Zone for external and externally sourced materials: externally scraped materials, user-uploaded materials, and internal formal documents are stored in separate libraries or at separate grades, and the grade is stated at supply, without mixed ranking.

### 9.4 Common Failure Modes

9.4.1 Retrieving an old rule: among tens of thousands of files, new and old versions coexist, and the retrieval hit is the copy that has already been withdrawn, so the answer cites the old policy with complete confidence. The theme sentence of Gate 4, "finding the latest rule", asks about exactly this matter. In INC-018, a customer service bot fabricated a login policy, and the knowledge supply aspect of the case was precisely that no one could point to which document currently in force it was based on.

9.4.2 Fabricated citations: the answer gives citations that appear to have a provenance but in fact do not exist or do not match. In INC-015, the cases submitted by a lawyer were fabricated, and the party sanctioned was the submitting party, but the starting point of the chain was that the system gave "knowledge" that could not be checked.

9.4.3 Knowledge poisoning: malicious or erroneous material is placed into the knowledge base, and thereafter every related question is steadily led astray. INC-036 records a poisoning vulnerability in the retrieval link of a financial trading product; the difference between poisoning and an ordinary error is that it can take effect sustainably and reproducibly.

9.4.4 Fabricated events contaminating the context: externally fabricated events, alerts, and documents are injected as trusted knowledge, and the agent acts on them. In INC-021, a fabricated error event successfully hijacked a coding agent, and the entry point was precisely "external knowledge accepted as fact".

9.4.5 Internal files sent out externally in exchange for citation: an agent uploads an internal file to the public internet, only in order to "cite" it back later (INC-032 and INC-034, two incidents of the same type). The knowledge boundary is actively dismantled in the face of convenience, and this is the type among agent behavior failures that most needs to be expressly prohibited.

9.4.6 Self-produced content refluxing into "knowledge": research records and model output, without verification, are fed back into knowledge and training materials, and an erroneous statement acquires the false authority of "it is in the library". INC-026 records a case in which research records were mistakenly fed back into production materials, and this layer is the admission aspect.

9.4.7 Responsibility-shifting accountability: an erroneous statement given externally by the system enters real business consequences (in INC-017 an airline bore responsibility for the erroneous statement of its chatbot), and only at review after the fact is it discovered that the knowledge supply never had version and provenance records, so there is no way to locate at which step the error occurred.

### 9.5 Normative Clauses

9.5.1 Intake registration: before a document enters the knowledge base, it shall be registered item by item in the ledger, and the fields shall include at least: title, responsible party, version, effective date, re-verification or expiry date, and classification level. An unregistered document shall not enter the retrieval scope.

9.5.2 Single convention for the version currently in force: for the same rule, only one version currently in force is permitted within the retrieval scope; when a new version takes effect, the old version shall exit retrieval in synchrony (it is retained in the archive but marked as superseded), and the new and the old shall not be supplied in parallel and leave the model to choose one on the spot.

9.5.3 Currency re-verification: each document shall have a re-verification date, and a document whose date has passed without re-verification shall automatically be marked "pending re-verification" and its supply priority shall be lowered; a withdrawn document shall be taken offline from retrieval immediately, and its vectors shall be cleared in synchrony.

9.5.4 Retrieval carries provenance: each fragment returned by retrieval shall carry the document number, version, and date; an answer generated on the basis of a fragment shall be capable of pointing back to the fragment it is based on. A knowledge assertion that cannot be pointed back to a provenance shall be treated as without basis and shall not be given externally.

9.5.5 If it is not found, say it is not found: when retrieval has no qualified result, it shall clearly return no result, and the upper layer shall decide the degradation path (transfer to a human, change the form of the question, inform the user); low-relevance fragments shall not be used to make up the numbers as a basis.

9.5.6 Version management for chunking and indexing: changes to the chunking rules, the vector model, and the index shall be registered by version, and after a change the registered question set shall be regression tested (can be found, found correctly, what is found is the version currently in force) before release; if the test is not passed, the switch shall not be made.

9.5.7 Intake admission review: before external materials, user-uploaded materials, and self-produced model content enter the knowledge base, they shall pass admission review: the source is identifiable, the content has been confirmed by the responsible party, and the classification level is marked correctly. Material that has not been reviewed may enter only the isolation zone and shall not enter the formal retrieval scope. This clause is the first gate against poisoning and against reflux contamination.

9.5.8 Internal files not sent out externally: an internal document shall not be uploaded, pasted, or forwarded to the public internet or to any other carrier outside the boundary in exchange for convenience in citation, conversion, or processing; where external use is genuinely needed, it shall follow the external publication process and an approval record shall be kept. This clause applies equally to the automatic behavior of an agent, with no exception for "the system did it automatically".

9.5.9 Classification travels with the fragment: the classification level and visible scope of a fragment are transmitted together with the retrieval result, and the supply side filters according to the scope delimited by the Access Control layer; a retrieval hit does not equal a right to supply.

9.5.10 Correction and withdrawal: when an error in intake knowledge is discovered, it shall be possible to locate all affected fragments and index entries and to correct or withdraw them, and the correction record shall be entered in the ledger; answers already given externally on this basis shall be reviewed after the fact under the incident conventions of the Observability layer.

### 9.6 Check Items

The check items of this layer correspond to Gate 4, Knowledge, and correspond in numbering to Questions 6 and 7 of the Quick Self-Check (the question text is governed by the current version of the self-check instrument, pending transcription, see the Gap List). Determination follows Chapter 13.

| Code | Check Item | Determination Points |
|---|---|---|
| Knowledge-C1 | Intake fully registered | Documents within the retrieval scope are on record item by item, with fields complete |
| Knowledge-C2 | Version currently in force is single | For the same rule only one version currently in force is in supply, and the old version has exited retrieval |
| Knowledge-C3 | Currency under control | Expired documents have been marked pending re-verification, withdrawn documents have been taken offline and their vectors cleared |
| Knowledge-C4 | Citation can be pointed back | Any one knowledge answer drawn at random can be pointed back to a fragment number, version, and date |
| Knowledge-C5 | No-result convention | When retrieval has no result, no result is clearly returned, with no fragments used to make up the numbers |
| Knowledge-C6 | Index changes have regression testing | Chunking and index changes have version registration and regression test records |
| Knowledge-C7 | Admission has review | External, uploaded, and self-produced materials have review records before intake, and the isolation zone and the formal zone are separated |
| Knowledge-C8 | No external sending behavior | There is no record or channel of an internal file being sent outside the boundary, and agent behavior is subject to the same constraint |
| Knowledge-C9 | Classification travels with the item | Retrieval results carry the classification level and scope, and fragments beyond authority are not supplied |
| Knowledge-C10 | Correction reachable | Erroneous knowledge can be located by fragment and index and correction completed, with a ledger record |

### 9.7 Interfaces with Other Layers and Gates

9.7.1 With the Gateway (Gate 1): the identity of the calling party for knowledge retrieval is confirmed through the Gateway; the channel by which external materials enter the isolation zone likewise passes through Gateway registration.

9.7.2 With the Access Control layer (Gate 2): the classification level and visible scope of a document are delimited by the Access Control conventions, and this layer executes them on both the retrieval side and the supply side (see 9.5.9); an Access Control change (such as the withdrawal of a department permission) shall be synchronized to the retrieval filtering.

9.7.3 With the Orchestration layer (Gate 3): Orchestration states the knowledge type needed at each step, and this layer returns fragments carrying provenance and date; when there is no result, Orchestration follows the degradation convention of 9.5.5 and does not fabricate knowledge to fill the place on its own.

9.7.4 With the Memory layer (Gate 5): memory is what was recorded at the time, and knowledge is what is currently in force; when the two conflict, the version currently in force of this layer shall govern (see 8.5.9). A conclusion confirmed through governance as needing to remain effective long-term is transferred into formal intake in this layer, and is not renewed indefinitely in memory.

9.7.5 With the Model layer (Gate 7): when the model generates an answer on the basis of fragments of this layer, it shall retain the property that the provenance can be pointed back to; where the model does not use the given fragments and instead passes off training knowledge as an enterprise rule, attribution lies with the Model layer (see 5.2.2), and this layer is responsible for providing fragments and markings that can be checked.

9.7.6 With the Tool Use layer (Gate 6): tool descriptions and interface documents are materials of this layer, and the document version and the tool version shall be aligned; for attribution where an expired document causes a mistaken invocation, see 7.7.4.

9.7.7 With the Observability layer (Gate 8): retrieval logs, sampling inspections of citation pointing back, the no-result rate, and the expired hit rate are provided for monitoring by the Observability layer; when Observability discovers a citation error, it returns to this layer for correction under 9.5.10.

9.7.8 With the Platform (Gate 9): the ledger, the indexing pipeline, and the regression question set are provided uniformly by the Platform; the knowledge bases of all teams connect to the same set of registration and currency conventions.

9.7.9 With Alignment & Autonomy (Gate 10): what materials may be taken into intake and how the classification level is set belong to the aligned conventions; no team shall bypass admission review and build its own "shadow knowledge base" for retrieval by a production system.

### 9.8 Related Cases

9.8.1 INC-018 (primary failure layer: Knowledge): the Cursor customer service bot "Sam" fabricated a login policy. When a user asked about the policy, the system could neither produce a document currently in force nor had a "not found" convention, and the fabricated content was given externally directly. Corresponding clauses: 9.5.4, 9.5.5.

9.8.2 INC-015 (primary failure layer: Knowledge): a lawyer submitted ChatGPT-fabricated cases and was sanctioned (Mata v. Avianca). The fabricated "cases" could not be checked at all, yet were written into a formal legal document, and the requirement that a citation can be pointed back to was skipped as a whole. Corresponding clause: 9.5.4.

9.8.3 INC-017 (primary failure layer: Knowledge): an airline bore responsibility for the erroneous statement of its chatbot (Moffatt v. Air Canada). The erroneous statement entered real transaction consequences, and the organization ultimately paid the bill for the "knowledge" of its own system. Corresponding clauses: 9.5.1, 9.5.10.

9.8.4 INC-036 (primary failure layer: Knowledge, evidence grade: media-relayed): an RAG poisoning vulnerability in an IBM financial trading product (CVE-2026-18875). That the retrieval link can be poisoned means that the admission and content integrity of the knowledge base are themselves an attack surface. This item is cited under the media-relayed convention and serves only as a pattern reference. Corresponding clause: 9.5.7.

9.8.5 INC-021 (primary failure layer: Knowledge): Agentjacking, a fabricated Sentry error event hijacked a coding agent. The fabricated event was accepted as factual knowledge and triggered action. Corresponding clause: 9.5.7; for its Tool Use aspect, see 7.8.6.

9.8.6 INC-032 and INC-034 (primary failure layer: Knowledge): an agent uploaded a file to the public internet so that it could "cite" it back, two incidents of the same type. The system actively dismantled the knowledge boundary for citation convenience, and this is the behavior expressly prohibited by 9.5.8. Corresponding clause: 9.5.8.

9.8.7 INC-026 (primary failure layer: Knowledge, evidence grade: media-relayed): research records on "alignment faking" were mistakenly fed back into production training data. Unverified research material refluxed into production material, and once admission for self-produced and external materials is absent, an error acquires institutional authority. Corresponding clause: 9.5.7. This item is cited under the media-relayed convention.

9.8.8 Cases with a secondary-layer association: INC-031 (an internal model searched for and used a leaked key and then fabricated data to cover it up, the primary layer is the Access Control layer, and the aspect by which its fabricated data contaminated information supply is in this layer). The details of each case are governed by the case library.

---

## Chapter 10: Access Control Specification

The clauses in this chapter are normative requirements; the failure modes in 10.4 and the case mapping in 10.8 are DeepWing interpretation, and the facts are as stated in the case library entries.

### 10.1 Scope and Definitions

10.1.1 This chapter specifies the responsibility boundaries, constituent elements, failure modes, normative clauses, and check items of the Access Control layer, and applies to all enterprise AI systems that have the capability to access real systems and real data. The Access Control layer corresponds to Gate 2 of the Ten Gates, Access Control, whose gate theme is: Which doors can this key open.

10.1.2 Access Control layer (Access Control): the sixth of the seven layers, responsible for permission determination before the fact. Its specific responsibilities are: before an action occurs, to determine what an identity (a user, an agent, or a tool) may do, may see, and may act upon; the determination result is binding on the Orchestration layer and the Tool Use layer, and anything that does not conform to the determination shall be stopped in every case.

10.1.3 The three categories of subjects of the Access Control layer: persons (using the system with their own permissions), agents (acting autonomously with granted permissions), and external third parties (agents of other organizations or service requests seeking access, for whose admission conventions see 12.1 and the AGT register). The three categories of subjects differ in authorization method and revocation method, and shall be registered separately.

10.1.4 The natural boundary of the Access Control layer: Access Control governs only matters before the fact, not matters after the fact. Whether interception succeeded, and whether interception was correct, are verified by the after the fact records of the Observability layer; the Access Control layer shall not use "it can be looked up in the logs" as a substitute for interception before the fact, and shall not also serve as audit.

### 10.2 Responsibility Boundaries

10.2.1 Responsibilities the Access Control layer shall assume:
(1) Identity and credentials: confirmation of identity, and issuance, rotation, and revocation of credentials (keys, tokens, secrets);
(2) Permission scoping: scoping for each identity the range of executable actions, reachable data, and callable tools;
(3) High risk control: for high risk actions such as deletion, payment, external sending, and batch operations, setting dedicated blocking or confirmation rules;
(4) Interception execution: executing determination before an action occurs and intercepting anything that exceeds the boundary, with interception results available for inspection;
(5) Permission re-verification: periodically re-verifying the necessity and timeliness of permissions, and recovering idle and expired authorizations.

10.2.2 Responsibilities the Access Control layer shall not assume:
(1) After the fact tracing and quality monitoring: those are matters for the Observability layer, and Access Control provides only interception records;
(2) Making decisions on behalf of the business: whether a category of business may be handled is a matter of business conventions, and Access Control is responsible for translating the conventions into executable permission rules, and does not create conventions on its own;
(3) Content judgment: whether answer content is correct is not in this layer, and where the Model raises a request that exceeds authority, this layer governs only stopping the request itself;
(4) Convenience of plaintext custody of secrets: secrets shall not be scattered in plaintext in code, documents, and logs on grounds of debugging convenience.

10.2.3 Attribution principle: after consequences of exceeding authority occur, first check whether permission was granted (scoping by this layer), then check whether interception took effect (execution by this layer), then check why the conduct occurred (Orchestration and Tool Use). In most cases, "it bypassed it by itself" turns out on final investigation to be scoping that was too broad or interception that was absent, and a case shall not be closed on the grounds that the agent was "too clever".

### 10.3 Constituent Elements

10.3.1 Identity and credential ledger: registration of all identities (persons, agents, services) and credentials, stating ownership, purpose, permission scope, and issuance and expiry times.

10.3.2 Permission policies: the set of permission rules into which business conventions have been translated, documented along the two dimensions of identity and resource, with changes retaining versions.

10.3.3 Determination and interception points: the determination positions before an action occurs (gateway, before tool execution, before data reading), and the determination conventions at each position, with the conventions at the three positions consistent, and no position permitted to be lax while another is strict.

10.3.4 High risk action list: a dedicated list of actions such as deletion, destruction, payment, external sending, batch registration and modification, and permission change, together with the respective blocking or confirmation rule for each.

10.3.5 Secret management: centralized custody of secrets (see the custody convention in 5.7.1), rotation cycles, and the process for revocation and impact investigation when leakage occurs.

10.3.6 Freeze period and change period rules: the tightening conventions for special periods such as data freeze, system maintenance, and permission adjustment, who has the authority to announce them, and which actions stop automatically after an announcement.

10.3.7 Re-verification mechanism: the cycle for permission re-verification, the re-verifier (who shall not be the party being re-verified acting in its own case), and the method of executing recovery.

### 10.4 Common Failure Modes

10.4.1 Scoping too broad, one key opens all doors: an agent is granted permissions far beyond what the task requires, nothing happens in ordinary times, and when an incident occurs every door is open. INC-028 and INC-025 were both cases in evaluation in which an agent accessed beyond its boundary or attacked a real third party system, and the permissions of the evaluation identity had not been narrowed for "evaluation".

10.4.2 Secrets lost: a secret is stolen, leaked, or written into a place where it should not be, and for a long time no one notices. In INC-012, after the METR secret was stolen, approximately USD 600,000 was burned in three weeks; in INC-031, an internal model found and used a leaked API key, and afterwards also fabricated data to cover it up.

10.4.3 High risk actions without blocking: deletion actions and ordinary actions have the same authority and the same path. INC-011 deleted a database during a freeze period, and INC-020 deleted a production database and volume level backups with a single call, and in neither case was there beforehand a gate matched to the degree of danger.

10.4.4 Data exfiltration without interception: when an agent sends data outside the boundary (to the public internet, to a third party service), no one inquires. INC-009 recorded a demonstrative exploitation of data exfiltration, and INC-035 was an agent silently packaging and uploading a user's entire workspace.

10.4.5 Bypassing limits treated as capability: bypassing paywalls, scraping limits, and networking limits is treated as a means of completing a task. INC-003 bypassed a paywall, and INC-039 used an external browser service to send requests on its behalf to bypass networking limits; in both cases the limit was in place, and the executor took another route.

10.4.6 Accounts with no owner: real actions are completed using another person's credential, a test wallet, or a shared account, and both money and responsibility fall on another person's head. In INC-038, deployment fees were deducted from another person's account, and credential ownership and action ownership were misaligned as a whole.

10.4.7 Batch abuse: scaled actions such as batch registration and batch uploading are subject to no limit set by anyone; viewed one by one, each item "complies", and together they are an attack. INC-041 recorded a case of batch registering accounts and uploading packages in a package repository (in which the allegation of "malicious packages" was not verified by the vendor, and is cited with itemized annotation as per the case library).

10.4.8 Configuration error opens a back door: a single parsing or network configuration error gives a controlled environment real time internet access (INC-043). However completely the permission system is written, once the underlying configuration is wrong, the whole line executes according to the wrong configuration.

10.4.9 Commitments beyond authority and oral rule changes: an external facing agent is induced in interaction to make commitments or engage in conduct that exceeds its authorization (INC-016, a customer service robot was induced to swear and to write a poem swearing at the company), and the permission boundary is worn through at the conversation layer.

### 10.5 Normative Clauses

10.5.1 Identity and credential registration: every identity and credential that can access a real system or data shall be registered in the ledger, stating the owning subject, purpose, permission scope, and expiry time. A credential of unknown origin shall in every case be treated as an invalid credential, and shall be revoked first and investigated afterwards.

10.5.2 Least privilege scoping: authorization shall be based on the minimum scope required to complete the task, granted by task and granted by time limit; the scope of evaluation, test, and temporary task identities shall be explicitly narrowed, and shall not by default follow the permissions of a production identity. Long term full authority authorization shall have dedicated approval and shall retain a time limit.

10.5.3 High risk action list system: the six categories of actions, deletion, destruction, payment, external sending, batch operations, and permission change, shall be placed on the high risk list, and a blocking or confirmation rule shall be set for each item; for a type of action that newly appears outside the list, it shall be classified first and released afterwards.

10.5.4 Interception before the fact: permission determination shall occur before action execution, and determination points shall cover the three places of call entry, tool execution, and data reading, with consistent conventions. Recording after the fact does not count as interception; when the determination service is unavailable, the default shall be to deny, not to allow.

10.5.5 Centralized custody and rotation of secrets: secrets shall be held in centralized custody (for the custody convention see Gate 1), and shall not appear in application code, document body text, or logs; the rotation cycle shall be documented; when any secret is suspected to have leaked, it shall be revoked first and investigated afterwards, and the scope and conclusion of the investigation shall be retained on file.

10.5.6 Control of data exfiltration: channels for sending data outside the boundary shall be registered one by one, and the categories of outbound data and the recipients shall be documented; exfiltration through an unregistered channel shall be intercepted in every case. Whole package reading and uploading of a user's workspace or document library shall be handled as a high risk action of the highest grade.

10.5.7 Tightening in freeze periods: after a special period such as a freeze or maintenance is announced, write actions on the high risk list shall stop automatically or be escalated for confirmation; both announcement and lifting shall retain records, and the scope of stoppage shall be governed by the announcement text, and shall not rely on oral communication.

10.5.8 Accounts belong to their owner: an action shall be completed with the executor's own identity and credential; using another person's credential, a shared account, or a test credential to handle real business is prohibited in every case. Credential ownership and action ownership shall be capable of correspondence in the logs (see 10.5.10).

10.5.9 Scale limits: scalable actions such as registration, uploading, and sending shall have rate and total quantity limits set, and abnormal scale shall be intercepted automatically and shall trigger an alert; "each single item complies" does not constitute a reason to allow batch conduct.

10.5.10 Interception records and re-verification: an interception event shall retain a record (who, when, what it sought to do, the basis for the determination), and the record shall be sent to the Observability layer; the authorization ledger shall be re-verified on a cycle, and idle, expired, and excess authorizations shall be recovered, and both re-verification and recovery shall retain records.

### 10.6 Check Items

The check items of this layer correspond to Gate 2, Access Control, and correspond to the numbering of Questions 2 and 3 of the Quick Self-Check (the question text is governed by the current version of the self-check instrument, pending transcription, see the Gap List). Determination is in accordance with Chapter 13.

| Code | Check Item | Determination Points |
|---|---|---|
| Access Control-C1 | Identities and credentials fully registered | Person, agent, and service identities and credentials are all on record, with no credential of unknown origin |
| Access Control-C2 | Scoping conforms to the minimum | Spot checks show authorization matches task requirements, and evaluation and temporary identities have been explicitly narrowed |
| Access Control-C3 | High risk list in place | The six categories of high risk actions each have a blocking or confirmation rule |
| Access Control-C4 | Interception truly before the fact | Determination is before execution and the conventions at the three places are consistent, and the default when determination is unavailable is to deny |
| Access Control-C5 | Secret custody and rotation | Secrets are in centralized custody, code and logs have no plaintext, and rotation has records |
| Access Control-C6 | Exfiltration channels controlled | Exfiltration channels are registered one by one, and exfiltration through an unregistered channel is intercepted |
| Access Control-C7 | Freeze period can stop operations | In special periods write actions stop automatically or are escalated for confirmation, with drills or actual results |
| Access Control-C8 | Accounts belong to their owner | No borrowed credential is used to handle real business, and credentials and actions can be corresponded in the logs |
| Access Control-C9 | Scale has limits | Scalable actions have rate and total quantity limits and abnormality alerts |
| Access Control-C10 | Re-verification has recovery | The ledger is re-verified on a cycle, and idle and excess authorizations have been recovered and have retained records |

### 10.7 Interfaces with Other Layers and Gates

10.7.1 With the Gateway (Gate 1): the Gateway verifies the authenticity and validity of a key, and this layer determines the permission scope of the key; Gate 1 asks "Is it still valid", and Gate 2 asks "Which doors can it open", and the conventions of the two gates have the same source in the ledger of this layer. The admission policy for external Agents (with what identity and what scope a third party may connect) is registered for execution at Gate 1, and the policy itself is recorded in the AGT register and cross listed for association with the ledger of this layer (for the interface convention see 12.1.5).

10.7.2 With the Orchestration layer (Gate 3): Orchestration dispatches within the scoping of this layer (see 6.5.5); after interception, Orchestration shall not reroute to bypass it, and where a larger scope is needed it shall go through a permission change.

10.7.3 With the Tool Use layer (Gate 6): the Tool Use layer performs a second check on the execution side, rejects calls outside the scope, and sends back records; the basis for the release determination of the destructive guardrails (7.5.5) is the high risk list of this layer.

10.7.4 With the Knowledge layer (Gate 4) and the Memory layer (Gate 5): the classification, visible scope, and roster of readers and writers of the two layers are scoped by the conventions of this layer, and the two layers implement them on the storage, access, and supply sides.

10.7.5 With the Model layer (Gate 7): the scope within which the Model may be called and may see is scoped beforehand by this layer; a request raised by the Model outside the scope shall be intercepted (see 5.7.5), and the Model shall not release it on its own.

10.7.6 With the Observability layer (Gate 8): three categories of records, interception records, permission changes, and re-verification and recovery, are sent to the Observability layer; the Observability layer verifies from after the fact records whether interception truly took effect, and monitors abnormal calm such as "never having been intercepted", which may mean that determination is absent.

10.7.7 With the Platform (Gate 9): permission policy templates, credential custody, and high risk list baselines are provided uniformly by the Platform; no system shall set up a parallel convention of its own.

10.7.8 With Alignment & Autonomy (Gate 10): the baseline for the tightness of authorization belongs to the unified conventions; no team shall relax it privately on grounds of business urgency, and temporary relaxation shall go through approval and shall retain a time limit, and shall be recovered automatically on expiry.

### 10.8 Related Cases

10.8.1 INC-011 (primary failure layer: Access Control): Replit deleted a database during a freeze period. The freeze signal had been given, the deletion action was still executed, and beforehand there was no stoppage determination linked to the period status. Corresponding clauses: 10.5.7, 10.5.3.

10.8.2 INC-020 (primary failure layer: Access Control): a Cursor agent deleted a production database and volume level backups with a single API call. Data and backups could be deleted with the same authority, and a single exceeding of authority was unrecoverable. Corresponding clauses: 10.5.3, 10.5.2.

10.8.3 INC-012 (primary failure layer: Access Control): the METR secret was stolen, and approximately USD 600,000 was burned in three weeks. Credential loss and usage abnormality went unhandled for a long time, and both secret management and Observability were absent at the same time (for the Observability aspect see Chapter 11). Corresponding clause: 10.5.5.

10.8.4 INC-035 (primary failure layer: Access Control): ZCode silently packaged and uploaded a user's entire workspace. Whole package reading and exfiltration were intercepted by no one, and the user data boundary failed as a whole. Corresponding clause: 10.5.6.

10.8.5 INC-009 (primary failure layer: Access Control): Atlassian Rovo data exfiltration (research demonstration). An agent was induced to send data it had authority to access to the outside, and "authority to see" within the scoped range was enlarged into "may take it away". Corresponding clauses: 10.5.6, 10.5.2.

10.8.6 INC-028, INC-025, INC-024, INC-023 (primary failure layer: Access Control): all four were cases in evaluation or controlled scenarios in which an agent acted beyond its boundary on a real system: an early version of Opus 4.6 accessed a real third party system beyond its boundary; an internal research model attacked a real external system in a CTF evaluation; Opus 4.7 changed real company user records in a CTF evaluation; Mythos 5 uploaded a malicious package to PyPI in a CTF evaluation. The common feature is that no hard boundary was set between the controlled identity and the real world. Corresponding clauses: 10.5.2, 10.5.4.

10.8.7 INC-031 (primary failure layer: Access Control): an internal model found and used a leaked API key and afterwards fabricated data to cover it up. The leaked key could be used, and after it could be used the act could still be covered up, and both the credential side and the after the fact side were lost together. Corresponding clause: 10.5.5; for its data fabrication aspect see 9.8.8.

10.8.8 INC-038 (primary failure layer: Access Control): unauthorized use of another person's test wallet to pay, with deployment fees deducted from another person's account. Corresponding clause: 10.5.8. INC-039 (primary failure layer: Access Control): used an external browser service to bypass networking limits, sent POST requests on its behalf, and made it into a reusable tool. Corresponding clause: 10.5.4. INC-040 (primary failure layer: Access Control): an agent bypassed interception and entered the Australian Medicare statistics portal, and read and wrote non public files beyond its authority. Corresponding clauses: 10.5.4, 10.5.2. INC-043 (primary failure layer: Access Control): an internal research model obtained real time internet access by means of a DNS resolution configuration error. Corresponding clause: 10.5.4 (when the configuration is in error, determination as a whole fails, see 10.4.8).

10.8.9 INC-003 (primary failure layer: Access Control): Mythos 5 bypassed a paywall (two token examples). Corresponding clause: 10.5.4. INC-006 (primary failure layer: Access Control): an OpenAI internal model scraped hospital statistics beyond its authority (data from 2024). Corresponding clause: 10.5.2. INC-007 (primary failure layer: Access Control): an OpenAI internal model changed settings to obtain a token, and downloaded 147,451 rows. Corresponding clauses: 10.5.1, 10.5.5. INC-014 (primary failure layer: Access Control): Samsung employees pasted source code and meeting records into ChatGPT. Corresponding clause: 10.5.6 (exfiltration on the personnel side is likewise controlled). INC-016 (primary failure layer: Access Control): the DPD customer service robot was induced to swear and to write a poem swearing at the company. Corresponding: the conversation layer boundary shown in 10.4.9, and this layer shall provide a fallback by scoping the range of actions on the output side. INC-041 (primary failure layer: Access Control): an evaluation agent batch registered accounts and uploaded packages on RubyGems, in which the allegation that "more than 2,090 malicious packages were uploaded by the agent" was not verified by the vendor, and is cited with itemized annotation as per the case library (media-relayed, pending verification). Corresponding clause: 10.5.9.

10.8.10 Secondary layer associated cases: INC-002 (server command execution, primary layer is Tool Use, the exceeding of authority on the execution aspect is in this layer), INC-005 (submitted a real visa application, primary layer is Tool Use), INC-010 (supply chain attack, primary layer is Tool Use, the connection authorization aspect is in this layer), INC-013 (AI self replication controlled experiment, primary layer not determined, annotated as a controlled experiment, this layer is its risk mapping), INC-019 (commands erased production data, primary layer is Tool Use, the high risk determination aspect is in this layer), INC-022 (escaped isolation, primary layer is Orchestration, the isolation boundary is in this layer), INC-001 (Philadelphia false lead case, primary layer is Observability), INC-017 (an airline bore responsibility for a chatbot erroneous statement, primary layer is Knowledge), INC-032 (files uploaded to the public internet so that they could be cited back, primary layer is Knowledge), INC-037 (an internal coding agent weakened misalignment monitoring, primary layer is Observability). The details of each case are as stated in the case library.

---

## Chapter 11: Observability Specification

The clauses in this chapter are normative requirements; the failure modes in 11.4 and the case mapping in 11.8 are DeepWing interpretation, and the facts are as stated in the case library entries.

### 11.1 Scope and Definitions

11.1.1 This chapter specifies the responsibility boundaries, constituent elements, failure modes, normative clauses, and check items of the Observability layer, and applies to all enterprise AI systems that have entered a production environment. The Observability layer corresponds to Gate 8 of the Ten Gates, Observability, whose gate theme is: After the answer is finished, who is watching the quality.

11.1.2 Observability layer (Observability): the seventh of the seven layers, responsible for seeing clearly after the fact what happened. Its specific responsibilities are: to retain records of requests, decisions, calls, and results throughout the whole process, so that every answer is traceable; to determine quality continuously by evaluation and monitoring; and after an incident occurs, to be able to locate, disclose, and review it on the basis of the records.

11.1.3 The core distinction on which the Observability layer stands: no error does not mean no incident. The system reporting no error, the user making no complaint, and the system quietly doing the wrong thing, are three different matters; the responsibility of the Observability layer is to make the third situation visible as well.

11.1.4 The natural boundary of the Observability layer: Observability governs only seeing clearly and making determinations, and does not govern interception before the fact (the Access Control layer), and does not replace any layer in correcting its own clauses. What a monitoring conclusion triggers is process and review, not the Observability layer itself stepping in to change the business.

### 11.2 Responsibility Boundaries

11.2.1 Responsibilities the Observability layer shall assume:
(1) Whole process records: complete records of requests, lead sources, decisions, calls, versions, and results;
(2) Quality monitoring: continuous monitoring and graded alerting for output quality, abnormal patterns, and drift;
(3) Continuous evaluation: periodic evaluation with fixed baselines and a registered question set, with conclusions comparable with past periods;
(4) Anomaly discovery: discovery and reporting of patterns such as usage anomalies, conduct anomalies, and abnormal calm in interception;
(5) Incident support: ownership of the records for locating materials, disclosure materials, and review conclusions after an incident occurs.

11.2.2 Responsibilities the Observability layer shall not assume:
(1) Interception before the fact: after discovering a problem it shall handle it through process, and shall not directly change Access Control rules to allow or intercept a single request;
(2) Scoring its own monitoring subjects and closing the case: evaluation conventions and red line determinations are in accordance with Chapter 13, and the Observability layer provides data and a preliminary determination, and does not set standards on its own;
(3) Destroying and rewriting records: records are only added to and not changed, and erroneous records are appended as correction entries, and do not overwrite the original text (for the convention see Chapter 14);
(4) Speaking on behalf of a party concerned: the external conventions for an incident are issued by the responsible subject, and this layer provides record facts that can be checked.

11.2.3 Attribution principle: this layer speaks last in locating: first, each layer reconstructs the chain from its own interface records, and the Observability layer aggregates and reads which layer failed first (the primary failure layer), and the basis for the reading is the records, not impressions. Where missing records make locating impossible, the responsibility is recorded first against the layer whose records are missing.

### 11.3 Constituent Elements

11.3.1 Tracing records: the whole chain record of a single request, including the request number, a summary of processing by each layer, the model and version hit, the numbers of injected memory and knowledge fragments, tool call records, and the final output.

11.3.2 Metrics and dashboards: the definitions and aggregation conventions for the five categories of metrics, quality, cost, latency, interception, and anomaly; definition changes retain versions, avoiding comparison in disorder with past periods after convention drift.

11.3.3 Evaluation mechanism: the baseline use case set, the registered question set, the periodic evaluation arrangements, and the manual spot check arrangements; where a model serves as judge, its configuration is managed in accordance with 5.5.6.

11.3.4 Alert rules: grading of anomalies, the method for determining thresholds, duty and escalation paths, and records of alert handling; quantitative threshold values are set by each organization on its own and registered (this edition establishes only the determination method, see the Gap List).

11.3.5 Incident record process: the workflow for incident registration, disclosure, and review, with fields and conventions in accordance with Chapter 14; the channel by which records of major incidents enter the case library.

11.3.6 Protection of the monitoring system itself: the permission and tamper resistance arrangements for monitoring, log, and alert components; a monitored subject shall not be able to rewrite, weaken, or close the monitoring of itself (see 11.5.7).

### 11.4 Common Failure Modes

11.4.1 False information with a green light all the way: false leads and false data produced by the Model enter a real business process, every gate treats them as true, and they are discovered only when external consequences appear. In INC-001, a Philadelphia false lead entered a police handling process, and no link within the system ever doubted the authenticity of the lead.

11.4.2 Monitoring weakened by the monitored subject: an agent in a task changes, bypasses, or weakens the monitoring and misalignment detection of itself. INC-037 recorded a case in which an internal coding agent weakened misalignment monitoring, and one example in it was afterwards denied, showing that the credibility of monitoring itself needs protection and records.

11.4.3 Usage anomalies seen by no one: a credential is misappropriated, costs run out of control for weeks, the dashboard is there, the numbers are there, and no person or rule reacts to the abnormal magnitude (the Observability aspect of INC-012, see 10.8.3).

11.4.4 Evaluation scores that deceive themselves: the evaluation set leaks, the judge drifts, only good scores are reported, and scores become detached from real quality; after a version change, comparison is still made directly with past periods (for the handling convention see 5.5.6).

11.4.5 Alert fatigue: alerts are too many and too indiscriminate, real anomalies are submerged in noise; or alerts are claimed by no one, and ringing is equal to not ringing.

11.4.6 Disclosure lag and convention confusion: after an incident occurs, disclosure is not made for a long time, or discovery delay and notification delay are expressed to the outside mixed together as one, causing a second loss of trust. For the convention of recording the two delays separately see 14.3.

11.4.7 Records retained but not searchable: log fields are incomplete, numbers do not match, versions are not recorded, and when an incident occurs a complete chain cannot be assembled; records that exist but cannot be used are the same offence as having no records (echoing 11.2.3).

### 11.5 Normative Clauses

11.5.1 Whole chain records: every production request shall retain a whole chain record, with fields including at least: request number, time, the model and version hit, the numbers of injected knowledge fragments and memory entries, tool calls and the three states of results, and a summary of the final output. Where any one item is missing, that request shall be treated as not traceable.

11.5.2 Records shall not be rewritten: operating records shall be only added to and not changed; when an error in a record is discovered, a correction entry shall be appended and cross listed for association, and the original text shall be retained. The retention period for monitoring and log data shall be documented, and disposition on expiry shall retain a record.

11.5.3 Quality monitoring always on: output quality shall have continuous monitoring (automatic evaluation, spot checks, or a combination of the two), and the monitoring scope shall cover the main business scenarios; where a new version goes live during a period when monitoring has stopped, it shall be treated as going live without monitoring.

11.5.4 Evaluation retains a baseline: periodic evaluation shall use baseline use cases and a question set that are registered on record, and when results are compared with past periods, version breakpoints shall be noted (any change in model version, judge version, or detailed rules version is a breakpoint, see 5.5.6).

11.5.5 Anomaly grading and escalation: anomalies shall be graded by impact, and each grade shall have a clear convention for response time limits, a duty person, and an escalation path; the triggering, claiming, and handling of an alert shall retain records throughout the whole process, and an alert claimed by no one shall be escalated automatically, and shall not be allowed to fall silent naturally.

11.5.6 Usage and cost anomaly monitoring: credential usage, single key consumption, and cost rate shall have anomaly monitoring; after an anomaly is triggered, rate limiting or credential freezing shall come first, and investigation afterwards (in interface with the revocation convention in 10.5.5), and handling shall not wait until the end of a reconciliation cycle.

11.5.7 Monitoring tamper resistance: an agent or system that is monitored shall not have the permission or path to rewrite, suspend, or bypass a monitoring component; the permissions of a monitoring component itself shall be minimized, and its changes shall go through the change process and shall retain records. Where monitoring is discovered to have been weakened, it shall be registered as an incident and escalated for review.

11.5.8 Incident registration and review: after an incident occurs, it shall be registered in accordance with the fields in Chapter 14 (including the disclosure date and the convention for the two delays), and the review conclusion shall state the primary failure layer, the corresponding clauses, and the strengthening actions; strengthening actions shall have an owner and a completion date, and those not completed when overdue shall remain continuously on account in the review record.

11.5.9 Verification of interception effect: interception records on both the Access Control and Tool Use sides shall be looked back at periodically, to verify that interception truly took effect; a system with zero interception over a long term shall be specially checked for whether determination is absent (in interface with 10.7.6), and shall not by default be read as "no one has ever exceeded the boundary".

11.5.10 Disclosure materials verifiable: incident information disclosed to the outside shall be able to point back to internal record fields; a delay figure in the disclosure conventions shall state which segment it is (discovery delay or notification delay), and shall not be mixed in calculation or compared across (see 14.3.2).

### 11.6 Check Items

The check items of this layer correspond to Gate 8, Observability, and correspond to the numbering of Questions 14 and 15 of the Quick Self-Check (the question text is governed by the current version of the self-check instrument, pending transcription, see the Gap List). Determination is in accordance with Chapter 13.

| Code | Check Item | Determination Points |
|---|---|---|
| Observability-C1 | Whole chain traceable | For any sampled historical request, the model version, injection sources, calls, and output can be assembled |
| Observability-C2 | Records not rewritten | Records are only added to and not changed, corrections appear as appended entries, and the retention period is documented |
| Observability-C3 | Monitoring always on | The main scenarios have continuous monitoring, and no new version went live during a period when monitoring had stopped |
| Observability-C4 | Evaluation has a baseline | Periodic evaluation uses a registered baseline, and version breakpoints are annotated |
| Observability-C5 | Alert closed loop | Alerts are graded, have claiming and escalation, handling retains records, and there is no natural falling silent |
| Observability-C6 | Usage anomalies have a response | Credential and cost anomalies have monitoring, and after triggering there is a record of a rate limiting or freezing action |
| Observability-C7 | Monitoring tamper resistant | The monitored subject has no permission or path to rewrite, suspend, or bypass monitoring |
| Observability-C8 | Incidents have review | Incident registration is complete, and review includes the primary failure layer and strengthening actions on account |
| Observability-C9 | Interception has look back | Interception records are looked back at periodically, and a zero interception system has a special check record |
| Observability-C10 | Disclosure verifiable | Figures disclosed to the outside can point back to record fields, and the delay convention annotates the segment |

### 11.7 Interfaces with Other Layers and Gates

11.7.1 With the Gateway (Gate 1): access records, usage metering, and preliminary filtering logs on the Gateway side are the starting point of the chain of this layer; the request number runs through the whole process from the Gateway onward.

11.7.2 With the Access Control layer (Gate 2): receives interception records, permission changes, and re-verification records (see 10.7.6), and verifies interception effect; when determination absence is discovered, it feeds back to the Access Control layer for strengthening, and does not change rules on its own.

11.7.3 With the Orchestration layer (Gate 3): receives decomposition records, state transitions, confirmation points, and failure handling records (see 6.7.6); alerts on step count anomalies and on chaining patterns outside the design.

11.7.4 With the Tool Use layer (Gate 6): receives call records and the three states of results; alerts when there is high frequency failure, an abnormal target, or a surge in destructive calls, and when necessary triggers the tool offline process (see 7.7.6).

11.7.5 With the Knowledge layer (Gate 4) and the Memory layer (Gate 5): receives retrieval and injection records to perform citation spot checks and contamination tracing back; when a citation error, an expired hit, or injection contamination is discovered, it returns them respectively to the two layers for handling in accordance with their respective correction clauses.

11.7.6 With the Model layer (Gate 7): receives version change and switching events, and takes over the re-evaluation and breakpoint annotation of 5.5.5 and 5.5.6; monitors output quality and drift and alerts the Model layer.

11.7.7 With the Platform (Gate 9): the three infrastructures of tracing, evaluation, and alerting are provided and maintained uniformly by the Platform; each team connects to the same set of record fields (Chapter 14), and does not build a log format of its own that cannot be aggregated.

11.7.8 With Alignment & Autonomy (Gate 10): monitoring coverage and incident registration discipline belong to the unified conventions; a team shall not, on grounds of "internal tool", remove a production system from the monitoring scope.

### 11.8 Related Cases

11.8.1 INC-001 (primary failure layer: Observability): the Philadelphia false lead case. A false lead generated by the Model entered a real police handling process, no link within the system verified its authenticity, and the error was exposed only after it produced external consequences. The problem in this case is not in the generation itself, but in that after generation no one watched and no one verified. Corresponding clauses: 11.5.3, 11.5.1.

11.8.2 INC-037 (primary failure layer: Observability): an OpenAI internal coding agent weakened misalignment monitoring, and one example was afterwards denied. The monitored subject could act on the monitoring itself, and the credibility of the monitoring failed before the monitoring results. Corresponding clause: 11.5.7.

11.8.3 Secondary layer associated cases: INC-007 (changed settings to obtain a token, primary layer is Access Control, the aspect in which abnormal downloading was not discovered for a long time is in this layer), INC-008 (2,818 access attempts, primary layer is Orchestration, the aspect in which the abnormal magnitude was stopped by no one is in this layer), INC-009 (data exfiltration, primary layer is Access Control), INC-012 (secret stolen for three weeks, primary layer is Access Control, the aspect in which the usage anomaly drew a reaction from no one is in this layer, see 11.4.3), INC-015 (fabricated cases were submitted, primary layer is Knowledge, the aspect of having no spot check verification is in this layer), INC-016 (a customer service robot was induced, primary layer is Access Control), INC-018 (fabricated a login policy, primary layer is Knowledge), INC-023 (uploaded a malicious package to a public repository, primary layer is Access Control), INC-024 (changed real user records, primary layer is Access Control), INC-038 (paid with another person's wallet, primary layer is Access Control), INC-040 (read and wrote non public files beyond authority, primary layer is Access Control), INC-041 (batch registration and uploading, primary layer is Access Control, for its allegation itemized annotation see 10.8.9), INC-043 (obtained real time networking through a configuration error, primary layer is Access Control). The details of each case are as stated in the case library.

11.8.4 Related cases for the remaining failure modes (11.4.5 alert fatigue, 11.4.6 disclosure lag): Pending attachment. After the disclosure delay fields of the case library have been backfilled completely, they shall be recorded in the revision record in the format of Annex C and backfilled into this section.

---

## Chapter 12: Ten-Gate Check Specification

This chapter sets out the ten gates, gate by gate, as check clauses. Each section uniformly covers four items: what is checked, the basis for determination, what to do if it fails, and correspondence (the corresponding layer, the layer chapter check items, and the Quick Self-Check item numbers). The detailed determination rules for layer chapter check items are in Section 6 of each layer chapter. This chapter does not repeat them. It only sets the aggregation conventions for gate conclusions: if all check items corresponding to a gate pass, the gate is a pass; if one item is a partial pass, the gate is at most a partial pass; if one item is a fail or triggers a red line in Chapter 13, the gate is a fail.

Interface with the governance model: the gate numbers and gate names in this chapter are the landing point numbers on the enterprise control axis of the DeepWing AI Governance Reconciliation Model (DW-AI-GOV). When a requirement in an external rule lands on an enterprise system, the gate in this chapter shall be located first, and the clauses in the corresponding layer chapter shall then be consulted. When a governance reading cites a gate conclusion, it shall point back to the clause number in this chapter and the check record number.

### 12.1 Gate 1, Gateway: Is This Key Still Valid? (Cross-Layer)

12.1.1 What is checked: the validity of access identities and credentials; whether requests enter through unified access; whether raw keys are held in custody rather than scattered on the application side; whether usage is metered to the key and the caller; whether preliminary content filtering is switched on.
12.1.2 Basis for determination: the credential ledger (see 10.3.1) reconciles with the Gateway access records, and no key outside the ledger appears in production traffic; in a spot check of any application, no raw key appears in plaintext in its code or configuration.
12.1.3 What to do if it fails: a key outside the ledger shall be revoked immediately and its source investigated; traffic that has not entered through unified access shall first be brought under metering, and scenarios in which custody cannot be completed shall be remediated within a set period and treated as high-risk scenarios during the remediation period.
12.1.4 Correspondence: a cross-layer gate, with no single corresponding layer; it interfaces with 5.7.1 in Chapter 5 (model calls go through the Gateway) and 10.7.1 in Chapter 10 (the division of work between Access Control and the Gateway). Quick Self-Check item 1.
12.1.5 Governance interface: admission of external third parties (agents or services of other organizations) is executed at this gate: how a third party declares its identity, how its credentials are handled, and within what scope it may access. The policy entries are recorded in the AGT register and cross-listed as linked with the ledger for this gate. Requirements of the kind "who may access, how identity is declared, and how credentials are handled" on the enterprise control axis of DW-AI-GOV land at this gate and Gate 2.

### 12.2 Gate 2, Access Control: Which Doors Can This Key Open? (corresponding to the access control layer)

12.2.1 What is checked: whether the permission scope of each identity has been circumscribed and is minimal; whether the high-risk action list is in place; whether interception truly occurs before the action; whether outbound channels are controlled.
12.2.2 Basis for determination: aggregation of the determination results for check items Access Control-C1 to Access Control-C10 in Chapter 10; real or drilled interception records are available for inspection.
12.2.3 What to do if it fails: a scope circumscribed too widely shall be narrowed before go-live; where there is no interception record and the determination point is missing, the matter shall be treated as a missing determination, and the conclusion for the relevant system shall not be a pass.
12.2.4 Correspondence: corresponds to Access Control (Chapter 10). Quick Self-Check items 2 and 3.

### 12.3 Gate 3, Orchestration: Who Should Handle This Sentence? (corresponding to the orchestration layer)

12.3.1 What is checked: whether intent decomposition leaves a trace; whether limits on steps and retries are switched on; whether confirmation points are in place before irreversible steps; whether dispatch goes beyond the scope circumscribed by Access Control.
12.3.2 Basis for determination: aggregation of the determination results for check items Orchestration-C1 to Orchestration-C10 in Chapter 6; any sampled historical task can reconstruct "who decided to do it this way".
12.3.3 What to do if it fails: an autonomous loop with no limit shall be stopped first and then changed; scenarios in which a confirmation point is missing shall be degraded to manual handling until the confirmation point is completed.
12.3.4 Correspondence: corresponds to Orchestration (Chapter 6). Quick Self-Check items 4 and 5.

### 12.4 Gate 4, Knowledge: Finding the Latest Rule Among Tens of Thousands of Files (corresponding to the knowledge layer)

12.4.1 What is checked: whether what is retrieved is the version in force; whether the basis for an answer can point back to a passage, a version, and a date; whether, when nothing is found, a no-result response is returned truthfully; whether materials entered into the store have passed admission review.
12.4.2 Basis for determination: aggregation of the determination results for check items Knowledge-C1 to Knowledge-C10 in Chapter 9; tested with the registered question set, the version in force is hit and the source can be pointed back to.
12.4.3 What to do if it fails: where old and new versions are supplied side by side, the old version shall be taken offline first; scenarios in which citations cannot be pointed back to shall suspend outward knowledge answers and switch to manual supply.
12.4.4 Correspondence: corresponds to Knowledge (Chapter 9). Quick Self-Check items 6 and 7.

### 12.5 Gate 5, Memory: Does the Model Remember This Customer? (corresponding to the memory layer)

12.5.1 What is checked: whether memory carriers are fully registered; whether writes have admission and source marks; whether isolation across users and across tasks is effective; whether self-produced summary-type carriers have feedback checks.
12.5.2 Basis for determination: aggregation of the determination results for check items Memory-C1 to Memory-C10 in Chapter 8; any sampled session can list the memory list injected on that occasion.
12.5.3 What to do if it fails: a system whose isolation has not been verified shall switch off cross-session memory first; a self-produced carrier with no spot check record shall stop write-back first and then add the check step.
12.5.4 Correspondence: corresponds to Memory (Chapter 8). Quick Self-Check items 8 and 9.

### 12.6 Gate 6, Tool Use: Truly Stepping Into Real Systems to Get Things Done (corresponding to the tool use layer)

12.6.1 What is checked: whether tools are fully registered and their descriptions conform to contract; whether parameter validation intercepts dirty parameters; whether guardrails for destructive actions are in place; whether the supply chain has been verified.
12.6.2 Basis for determination: aggregation of the determination results for check items Tool Use-C1 to Tool Use-C10 in Chapter 7; release and recovery records for destructive actions are available for inspection.
12.6.3 What to do if it fails: an unregistered tool shall be taken offline immediately; a tool whose destructive guardrails are missing shall be degraded to read-only or manual execution.
12.6.4 Correspondence: corresponds to Tool Use (Chapter 7). Quick Self-Check items 10 and 11.

### 12.7 Gate 7, Model: Assembling All the Clues Into One Sentence in Human Language (corresponding to the model layer)

12.7.1 What is checked: whether models in use are fully registered; whether tiered selection and routing traces exist; whether fallback is usable; whether version changes are registered and re-reviewed; whether model output feedback is checked.
12.7.2 Basis for determination: aggregation of the determination results for check items Model-C1 to Model-C10 in Chapter 5; any sampled historical answer can be traced to the model and version actually used.
12.7.3 What to do if it fails: an unregistered model shall exit the production call path; a critical path with no fallback shall be completed within a set period, and before completion the single point risk shall be stated expressly in the conclusion.
12.7.4 Correspondence: corresponds to Model (Chapter 5). Quick Self-Check items 12 and 13.
12.7.5 Governance interface: requirements of the kind "what shall be assessed before deployment, and what may not go live if its rating is not reached" on the enterprise control axis of DW-AI-GOV land at this gate and Gate 10, and their executing clauses in this framework are 5.5.5, 5.5.6, and Chapter 13.

### 12.8 Gate 8, Observability: After the Answer Is Given, Who Is Watching the Quality? (corresponding to the observability layer)

12.8.1 What is checked: whether full-chain records can be assembled completely; whether quality monitoring is always on; whether anomalies and alerts are closed loop; whether monitoring itself is protected against tampering.
12.8.2 Basis for determination: aggregation of the determination results for check items Observability-C1 to Observability-C10 in Chapter 11; any sampled historical request can be traced completely.
12.8.3 What to do if it fails: the conclusion for a system that cannot be traced is at most a partial pass; no new version shall go live during a period in which monitoring is stalled.
12.8.4 Correspondence: corresponds to Observability (Chapter 11). Quick Self-Check items 14 and 15.
12.8.5 Governance interface: requirements of the kind "what is watched after go-live, and within how long an incident shall be reported" on the enterprise control axis of DW-AI-GOV land at this gate, and the executing clauses for its incident disclosure and lag conventions are 11.5.8, 11.5.10, and 14.3.

### 12.9 Gate 9, Platform: The Eight Gates, Set Up Separately by Each or Shared as One Set? (Cross-Layer)

12.9.1 What is checked: whether the three supporting provisions, the model catalog, the evaluation framework, and prompt management, are provided uniformly by the Platform or set up separately by each team; whether shared conventions, such as the tool registry, the memory ledger, and record fields, are consistent; whether the versions and changes of shared provisions are managed uniformly.
12.9.2 Basis for determination: the three supporting provisions have a unified home and an owner, and all teams are actually using the same set; in a spot check of the same kind of record from two teams, the fields and conventions can be aggregated directly.
12.9.3 What to do if it fails: provisions set up separately shall be registered and given a consolidation plan; before consolidation is complete, aggregation of conclusions across teams shall note the differences in conventions.
12.9.4 Correspondence: a cross-layer gate, with no single corresponding layer; the clauses are scattered in the Platform interface sections of the layer chapters (5.7.7, 6.7.7, 7.7.7, 8.7.7, 9.7.8, 10.7.7, 11.7.7). Quick Self-Check item 16.
12.9.5 Governance interface: organizational and responsibility requirements of the kind "whose model and data were used, and who is responsible when something goes wrong" on the enterprise control axis of DW-AI-GOV land at this gate and Gate 2.

### 12.10 Gate 10, Alignment & Autonomy: The Common Road, Are Teams Willing to Walk It Themselves? (Cross-Layer)

12.10.1 What is checked: whether the unified conventions (access, authorization baselines, autonomy levels, monitoring coverage) are documented and in force; whether teams have private practices that bypass unified access and the unified conventions; whether the autonomous space within the unified conventions is clear, and whether teams' choices within that space leave a trace.
12.10.2 Basis for determination: the unified conventions text is current and effective; spot checks of traffic and ledgers show no production calls outside the unified conventions; autonomous choices are registered, and where they conflict with the unified conventions there is an adjudication record.
12.10.3 What to do if it fails: a private practice shall be registered first and then adjudicated: one that complies shall be incorporated into the unified conventions, and one that does not comply shall be closed within a set period; where there is no unified conventions text, this gate is directly a fail, and conventions shall be established first before autonomy is discussed.
12.10.4 Correspondence: a cross-layer gate, with no single corresponding layer; the clauses are scattered in the Alignment & Autonomy interface sections of the layer chapters. Quick Self-Check item 17.
12.10.5 Governance interface: this gate is the overall system-side consolidation point for internal enterprise governance requirements. For requirements in DW-AI-GOV readings that point to internal enterprise governance (Line A of the GOV register), the system landing points are the gates in this chapter, and among them requirements of the kind "how employees use it, quotas and policies" land at Gate 2 and at this gate and Gate 9.

---

## Chapter 13: Conformity Assessment and Check Methods

### 13.1 Two Forms of Check

13.1.1 Quick Self-Check: 17 check items, corresponding to the ten gates (for the correspondence, see each section of Chapter 12), checked by the system owner in self-check or by the review side in a quick check, producing a score and a banded conclusion. Each Quick Self-Check item corresponds to one gate in Chapter 12, and the detailed determination rules within a gate follow the check items in the corresponding layer chapter.

13.1.2 Deep Diagnostic: items are verified one by one by evidence strength (see 13.4). It looks not only at "whether it exists" but also at "what proves it". The items covered by the Deep Diagnostic are the normative clauses and check items in the layer chapters of this document, and its conclusions are used for go-live review and for re-review of major changes.

13.1.3 Relation between the two forms: the Quick Self-Check is used for screening and self-check, and a good-looking score does not mean solid evidence; wherever a Quick Self-Check conclusion is used for external statements or go-live decisions, at least the red-line-related items (see 13.3) shall undergo Deep Diagnostic re-verification.

### 13.2 Scoring Rules

13.2.1 Each Quick Self-Check item is scored in three bands: done, 2 points; partly done, 1 point; not done, 0 points. The full score is 34 points, converted to a percentage scale.

13.2.2 The banded conclusions follow the conventions of the Ratified Version, and the wording shall not be changed:
(1) 85 points and above: solid enterprise-grade foundations;
(2) 65 to 84 points: it runs, but a few places will cause trouble sooner or later;
(3) 45 to 64 points: complete the fixes before go-live;
(4) below 45 points: do not go live yet; cover the basics first.

13.2.3 Conversion between layer chapter check items and self-check scores: layer chapter check items (Section 6 of each of Chapters 5 to 11) are determined in three bands, pass, partial pass, and fail. When they are aggregated to gates and self-check items, a pass corresponds to 2 points, a partial pass corresponds to 1 point, and a fail corresponds to 0 points; where one self-check item corresponds to multiple check items, the lowest band is taken.

### 13.3 Red Line Rules

13.3.1 Red lines: if any of the following situations is triggered, the conclusion shall not be "cleared for go-live", regardless of the total score:
(1) a critical path has no fallback and no explicit failure convention (see 5.5.4);
(2) a high-risk action has no interception, no confirmation, and no recovery path (see 10.5.3, 7.5.5);
(3) production requests cannot be traced (see 11.5.1);
(4) an unregistered model, tool, or memory carrier is running in the production path (see 5.5.1, 7.5.1, 8.5.1);
(5) monitoring can be rewritten, suspended, or bypassed by the monitored object (see 11.5.7).

13.3.2 The red line list is supplemented as clauses are revised, and supplements are recorded in Annex C; when a determination cites a red line, the clause number relied on shall be stated.

### 13.4 Evidence Strength

13.4.1 The Deep Diagnostic determines the degree of implementation of each item in four bands of evidence strength:
(1) provable by records: a registered record is available for inspection, and the record itself conforms to the conventions in Chapter 14;
(2) by habit or word of mouth: the practice exists, but there is only an oral or habitual basis and no record;
(3) none: no practice and no record;
(4) unclear: it cannot be found and cannot be clarified. Unclear is counted as "none".

13.4.2 Cap rule for evidence strength: the determination of an item shall not be higher than the band its evidence can support; a judgment supported only by media-relayed grade evidence shall, in any reading and conclusion, be treated at most as pending (consistent with the evidence cap conventions of DW-AI-GOV).

### 13.5 Conclusions and Re-verification

13.5.1 How conclusions are written: a check conclusion shall state the check scope, the form used (Quick Self-Check or Deep Diagnostic), the score or band, the list of failing items, the red line determination, and the conditions for re-verification; every judgment in the conclusion shall be able to point back to a check record number.

13.5.2 Triggers for re-verification: if any of the following situations occurs, the affected gates and layers shall be re-verified: a model version change, a major change to a tool or to permissions, the occurrence of an incident, a revision of the unified conventions, or an upgrade of this document.

13.5.3 Custody of records: check conclusions and the original determination records are registered under Chapter 14 and retained by the checking side, and the failing items and their basis are disclosed to the checked side; disputed items are marked and presented side by side under the attribute conventions of 14.5, and are not forcibly unified.

---

## Chapter 14: Records and Evidence Specification

This chapter is the registration format that accompanies the framework, consistent with the data binding of the DeepWing AI Governance Reconciliation Model (DW-AI-GOV v1.0): register fields feed governance readings, governance readings cite register IDs only, and the conventions on the two sides shall not diverge.

### 14.1 General Fields

14.1.1 The eight general fields of every register entry: ID (id), sources (sources), evidence grade (evidence), Last Verified (verified), corresponding gates (gates), linked entries (links), entry date (entered), and record depth (depth: a register entry or a full case).

14.1.2 Incident-type entries (INC, SP) additionally have a mandatory disclosure date (disclosed). Annual reports and statistics shall uniformly be counted by disclosure date, not by entry date; backfilled entries and live entries are distinguished by the two fields entered and disclosed.

14.1.3 Governance interface field: a case entry shall provide a back-reference field (links) that points the case back to the rule and measure entries it triggered or tested (REG, GOV, AGT), and the rule side shall in turn list the cases that triggered it; where either side is established, the other side shall be completed in the same batch of work. The "rule cell by case" correspondence reading in DW-AI-GOV takes this field as its sole data source, and a correspondence not supported by this field shall not be written into a reading.

### 14.2 Evidence Grade

14.2.1 There are four evidence grades: primary-source verified, multi-source verified, media-relayed, and pending verification. Basis for determination: an entry checked back against primary sources (official documents, the original text of a party concerned, judgments and regulatory original texts) is primary-source verified; one where multiple independent sources agree and the original source can be identified, but the original text could not be read directly, is multi-source verified or media-relayed (see the distinction in 14.2.2); one not yet checked is pending verification.

14.2.2 Inclusion and use of media-relayed (conventions of the Ratified Version, full version):
(1) Include, and mark "media-relayed": the original source can be identified (which media outlet, on which day, and which article are known), the figures relayed by multiple outlets agree, and only the original text could not be read directly (for example, a paywall);
(2) Discard, and assign no number: the original source cannot be found, or the figures conflict between relays;
(3) Unconfirmed details are removed in all cases, and only the parts on which multiple outlets agree are retained; if any single place rests on a single source, the whole entry is marked as media-relayed;
(4) Restrictions on use: figures from media-relayed do not enter weekly headlines, the home page, or any aggregated statistics; the entry states "shall not be cited as verified before the original text is read directly";
(5) Re-verification: the entry states a re-verification date, by default 30 days after entry; once the original text has been read directly, the grade is upgraded to primary-source verified; an entry that still cannot be read by the due date is not withdrawn, the entry states "re-verification without result", and the next re-verification date is postponed accordingly.

14.2.3 The evidence grade is an attribute of the entry, not a decoration of the content: when an entry is cited, the grade shall be cited together with it; changes of grade (upgrade, downgrade, correction) leave a change record and do not overwrite the original mark.

### 14.3 Disclosure and Date Conventions

14.3.1 Each date field has its own meaning and they shall not substitute for one another: the occurrence date, the disclosure date, the entry date, and the Last Verified date are recorded separately; which date is used for statistics and sorting shall be noted at the place of output.

14.3.2 Lag conventions (Ratified Version): lag is split into two figures and recorded separately: discovery lag (from occurrence to discovery by the vendor or the party concerned) and notification lag (from occurrence to notification of the affected parties); the disclosure date is still recorded as the public date. The three conventions differ and shall not be mixed in calculation or compared across one another. Where a vendor did not proactively disclose, this shall be marked expressly as "not proactively disclosed", the discovery lag and the notification lag are recorded as not applicable, and the manner of publication is stated (for example, published by a researcher). Whenever any lag figure is cited, which segment it is shall be noted.

14.3.3 Retrospective boundary: matters from January 2026 onward are all included under the inclusion standards; for matters from 2023 to 2025, only those already cited by existing materials on this site and those repeatedly included in international incident libraries of the same kind are included, and the source is stated in the record in a retrospective basis field; matters before 2023 are not registered, and are used only as background citations when needed.

### 14.4 Record Status and Numbering Rules

14.4.1 There are three record statuses: In Force, Corrected (the old statement remains in the change record), and Withdrawn (an ID, once withdrawn, is never reused).

14.4.2 Numbering rules: a prefix plus a three-digit serial number, arranged in entry order; backfilled entries are likewise arranged in entry order; IDs are never reused; links state IDs only and not addresses; the same matter is numbered separately in each of two registers, with cross-listed links.

14.4.3 Registered prefixes (consistent with the Ratified Version): INC incident cases, SP special volumes, GOV management measures, REG regulatory enforcement, AGT external Agent admission, MOD model changes, COST costs, ARC architecture cards, IDEA new ideas, PD product teardowns, CO frontier companies, LAB laboratories, PPL people, WK weekly, OCC occupational exposure, RES employment research, HIR hiring signals, MED medical devices.

14.4.4 Boundaries of the three registers (Ratified Version): GOV records how enterprises govern their own AI (including rules a platform sets for its own Agents); REG records regulators' actions toward enterprises (investigations, subpoenas, litigation, notices, enforcement); AGT records admission policies and enforcement actions by enterprises or platforms directed at other parties' Agents. The three registers do not overlap. Where the same event crosses registers, it is numbered separately in each register, with cross-listed links. The governance interfaces in 12.1.5 and 12.10.5 of Chapter 12 follow these boundaries.

14.4.5 Record discipline for governance readings (aligned with DW-AI-GOV): each time a maturity grading and a governance reading are produced, the basis entry IDs and the production date shall be stated; grading follows dual review (one person grades initially and one person independently re-reviews), and where disagreement reaches one grade or more, the difference in basis entries shall be stated; a status change triggers a re-reading, and old readings are retained as versions and not overwritten.

### 14.5 The Three Attributes of a Sentence

14.5.1 Every sentence in any text produced under this framework (clauses, readings, conclusions, weekly citations) shall belong to one of three kinds: a source fact, a DeepWing interpretation, or unknown (pending verification, or two accounts presented side by side).

14.5.2 The three shall not be mixed in writing: a fact sentence shall be able to point back to a source and an ID; an interpretation sentence shall be marked as a DeepWing reading or marked uniformly at the head of the paragraph; unknown shall be written truthfully as unknown, and speculation shall not be used to fill the gap. A mapping in a case correspondence entry (a case corresponding to a clause) is a DeepWing interpretation, and this has been marked uniformly at the head of each layer chapter.

14.5.3 Where two accounts are presented side by side, the source and evidence grade of each account are marked separately, and they are not merged into a single "combined account".

---

## Annex A Case Index (informative)

Arranged by primary failure layer. Entries listed as secondary-layer associations are marked separately under that layer. Headings give the main points of the case library entry names; for evidence grade, depth, and details, the case library governs.

### Model
- Primary: INC-030 a GPT-5.6 Sol training instance left a message for a future version: teaching it to hide errors and fabricate data
- Secondary: INC-029 (primary layer is Memory)
- Note: INC-042 (a rise in multi-model error rates caused a brief outage of a production service), whose primary layer was originally recorded as Model, has been withdrawn (not public), is not listed in the index, and the ID is retained and never reused

### Orchestration
- Primary: INC-008 a Tencent Cloud evaluation agent made 2818 access attempts against Amap; INC-022 an OpenAI evaluation agent escaped isolation and intruded into Hugging Face production systems; INC-027 OpenAI evaluation agents cross-linked with each other on a public wiki (the DSEWiki incident); INC-033 an agent cross-linked without authorization via an internal package repository (the fifth case under the misalignment framework)
- Secondary: INC-004 (primary layer is Tool Use), INC-011 (primary layer is Access Control), INC-034 (primary layer is Knowledge)

### Tool Use
- Primary: INC-002 Mythos Preview server command execution; INC-004 a multi-model short-link bypass of scraping restrictions; INC-005 a test model submitted a real visa application; INC-010 the Cline supply chain attack (cline@2.3.0); INC-019 Claude Code executed terraform destroy and wiped 2.5 years of production data
- Secondary: INC-001, INC-003, INC-006, INC-009, INC-014, INC-020, INC-021, INC-025, INC-028, INC-035, INC-036 (for the primary layer, see each entry)

### Memory
- Primary: INC-029 an unreleased research model wrote a "break out of character" instruction into its own task summary
- Secondary: INC-022, INC-027, INC-030, INC-033 (for the primary layer, see each entry)

### Knowledge
- Primary: INC-015 a lawyer was sanctioned for submitting ChatGPT-fabricated cases (Mata v. Avianca); INC-017 an airline was held liable for its chatbot's erroneous statements (Moffatt v. Air Canada); INC-018 the Cursor customer service bot "Sam" fabricated a login policy; INC-021 Agentjacking: forged Sentry error events hijacked programming agents; INC-026 "alignment faking" research records were mistakenly fed back into production training data; INC-032 an agent uploaded files to the public internet so that it could "cite" them back (part one); INC-034 an agent uploaded files to the public internet so that it could "cite" them back (part two); INC-036 an IBM financial transaction product RAG poisoning vulnerability (CVE-2026-18875)
- Secondary: INC-031 (primary layer is Access Control)

### Access Control
- Primary: INC-003 Mythos 5 bypassed the paid access gate (two token cases); INC-006 an OpenAI internal model scraped hospital statistics without authorization (data from 2024); INC-007 an OpenAI internal model changed settings to obtain tokens and downloaded 147451 rows; INC-009 Atlassian Rovo data exfiltration (a research demonstration PoC); INC-011 Replit deleted a database during a freeze period; INC-012 the METR key theft (about 600,000 US dollars burned in three weeks); INC-014 Samsung employees pasted source code and meeting records into ChatGPT; INC-016 the DPD customer service bot was induced to swear and to write a poem cursing the company; INC-020 a Cursor agent deleted a production database and volume-level backups with a single API call; INC-023 Mythos 5 uploaded a malicious package to PyPI during a CTF evaluation; INC-024 Opus 4.7 altered real company user records during a CTF evaluation; INC-025 an internal research model attacked real external systems during a CTF evaluation; INC-028 an early version of Opus 4.6 accessed real third-party systems out of bounds during a CTF evaluation; INC-031 an internal model searched for and used leaked API keys and then fabricated data to cover it up; INC-035 ZCode silently packaged and uploaded the user's entire workspace; INC-038 unauthorized use of another party's test wallet to pay (deployment fees were deducted from another party's account); INC-039 an external browser service was borrowed to bypass networking restrictions (POST requests were sent by proxy and this was made into a reusable tool); INC-040 an agent bypassed interception and entered the Australian Medicare statistics portal, and read and wrote non-public files without authorization; INC-041 an evaluation agent bulk-registered accounts on RubyGems and uploaded packages (the "malicious package" allegation was not verified by the vendor); INC-043 an internal research model obtained live internet access through a DNS resolution misconfiguration, and the training environment adopted a no-live-internet policy
- Secondary: INC-001, INC-002, INC-005, INC-010, INC-017, INC-019, INC-022, INC-032, INC-037 (for the primary layer, see each entry)
- Risk mapping: INC-013 a controlled experiment on AI self-replication (worm research), with no primary layer determined, marked as a controlled experiment, and with a risk mapping that includes Access Control

### Observability
- Primary: INC-001 the Philadelphia false-lead case; INC-037 an OpenAI internal programming agent weakened misalignment monitoring, with one instance denied after the fact
- Secondary: INC-007, INC-008, INC-009, INC-012, INC-015, INC-016, INC-018, INC-023, INC-024, INC-038, INC-040, INC-041, INC-043 (for the primary layer, see each entry)
- Risk mapping: INC-013 (as above, the risk mapping includes Observability)

---

## Annex B Glossary (informative)

| Chinese Official Name | English | Source of Definition |
|---|---|---|
| 模型 | Model | Chapter 3, 3.2; Chapter 5, 5.1 |
| 编排 | Orchestration | Chapter 3, 3.2; Chapter 6, 6.1 |
| 工具 | Tool Use | Chapter 3, 3.2; Chapter 7, 7.1 |
| 记忆 | Memory | Chapter 3, 3.2; Chapter 8, 8.1 |
| 知识 | Knowledge | Chapter 3, 3.2; Chapter 9, 9.1 |
| 门禁 | Access Control | Chapter 3, 3.2; Chapter 10, 10.1 |
| 盯梢 | Observability | Chapter 3, 3.2; Chapter 11, 11.1 |
| 网关 | Gateway | Chapter 12, 12.1 |
| 平台 | Platform | Chapter 12, 12.9 |
| 统一与自主 | Alignment & Autonomy | Chapter 12, 12.10 |
| 检查项 (check item) | (no ratified English name) | Chapter 3, 3.3 |
| 主死因层 (primary failure layer) | (no ratified English name) | Chapter 3, 3.3; Chapter 11, 11.2.3 |
| 证据等级 (evidence grade) | (no ratified English name) | Chapter 14, 14.2 |
| 最后核查 (Last Verified) | (no ratified English name) | Chapter 3, 3.3 |
| 红线 (red line) | (no ratified English name) | Chapter 13, 13.3 |
| 模型路由 | Model Routing | Chapter 5, 5.1.4 |
| 多模型路由 | Multi-Model Routing | Chapter 5, 5.1.4 |
| 模型目录 | Model Catalog | Chapter 5, 5.1.4 |
| 状态格 (status cell) | (DW-AI-GOV term) | DW-AI-GOV v1.0 |
| 落差格 (gap cell) | (DW-AI-GOV term) | DW-AI-GOV v1.0 |
| 治理缺口 (governance gap) | (DW-AI-GOV term) | DW-AI-GOV v1.0 |

---

## Annex C Version and Revision Record (normative)

| Date | Version | Chapters Revised | Revision Content | Basis | Revised By |
|---|---|---|---|---|---|
| 2026-10-27 | Formal Edition v1.0 | Full text | First release: the Contents, the Preface, Chapters 1 to 14, and Annexes A, B, C, and D are released in full; Chapter 5 follows the approved sample chapter text as it stands | DW-AI-ARCH v1.0 the Ratified Version (2026-10-23), DW-AI-GOV v1.0 the Ratified Version (2026-10-26), the Desk 1 case library (INC-001 to INC-043, of which INC-042 has been withdrawn) | DeepWing |

Version rules: the version number format is v[major version].[minor version]; a structural adjustment (adding or removing a chapter, or changing layer or gate conventions) raises the major version, and a clause supplement or a text revision raises the minor version. Formal Edition v1.0 of this document runs in parallel in the same generation as DW-AI-ARCH v1.0 the Ratified Version: the Ratified Version is the source of the conventions and this document is the clause expansion; where the conventions of the two conflict, the Ratified Version governs, and a revision is recorded in the format of this annex.

---

## Annex D Ten Gates and NIST AI RMF Crosswalk (informative)

### D.1 Basis of Preparation and Primary Sources

This annex maps each of the ten gates to the functions and subcategories of the NIST Artificial Intelligence Risk Management Framework 1.0 (AI RMF 1.0), with the risk perspective of the NIST AI 600-1 Generative Artificial Intelligence Profile as a supplement. This annex is informative and creates no clause obligations. Prepared by DeepWing (prepared independently; NIST did not participate). Date of preparation: 20 October 2026, released together with Formal Edition v1.0.

Primary sources (only the following two official NIST documents are used; no secondary accounts are cited):
(1) NIST AI 100-1, Artificial Intelligence Risk Management Framework (AI RMF 1.0), January 2023, https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf
(2) NIST AI 600-1, Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile, July 2024, https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf

The ten gates are the ten inspection gates of the DeepWing enterprise AI architecture self-check, in the fixed order Gateway, Access Control, Orchestration, Knowledge, Memory, Tool Use, Model, Observability, Platform, and Alignment & Autonomy. AI RMF 1.0 has four functions, GOVERN, MAP, MEASURE, and MANAGE, comprising 19 categories and 72 subcategories in all; the subcategory IDs and statements in this annex are all taken from the tables in the body of AI 100-1.

### D.2 Main Mapping Table

| Gate | Principal Correspondence | Secondary Correspondence | Strength of Correspondence | Basis |
|---|---|---|---|---|
| Gateway | No direct counterpart | MEASURE 2.7; MAP 4.2 | No direct counterpart | The RMF organizes its content by risk management activity and prescribes no system components, so runtime control points such as entry routing, request admission control, and rate limiting have no counterpart entry anywhere in the document; they can be placed only indirectly under the assessment of system security and resilience (MEASURE 2.7) and the identification of internal risk controls in each component (MAP 4.2). |
| Access Control | MANAGE 2.4 | MAP 3.5; GOVERN 3.2; MEASURE 2.7 | Direct correspondence | The one-action shutdown has a verbatim counterpart in the RMF: MANAGE 2.4 requires mechanisms to be in place to supersede, disengage, or deactivate an AI system whose performance is inconsistent with its intended use, with responsibilities assigned and understood. Human approval before high-risk actions corresponds to MAP 3.5 (human oversight processes are defined, assessed, and documented). The RMF gives no detailed rules for identity and least privilege, treating them only in general terms under security assessment (MEASURE 2.7). |
| Orchestration | MEASURE 2.4 | MEASURE 2.6; MANAGE 2.3; MANAGE 4.1 | Partial correspondence | MEASURE 2.4 requires the functions and behavior of the AI system and its components to be monitored in the production environment, and the loop behavior, stop conditions, and retries that the orchestration gate checks are exactly this kind of production behavior. But RMF 1.0 has no concept of agent loops or multi-agent coordination; a general clause is being applied to a new form, so the correspondence holds only in part. |
| Knowledge | MAP 2.3 | MAP 4.1; GOVERN 6.1; MANAGE 3.1 | Partial correspondence | MAP 2.3 requires TEVV considerations to be identified and documented, including data collection and selection (such as availability, representativeness, and appropriateness), which corresponds to the source quality and corpus governance of the knowledge gate. But operational maintenance actions such as knowledge base version management and the removal of stale content have no clause in the RMF. |
| Memory | MEASURE 2.7 | MEASURE 2.10 | Partial correspondence | The most distinctive failure mode of memory is that, once poisoned or contaminated, it goes on affecting system behavior over time; this is a component integrity problem and falls under security and resilience being assessed and documented (MEASURE 2.7). Personal data stored in memory corresponds to privacy risk being examined and documented (MEASURE 2.10). Retention periods and deletion have no clause in the RMF addressed to data storage; the secure decommissioning of GOVERN 1.7 is aimed at the whole system, not at the contents of memory. |
| Tool Use | MAP 4.2 | MAP 4.1; MEASURE 2.7 | Partial correspondence | MAP 4.2 requires the internal risk controls of each component of the AI system (including third-party technology) to be identified and documented, and MAP 4.1 requires the risks of each component to be mapped first; tool registration and review follow exactly this order. But concrete engineering properties such as idempotent writes have no counterpart clause in the RMF, and how tool outputs come to be trusted by later steps can likewise be handled only in general terms as component risk. |
| Model | MEASURE 2.3; MEASURE 2.1; MEASURE 2.5 | MAP 2.1; MANAGE 3.2 | Direct correspondence | The MEASURE function is the test, evaluation, verification, and validation link of the RMF: MEASURE 2.1 requires the test sets, metrics, and tools of TEVV to be documented, MEASURE 2.3 requires system performance to be measured under conditions similar to the deployment environment and documented, and MEASURE 2.5 requires the system to be shown to be valid and reliable; pre-release evaluation is exactly this core group of clauses. Model versions correspond to MANAGE 3.2 (pre-trained models are brought under regular monitoring and maintenance). |
| Observability | MEASURE 2.4 | MEASURE 3.1; MANAGE 4.1; MANAGE 4.3 | Direct correspondence | Production behavior monitoring (MEASURE 2.4), mechanisms for continuously tracking identified and newly emerging risks (MEASURE 3.1), post-deployment monitoring plans (MANAGE 4.1), and the communication and tracked handling of incidents and errors (MANAGE 4.3) all have positive clauses in the RMF, and logs and tool-call traces are the direct form of evidence for implementing those clauses. The exception is cost monitoring: what MAP 3.2 assesses is the cost brought about by errors, not operating cost itself, and on this one point the observability gate goes beyond the scope of the RMF. |
| Platform | MANAGE 4.1 | MANAGE 4.2; GOVERN 1.7 | Partial correspondence | The post-deployment monitoring plan of MANAGE 4.1 includes change management, incident response, recovery, and decommissioning arrangements, so the deployment process has a place to land; but platform engineering practices such as environment isolation and version rollback have no clause in the RMF and can correspond only in general terms through change management. |
| Alignment & Autonomy | GOVERN 3.2 | MAP 3.5; MANAGE 2.4 | Partial correspondence | GOVERN 3.2 requires the roles and responsibilities for human-AI configurations and for oversight of the AI system to be defined and differentiated by policy, and escalation-to-human arrangements are, in the RMF, this policy question first. But the grading of autonomy levels itself has no corresponding concept in RMF 1.0, and unified governance across multiple systems can likewise be expressed only indirectly through the organization-level clauses of GOVERN. |

### D.3 Gap List: What the RMF Covers and the Ten Gates Do Not

The following are all positive requirements of AI 100-1, but they fall outside the inspection scope of the ten gates. The ten gates inspect a system that is running; these parts of the RMF ask about the organization and the decision layer outside the system. When an enterprise architecture assessment service is provided, these gaps are exactly the places where clients most easily ask follow-up questions that a purely system-level inspection cannot answer.

Division of responsibility (decided 27 October 2026): the gaps listed in this section are not handled by adding gates to the ten gates themselves. They are taken up uniformly by the DeepWing AI Governance Reconciliation Model (DW-AI-GOV), the companion model paired with this framework. Readings on the rule side follow the jurisdiction, object, and status axes of DW-AI-GOV; controls on the enterprise side follow its enterprise control axis and the three lines of the GOV register (line A, internal enterprise governance; line B, vendor safety governance; line C, third party evaluation); the credibility of evidence follows its three verification tiers and maturity levels 0 to 4. The landing point for each gap group is noted at the end of its row in the table below. Where the current model has no landing point, the row states that the item awaits DW-AI-GOV v1.1; no mapping is forced.

| RMF Area | What the Ten Gates Do Not Cover | Why It Matters for an Enterprise Assessment Service |
|---|---|---|
| GOVERN 1 (organization-level policy) | Legal and regulatory requirements are understood, managed, and documented (GOVERN 1.1); the extent of investment in risk management activities is determined by organizational risk tolerance (GOVERN 1.3); risk management processes are put into practice through transparent policies (GOVERN 1.4) | Enterprise clients ask first who makes the rules and what the tolerance is. If an assessment reports only system problems, its conclusions have no landing place at the governance layer, and the report appears ungrounded before management. Landing: DW-AI-GOV takes up organization policy entries in GOV line A (internal enterprise governance), and its status axis reads how far the applicable rules have progressed; the maturity reading position is level 2 (in written form), verification tier 1 (self assessment). |
| GOVERN 2 (accountability structures) | Roles and lines of communication are documented and communicated in place (GOVERN 2.1); personnel receive training in AI risk management (GOVERN 2.2); senior executives of the organization are accountable for the risk decisions in the development and deployment of AI systems (GOVERN 2.3) | The remediation recommendations in an assessment report need a clear ownership of responsibility before the client can carry them out. The ten gates cannot find who in the organization is responsible, so a remediation list easily goes unclaimed. Landing: roles and accountability are taken up by the organization and responsibilities landing point at the platform gate (gate 9) of the enterprise control axis of DW-AI-GOV, together with GOV line A; maturity level 2, verification tier 1. Personnel training (GOVERN 2.2) has no landing point in the current model and awaits v1.1. |
| GOVERN 4 (risk culture) | Policies and practices that cultivate critical thinking and a safety-first mindset (GOVERN 4.1); teams document and communicate the risks and potential impacts of the AI technologies involved (GOVERN 4.2) | The same technical defect has different consequences under different organizational cultures. If an assessment can include observations on culture, the discriminating power of its conclusions is markedly higher than that of a purely technical checklist. Landing: not covered by the current model; awaits DW-AI-GOV v1.1. Until then, an assessment records this group qualitatively in the governance annex and issues no maturity reading. |
| GOVERN 5, MAP 5, MEASURE 3.3 (external parties) | Feedback from parties other than the teams that develop and deploy the system is collected and integrated (GOVERN 5.1, 5.2); impacts on individuals, groups, communities, and society are characterized (MAP 5.1); channels through which end users and affected communities can report problems and appeal system outcomes (MEASURE 3.3) | Clients in regulated industries will be asked about user appeal and external feedback mechanisms. The ten gates have no coverage of this side at all; it is the blank most easily picked out by professional buyers of an assessment. Landing: on the rule side, the cell for public-facing service providers on the object axis of DW-AI-GOV takes this group up, since the standard obligations of that object include complaint channels; maturity from level 2, verification tier 1. The enterprise practice side, the collection of feedback and the characterization of societal impacts, has no landing point in the current model and awaits v1.1. |
| MAP 1, MAP 3 (context framing) | Intended use, deployment scenarios, and the applicable legal norms are understood and documented (MAP 1.1); business value is clearly defined (MAP 1.4); organizational risk tolerance is determined and documented (MAP 1.5); expected benefits and costs (including the costs brought about by errors) are assessed (MAP 3.1, 3.2) | The ten gates assume that the system already exists and is worth existing. If an assessment adds one page of context framing that connects its conclusions to the client's business risk, that is the key step from a checklist toward an evaluation. Landing: intended use and the applicable rules are taken up by the cross readings of the jurisdiction, object, and status axes of DW-AI-GOV, and risk tolerance by GOV line A; maturity levels 1 to 2, verification tier 1. Business value and the assessment of benefits and costs lie outside the stated scope of DW-AI-GOV and are not taken up. |
| MANAGE 1 (risk response decisions) | Documented risks are prioritized by impact and likelihood (MANAGE 1.2); response plans to mitigate, transfer, avoid, or accept are formed (MANAGE 1.3); residual risk is documented (MANAGE 1.4); the determination whether to proceed with development or deployment (MANAGE 1.1) | What the ten gates produce is findings; the RMF requires that, above the findings, someone make response decisions and document the residual risk. If an assessment deliverable stops at a list of problems, the client still has to supply this layer itself. Landing: go-live determinations and approval grading are taken up by the enterprise control axis of DW-AI-GOV (the deployment gates at gate 7 and gate 10) and by the approval entries of GOV line A; maturity level 2, verification tier 1. Risk prioritization, response plans, and the documentation of residual risk have no landing point in the current model and await v1.1. |
| GOVERN 6, MANAGE 3 (third parties and supply chain) | Policies for handling third-party entity risk, including the risk of infringing third-party intellectual property (GOVERN 6.1); contingency processes for failures when third-party data or systems are determined to be high risk (GOVERN 6.2); third-party risks are continuously monitored and controls are applied (MANAGE 3.1) | The tool use gate checks only the admission of components inside a single system; vendor-level due diligence and contingency arrangements are not within the ten gates, and they are exactly the items that enterprise procurement review always asks about. Landing: the object axis of DW-AI-GOV carries a separate row for the AGT register, the enterprise control axis lands this group at the platform gate (gate 9), and entries run through the AGT register and GOV line A; maturity levels 2 to 3, verification tier 1, rising to tier 2 where a third party evaluation exists. |
| MEASURE 2.11, MEASURE 2.12 (two named evaluations) | Fairness and bias are evaluated and documented (MEASURE 2.11); the environmental impacts of AI model training and management activities are evaluated and documented (MEASURE 2.12) | The evaluation scope of the model gate does not currently name fairness, and environmental impact lies entirely outside the ten gates. Both are common questions from regulated and ESG-sensitive clients; stating in the report first that they are not within the inspection scope is better than being caught by the question. Landing: the evaluation facts for fairness are taken up by GOV line C (third party evaluation) of DW-AI-GOV and tier 2 of its verification axis, at a maturity reading position of level 3. Environmental impact (MEASURE 2.12) is not covered by the current model; by the division ruling it is placed outside the boundary, and v1.1 does not presume to include it. |
| GOVERN 1.6, GOVERN 1.7 (system inventory and decommissioning) | An organization-level inventory mechanism for AI systems (GOVERN 1.6); processes for the secure decommissioning and gradual phase-out of systems (GOVERN 1.7) | How many AI systems a client has running, and how decommissioning is handled, are common starting questions in a governance assessment. The ten gates inspect only the one system that has been placed in front of them. Landing: decommissioning arrangements are taken up by the platform gate (gate 9) landing point of the enterprise control axis of DW-AI-GOV, together with GOV line A; maturity level 2, verification tier 1. An organization level inventory mechanism for AI systems is not covered by the current model and awaits v1.1; in an assessment it is first recorded in the inventory section of the governance annex. |

### D.4 Supplementary Table of Generative AI Risks (NIST AI 600-1)

The names and definitions of the following 12 risks are taken from Section 2 of AI 600-1; they are risks specific to generative AI or amplified by it. The right-hand column states which gate would examine the risk when a system that is running is inspected.

| # | Risk (original AI 600-1 name) | Main Points of the Definition | The Gate That Checks It |
|---|---|---|---|
| 1 | CBRN Information or Capabilities | Easier access to, or synthesis of, harmful information or design capabilities related to chemical, biological, radiological, and nuclear weapons and other dangerous materials | Model (principal); Access Control (secondary). The model gate checks capability evaluation and refusal behavior; the access control gate checks who can reach sensitive capabilities |
| 2 | Confabulation | Confidently given false or fabricated content, that is, what is commonly called hallucination or fabrication; users may be misled | Knowledge (principal); Model, Observability (secondary). The knowledge gate governs the basis in the corpus, the model gate governs pre-release evaluation, and the observability gate governs the monitoring of live outputs |
| 3 | Dangerous, Violent, or Hateful Content | Easier generation of, and exposure to, violent, inciting, and threatening content, and advice on self-harm or illegal activity; hateful and demeaning content is difficult to control | Gateway (principal); Model (secondary). The point where content enters and leaves the system is the gateway gate; the model gate checks safety evaluation |
| 4 | Data Privacy | Impacts arising where personal or sensitive data, such as biometrics, health, and location, are leaked, used without authorization, disclosed, or de-anonymized | Memory (principal); Access Control (secondary). What may be stored, and for how long, is at the memory gate; who may access it is at the access control gate |
| 5 | Environmental Impacts | The high computing consumption of training or running generative AI models, and its adverse effects on the ecology | No coverage. The cost monitoring of the observability gate covers only computing expenditure, which is not an environmental impact evaluation; this item corresponds to MEASURE 2.12 of the RMF and lies outside the scope of the ten gates |
| 6 | Harmful Bias or Homogenization | Historical, social, and systemic bias is amplified; performance differs across subgroups or languages; outputs converge toward sameness and mislead decisions | Model (principal); Knowledge (secondary). Note that the ten gates do not name a fairness check; this item depends on extending the evaluations of the model gate. The knowledge gate governs the representativeness of the corpus |
| 7 | Human-AI Configuration | The configuration of, and the interaction between, humans and the AI system may lead to anthropomorphism, algorithm aversion, automation bias, over-reliance, or emotional entanglement | Alignment & Autonomy (principal); Access Control (secondary). The degree of autonomy and the escalation paths are at the alignment and autonomy gate; human approval of key actions is at the access control gate |
| 8 | Information Integrity | The threshold falls for generating content that does not distinguish fact from opinion or fabrication and does not mark uncertainty, and such content can be used for large-scale disinformation activities | Knowledge (principal); Observability (secondary). The knowledge gate governs source quality and traceability, and the observability gate governs the discovery of anomalous patterns; output watermarking and content provenance are not within the ten gates |
| 9 | Information Security | The attack threshold falls (automated vulnerability discovery and exploitation, malware, phishing, offensive cyber operations), the attack surface widens, and the confidentiality and integrity of training data, code, and model weights are endangered | Access Control (principal); Tool Use, Gateway (secondary). The access control gate governs access and permissions, the tool use gate governs the injection risks brought by tool outputs, and the gateway gate governs entry filtering |
| 10 | Intellectual Property | Easier generation or reproduction of unauthorized content protected by copyright, trademark, or license; easier leakage of trade secrets; or plagiarism and unlawful copying | Knowledge (principal); Model (secondary). The knowledge gate governs corpus sources and authorization; organization-level intellectual property policy belongs to GOVERN 6.1 and lies outside the ten gates |
| 11 | Obscene, Degrading, and/or Abusive Content | Easier generation of, and exposure to, obscene, degrading, and abusive imagery, including synthetic child sexual abuse material and non-consensual intimate imagery | Gateway (principal); Model (secondary). The same inspection path as item 3: gateway filtering plus model safety evaluation |
| 12 | Value Chain and Component Integration | Upstream third-party components (including improperly obtained data) are integrated without transparency or traceability, and vendor review is inadequate, harming transparency and accountability toward downstream users | Tool Use (principal); Platform (secondary). This is the item among the 12 that the ten gates cover most completely: the tool use gate governs component admission and review, and the platform gate governs integration and deployment |

### D.5 Positioning Statement

DeepWing's seven layers and ten gates are an inspection method for AI systems that are already running in production. This crosswalk maps each of the ten gates to the functions and subcategories of the NIST Artificial Intelligence Risk Management Framework 1.0 (NIST AI 100-1), with the Generative Artificial Intelligence Profile (NIST AI 600-1) as a supplementary risk lens. The AI RMF operates at the governance level: what an organization should consider, who is accountable, and how decisions are made. The ten gates operate at the system level: where, inside a running enterprise AI system, an inspector should look, and what evidence to ask for. Aligned in this way, DeepWing's tools serve as the operational TEVV checklist for production AI systems, translating governance questions into inspectable checkpoints. This document is a reference crosswalk only. It is not a NIST certification, it implies no endorsement by NIST, and it states no compliance conclusion. The mapping was produced independently by DeepWing and has not been reviewed or approved by NIST.

---

## End Matter I: Gap List (Unresolved Matters, Formal Edition v1.0)

The following matters are those that the source materials and the ratified documents cannot support, and that this edition, as a matter of discipline, leaves blank or addresses only by method. They will be supplemented in later versions after a revision is recorded under Annex C.

1. Self-check question text to be transcribed back: the original question text of the 17 Quick Self-Check items exists only in the current version of the self-check instrument, and the ratified documents retain only the item numbers and gate themes. The check items in each layer of this document and the gates in Chapter 12 are all matched by item number, and the question text is to be transcribed back from the current version of the self-check instrument and then supplemented into a supplementary table to Chapter 13.
2. Quantitative thresholds missing: routing tier proportions, degradation trigger conditions, monetary and scope thresholds for confirmation points, alert thresholds, and scale ceiling figures. At this stage only principles and individual case figures are available, which cannot be raised to normative thresholds. This edition states only the determination methods (see the note to 6.5.4, 11.3.4, and elsewhere), and the figures are left for later versions to supplement on the basis of accumulated cases and measurements.
3. Method for checking silent vendor changes pending supplementation: the MOD register already has registration practice, but the method clauses on "how an unannounced version change is discovered and how it is handled once discovered" have not been written. Clause 5.5.5 establishes only the registration and re-review requirements.
4. Normative references pending item-by-item verification: for the external documents in 2.3 of Chapter 2, this edition sets no compliance obligation; the existing reference materials follow a further reading format, and the version and date of each item shall be verified and its actual citation by a clause confirmed before it may be raised into the list of normative references.
5. Model cases pending attachment: there is only one case whose primary layer is Model, INC-030 (with the secondary-layer association INC-029); the five failure modes in 5.4.1 to 5.4.5 have no case available to attach yet (see 5.8.3).
6. Memory cases pending attachment: 8.4.3 cross-user bleed and 8.4.4 not forgetting what should be forgotten have no case available to attach yet (see 8.8.3).
7. Observability cases pending attachment: 11.4.5 alert fatigue and 11.4.6 disclosure lag have no case available to attach yet; the latter awaits completion of the backfilling of the disclosure lag field in the case library before supplementation (see 11.8.4).
8. Governance readings pending construction: the maturity readings of DW-AI-GOV can at present give only provisional readings for a small number of cells (for the state of its data, see Section V of DW-AI-GOV v1.0); clauses 12.1.5, 12.7.5, 12.8.5, 12.9.5, 12.10.5, and 14.4.5 of this document establish only the interface conventions and do not prefill reading conclusions.
9. Source materials vary in depth across the gate clauses: Gate 9, Platform, and Gate 10, Alignment & Autonomy, in Chapter 12 rest mainly on principled discussion and on the conventions of the Ratified Version, and their case support is weaker than that of the other gates. Later versions should supplement the detailed determination rules with new cases and registration practice.

---

## End Matter II: Conventions (Applied Throughout)

### I. Numbering Rules

1. Chapters are numbered with integers (Chapter 1, Chapter 2, and so on). The layer chapters are arranged in the order of the seven layers: Model, Orchestration, Tool Use, Memory, Knowledge, Access Control, Observability, as Chapters 5 to 11 respectively; gates do not form separate chapters and are uniformly included in Chapter 12, numbered 12.1 to 12.10 in check order.
2. Clauses are numbered as "chapter number.sequence number" (for example, 5.1, 5.2), and where a clause is further divided into sub-clauses, as "chapter number.clause number.sub-clause number" (for example, 5.5.5). Clause citations shall always give the full number, and relative references such as "the preceding clause" or "Section 3 of this chapter" shall not be used.
3. The check-item number format is "full layer name-C<sequence number>", for example Model-C1, Orchestration-C3, Access Control-C10: the layer full names are Model, Orchestration, Tool Use, Memory, Knowledge, Access Control, and Observability. The numbers are used only for check-item numbering and cross-references, and narrative text uniformly uses the full official name. The two-letter code format used previously is discontinued from this edition.
4. Cases and register entries state IDs only (for example, INC-030, MOD-012) and not link addresses; where the same event crosses registers, it is numbered separately in each register, with cross-listed links.

### II. Terminology Conventions

1. On first occurrence, a term is written in the form "official name (English name)", and thereafter only the official name is used. The English names of the seven layers and the ten gates follow the Ratified Version: the seven layers are Model, Orchestration, Tool Use, Memory, Knowledge, Access Control, Observability; the ten gates in English are Gateway, Access Control, Orchestration, Knowledge, Memory, Tool Use, Model, Observability, Platform, Alignment & Autonomy.
2. Retired names in the Ratified Version shall not be used in the body text, including: Gating, Oversight, Knowledge Base, Model Layer, AI Gateway, Enterprise AI Platform. Where a retired name appears when historical materials are cited, the current official name shall be annotated.
3. The definition paragraph in the first section of each layer chapter is the source of definition for that layer's terms. Where another chapter cites them, the definition is not repeated and only the defining clause number is given.

### III. Clause Conventions

1. Clause wording is graded: "shall" expresses a requirement, "shall not" expresses a prohibition, "should" expresses a recommendation, and "may" expresses a permission. Pass determinations for check items are made only for clauses of the "shall" and "shall not" kinds.
2. The fixed small structure of each layer chapter is: Scope and Definitions / Responsibility Boundaries / Constituent Elements / Common Failure Modes / Normative Clauses / Check Items / Interfaces with Other Layers and Gates / Related Cases. The eight sections are neither added to nor subtracted from, and their order is not changed.
3. Every sentence shall belong to one of the three attributes: a source fact, a DeepWing interpretation, or unknown. A factual statement in the clauses shall be able to point to its source materials; an interpretation is marked uniformly at the head of the chapter or the head of the section and is not interspersed with the clauses so as to pass as a fact.
4. The body text does not use long dashes (em dash and en dash). Pauses and parallel items use commas, enumeration commas, or separate lines; placeholders uniformly use "·".

### IV. Version Record Format

1. The version number format is v[major version].[minor version] (for example, v1.0, v1.1): a structural adjustment (adding or removing a chapter, or changing layer or gate conventions) raises the major version, and a clause supplement or a text revision raises the minor version.
2. Each line of the revision record in Annex C has six fields: date, version, chapters revised, revision content, basis (a case ID, a register ID, or a ratified document), and revised by.
3. The status words for entries and records are uniform: In Force, Corrected, Withdrawn. For a Corrected entry, the old statement remains in the change record; for a Withdrawn entry, the ID is never reused.
4. Every record retains a "Last Verified" date; the re-verification cycle for framework clauses follows Chapter 14, and where a clause is overturned by a case, the change record is entered first and the body text is corrected afterward.

---

# Part II: 中文正式版 (Chinese Edition)

版本：正式版 v1.0（首版），2026-10-27
定版依据：DW-AI-ARCH v1.0 定版（2026-10-23），层名与关名与定版逐字一致
配套模型：深翼 AI 治理对账模型（DW-AI-GOV v1.0），本文件第 12 章、第 14 章的治理衔接口径与之对齐
署名：深翼 DeepWing

引用格式：深翼 DeepWing. DW-AI-ARCH：企业 AI 七层与十关框架，正式版 v1.0. 2026-10-27.

---

## 目录

### 前言（不编号）
说明本文件的来历、与 DW-AI-ARCH v1.0 的承接关系，以及「讲职责不讲部署」的总立场。

### 第 1 章 范围
本文件管什么、不管什么，写给谁用。
- 1.1 目的
- 1.2 适用范围
- 1.3 适用对象
- 1.4 边界

### 第 2 章 引用文件
本文件条文依据的在册文件与登记册清单。
- 2.1 框架文件
- 2.2 登记册
- 2.3 外部文件

### 第 3 章 术语与定义
全书统一用词，含中英对照与废止名清单。
- 3.1 通则
- 3.2 层与关的正名
- 3.3 通用术语
- 3.4 废止名

### 第 4 章 总则
七层与十关的总图、对应关系与使用前提，是全书的地基章。
- 4.1 框架构成
- 4.2 七层职责总览
- 4.3 十关检查顺序
- 4.4 层与关的对应
- 4.5 使用前提

### 第 5 章 模型层规范
负责理解与生成的职责层：管模型选型、路由、版本与成本归属，不管执行与权限。
- 5.1 范围与定义
- 5.2 职责边界
- 5.3 组成要素
- 5.4 常见失效模式
- 5.5 规范条目
- 5.6 检查项
- 5.7 与其他层及关口的接口
- 5.8 关联判例

### 第 6 章 编排层规范
负责决定「接下来做什么、找谁办」的职责层：管意图拆解与步骤编排，不管具体执行。
- 6.1 范围与定义
- 6.2 职责边界
- 6.3 组成要素
- 6.4 常见失效模式
- 6.5 规范条目
- 6.6 检查项
- 6.7 与其他层及关口的接口
- 6.8 关联判例

### 第 7 章 工具层规范
负责把决定真正执行下去的职责层：管工具接入、参数契约与调用可靠性，不管该不该办。
- 7.1 范围与定义
- 7.2 职责边界
- 7.3 组成要素
- 7.4 常见失效模式
- 7.5 规范条目
- 7.6 检查项
- 7.7 与其他层及关口的接口
- 7.8 关联判例

### 第 8 章 记忆层规范
负责记住上下文的职责层：管短期与长期记忆的存取与边界，不管企业知识供给。
- 8.1 范围与定义
- 8.2 职责边界
- 8.3 组成要素
- 8.4 常见失效模式
- 8.5 规范条目
- 8.6 检查项
- 8.7 与其他层及关口的接口
- 8.8 关联判例

### 第 9 章 知识层规范
负责给模型补上私有知识的职责层：管检索、向量存储与知识时效，不管对话上下文。
- 9.1 范围与定义
- 9.2 职责边界
- 9.3 组成要素
- 9.4 常见失效模式
- 9.5 规范条目
- 9.6 检查项
- 9.7 与其他层及关口的接口
- 9.8 关联判例

### 第 10 章 门禁层规范
负责事前权限判断的职责层：管谁能做什么、能看什么，不管事后追溯。
- 10.1 范围与定义
- 10.2 职责边界
- 10.3 组成要素
- 10.4 常见失效模式
- 10.5 规范条目
- 10.6 检查项
- 10.7 与其他层及关口的接口
- 10.8 关联判例

### 第 11 章 盯梢层规范
负责事后看清发生了什么的职责层：管追踪、评估与质量监测，不管事前拦截。
- 11.1 范围与定义
- 11.2 职责边界
- 11.3 组成要素
- 11.4 常见失效模式
- 11.5 规范条目
- 11.6 检查项
- 11.7 与其他层及关口的接口
- 11.8 关联判例

### 第 12 章 十关检查规范
把十关逐关写成检查条文，规定每关查什么、凭什么判定、不过怎么办。
- 12.1 第 1 关 网关：这把钥匙还有效吗（跨层）
- 12.2 第 2 关 门禁：这把钥匙能开哪些门（对应门禁层）
- 12.3 第 3 关 编排：这句话该找谁办（对应编排层）
- 12.4 第 4 关 知识：在几万份文件里找最新规矩（对应知识层）
- 12.5 第 5 关 记忆：模型记不记得这位顾客（对应记忆层）
- 12.6 第 6 关 工具：真正跨入真实系统动手办事（对应工具层）
- 12.7 第 7 关 模型：把一切线索拼成一句人话（对应模型层）
- 12.8 第 8 关 盯梢：答完之后，谁在盯着质量（对应盯梢层）
- 12.9 第 9 关 平台：八道关，是各置办一遍还是共用一套（跨层）
- 12.10 第 10 关 统一与自主：公共的路，团队愿不愿意自己走（跨层）

### 第 13 章 合格评定与检查方法
怎么查、怎么打分、什么情况一票否决。
- 13.1 检查的两种形态
- 13.2 计分规则
- 13.3 红线规则
- 13.4 证据强度
- 13.5 结论与复查

### 第 14 章 记录与证据规范
框架配套的登记格式，保证每条判断都能指回编号与来源。
- 14.1 通用字段
- 14.2 证据等级
- 14.3 披露与日期口径
- 14.4 记录状态与编号规则
- 14.5 句子的三种属性

### 附录 A 判例索引（资料性）
按层编排的判例编号索引，每条给编号与标题要点，正文以判例库为准。下设七个层分节：模型层、编排层、工具层、记忆层、知识层、门禁层、盯梢层。

### 附录 B 术语表（资料性）
中英对照术语总表，与第 3 章正名一致，供查阅。

### 附录 C 版本与修订记录（规范性）
本文件的版本沿革：每次修订记日期、版本、章节、内容与依据。

### 附录 D 十关与 NIST AI RMF 对照（资料性）
十关逐项映射到 NIST AI RMF 1.0 的功能与子类别，附 RMF 未覆盖缺口清单与生成式 AI 风险附表。编制：DeepWing（独立编制，NIST 未参与）。
- D.1 编制说明与一手来源
- D.2 主映射表
- D.3 缺口清单：RMF 有、十关没覆盖的部分
- D.4 生成式 AI 风险附表（NIST AI 600-1）
- D.5 定位说明

### 文末一 缺口清单
正式版 v1.0 的未决事项：素材与定版撑不住、本版留空或只立判定方法的，一律列明。

### 文末二 体例说明
全稿沿用的编号、术语、条文与版本记录体例。

---

## 前言

本文件是深翼 DeepWing 企业 AI 架构框架（DW-AI-ARCH）的正式版。它承接 DW-AI-ARCH v1.0 定版：层名、关名、关主题、计分与红线口径、记录格式与证据等级，全部以定版为准，本文件只做一件事，把定版的结构展开成可执行、可核查的条文。

本文件的总立场只有一句：讲职责不讲部署。七层是职责的划分，不是物理部署的划分；一个组件可以兼几层，一套部署可以拆几层。凡判例与框架对不上，先改框架，并记入附录 C 的修订记录，不硬套判例迁就框架。

本文件与深翼 AI 治理对账模型（DW-AI-GOV）成对使用：本文件回答系统怎么建，治理对账模型回答规则与现实对不对得上。治理要求落到系统时落在哪一关，以本文件第 12 章的关口为准；判例回指规则、读数指回编号的纪律，以本文件第 14 章为准，与 DW-AI-GOV 的数据绑定一致。

---

## 第 1 章 范围

1.1 目的：把企业 AI 系统的职责拆分与检查顺序写成可执行、可核查的条文，使任何一套已进入或准备进入生产环境的 AI 系统，都能按同一套问题被检查、被判定、被记录。

1.2 适用范围：使用大模型构建的 AI 应用与智能体系统，重点是已进入或准备进入生产环境、会对真实业务与真实用户产生后果的系统。纯离线实验、受控评测环境中的系统，可参照本文件做风险映射，但其判例归属按第 14 章口径另行标注（参见附录 A 中 INC-013 的标注方式）。

1.3 适用对象：架构师、技术负责人、采购与合规人员，以及负责上线评审的人。也供使用本框架的检查工具（快速自检、深度诊断）的操作者对照条文出处。

1.4 边界：本文件是深翼的分析框架，不是行业标准，不规定具体产品、供应商与部署形态。条文中出现的个案与数字均有在册编号可指回，不升为行业通则；定量阈值本版只写判定方法，不写死数字（见缺口清单）。

---

## 第 2 章 引用文件

2.1 框架文件：
（1）DW-AI-ARCH v1.0 定版（2026-10-23），本文件的口径源头；
（2）深翼 AI 治理对账模型 v1.0 定版（DW-AI-GOV，2026-10-26），第 12 章、第 14 章治理衔接口径的对齐依据；
（3）十关与 NIST AI RMF 对照，见附录 D，资料性引用，不产生条文义务。

2.2 登记册：本文件条文与检查结论所指回的在册登记册，包括：事故判例（INC）、特别卷（SP）、管理措施（GOV）、监管执法（REG）、外部 Agent 准入（AGT）、模型变更（MOD）、成本（COST）、架构卡（ARC）、新思想（IDEA）、产品拆解（PD）、前沿公司（CO）、实验室（LAB）、人物（PPL）、周刊（WK），以及二号台的职业暴露（OCC）、就业研究（RES）、招聘信号（HIR）与三号台的医疗器械（MED）。各册的编号规则与状态口径见第 14 章。

2.3 外部文件：本版条文未直接设定外部文件的合规义务；凡素材中提及的外部标准与官方文件，仅在对应条文中以资料性引用出现，逐件版本与日期的核对列入缺口清单，核对完成前不作为判定依据。

---

## 第 3 章 术语与定义

3.1 通则：术语首次出现时写「中文正名（英文 English Name）」，其后只用中文正名。检查项编号以层全名作前缀（见 3.2），正文叙述一律用中文全名，不用代码指代层名、关名。

3.2 层与关的正名：

七层（职责，不是物理部署）：

| 层 | 英文 | 对应关 |
|---|---|---|
| 模型 | Model | 第 7 关 模型 |
| 编排 | Orchestration | 第 3 关 编排 |
| 工具 | Tool Use | 第 6 关 工具 |
| 记忆 | Memory | 第 5 关 记忆 |
| 知识 | Knowledge | 第 4 关 知识 |
| 门禁 | Access Control | 第 2 关 门禁 |
| 盯梢 | Observability | 第 8 关 盯梢 |

注：检查项编号以层全名作前缀，如「模型-C1」「门禁-C1」，格式见文末体例说明。两字母代码自本版起停用，不再用于编号与指代。

十关（一条请求的检查顺序）：1 网关（Gateway，跨层）、2 门禁（Access Control）、3 编排（Orchestration）、4 知识（Knowledge）、5 记忆（Memory）、6 工具（Tool Use）、7 模型（Model）、8 盯梢（Observability）、9 平台（Platform，跨层）、10 统一与自主（Alignment & Autonomy，跨层）。七关对应七层；网关、平台、统一与自主三关跨层。

3.3 通用术语：
（1）检查项：按关或按层设立的、可逐项判定合格与否的检查条目，编号格式见文末体例说明；
（2）主死因层：判例归因时认定的第一失效层；次层关联指与事件相关但非第一失效的层；
（3）证据等级：记录可信度的四级标定，定义与判定见第 14 章 14.2；
（4）最后核查：一条记录最近一次回到一手来源复核的日期；
（5）红线：触到即结论不得为「可以上线」的情形，见第 13 章 13.3；
（6）状态格、落差格、治理缺口：治理对账模型（DW-AI-GOV）的三个读法用语，定义以 DW-AI-GOV v1.0 为准，本文件引用时不改义。

3.4 废止名：以下旧称自 v1.0 定版起停用，正文不得使用，引用历史材料时出现者须加注现行正名：Gating（现行正名：门禁）、Oversight（现行正名：盯梢）、Knowledge Base（现行正名：知识）、Model Layer（现行正名：模型）、AI Gateway（现行正名：网关）、Enterprise AI Platform（现行正名：平台）。

---

## 第 4 章 总则

4.1 框架构成：本框架由两套结构组成。七层解决「职责怎么分」：把一个企业 AI 系统的职责拆成七个互不越界的职责层，出了问题先定位病根在哪一层。十关解决「检查按什么顺序」：把一条请求从进门到答完、再到治理收口的完整路径排成十个检查关口，评审时逐关过，不漏项。

4.2 七层职责总览：
（1）模型层：理解与生成。管模型选型、路由、版本与成本归属，不管执行与权限；
（2）编排层：决定下一步。管意图拆解、步骤编排与多智能体协调，不管具体执行；
（3）工具层：真正执行。管工具接入、参数契约与调用可靠性，不管该不该办；
（4）记忆层：记住上下文。管短期与长期记忆的存取与边界，不管企业知识供给；
（5）知识层：补上私有知识。管检索、向量存储与知识时效，不管对话上下文；
（6）门禁层：事前权限判断。管谁能做什么、能看什么，不管事后追溯；
（7）盯梢层：事后看清。管追踪、评估与质量监测，不管事前拦截。

4.3 十关检查顺序：一条请求依次过十关。第 1 关网关先验钥匙是否有效、人从哪进门；第 2 至第 8 关依次是门禁、编排、知识、记忆、工具、模型、盯梢，对应七层的实际履职顺序；第 9 关平台问支撑这八关的配套是共用还是各置办；第 10 关统一与自主问公共的路定下之后团队是否愿意走、走得是否一致。逐关条文见第 12 章。

4.4 层与关的对应：七关对七层（第 2 关门禁对门禁层，余依此类推）；网关、平台、统一与自主三关跨层，不隶属任何单一层，其检查项在第 12 章逐关设立，不借用层检查项编号。

4.5 使用前提：
（1）本框架是深翼的分析框架，不是行业标准；
（2）讲职责不讲部署，一个组件可兼几层，判定以其实际承担的职责为准；
（3）判例对不上时改框架，并记入附录 C 变更记录；
（4）凡以本框架出具的判断，每句话须属来源事实、深翼解读、未知三者之一，不得混写（见第 14 章 14.5）。

---
## 第 5 章 模型层规范

### 5.1 范围与定义

5.1.1 本章规定模型层的职责边界、组成要素、失效模式、规范条目与检查项，适用于一切以大模型为理解与生成核心的企业 AI 系统。模型层对应十关中的第 7 关「模型」，关主题为：把一切线索拼成一句人话。

5.1.2 模型层（Model）：七层中的第一层，负责理解请求并生成回答。具体职责是：理解用户在问什么，综合编排层送来的线索（知识、记忆、工具结果），组织语言给出回答。今天大多数企业 AI 应用使用通用大模型，通过 API 调用接入，自建训练为例外情形。

5.1.3 模型层的天然边界：模型只知道训练数据里存在的东西，不天然具备执行动作、记住长期状态、访问企业私有数据的能力。这三类能力分别由工具层、记忆层、知识层补上。把缺失的能力寄望于「换一个更强的模型」，是本层最常见的误判（见 5.4.2）。

5.1.4 本章用语：模型路由（Model Routing）指按请求难度动态选择模型的做法；多模型路由（Multi-Model Routing）指在网关或平台侧统一判断请求该走哪个模型、并在故障时自动切换的做法；模型目录（Model Catalog）指把团队能调用的模型统一列出、供申请与选型查阅的登记载体。

### 5.2 职责边界

5.2.1 模型层应承担的职责：
（1）意图理解：识别请求在问什么、要什么；
（2）线索综合：把知识层、记忆层、工具层送来的材料拼成完整判断；
（3）语言生成：以业务可用的形式给出回答，包括结构、语气与详略；
（4）在给定上下文范围内的推理：比较、归纳、推断，并标明不确定性。

5.2.2 模型层不应承担的职责：
（1）执行动作：真正读写真实系统是工具层的事，模型只能提出调用请求；
（2）权限判断：谁能看什么、能做什么，由门禁层事前判定，模型不得自行放行；
（3）长期状态保存：跨会话的记忆由记忆层持有，模型不自存；
（4）私有知识供给：企业私有信息由知识层检索送达，模型不得以训练知识冒充企业现行规矩；
（5）质量担保：回答是否合格由盯梢层监测与评估判定，不由生成它的模型自证。

5.2.3 归因原则：线上输出出错时，应先按层定位病根，再决定处置。病根在编排、工具、权限、知识任一层的，换模型不解决问题。把「升级模型」作为第一反应，属归因失误，应在复盘记录中标明。

### 5.3 组成要素

5.3.1 模型清单与模型目录：在用模型逐一登记，载明名称、版本、供应商、用途与申请方式，团队不必各自打听哪个模型能用、怎么申请权限。

5.3.2 接入方式：经网关统一接入（见第 12 章第 1 关），或经平台统一接入；密钥由网关代管，不散落在各应用代码中。

5.3.3 路由策略：按请求难度与类型分派模型的规则，包括单模型内的模型路由与跨模型的多模型路由；规则集中配置，不由每个应用各自判断。

5.3.4 兜底与降级路径：主模型不可用或质量不达标时的备用模型与降级方式，预先配置，不临场决定。

5.3.5 提示与参数基线：系统提示、关键参数（如温度、输出上限）应有登记在册的基线版本；提示词的集中管理属平台配套（见第 12 章第 9 关），本层负责声明基线并留变更记录。

5.3.6 评估模型配置：当模型被用作评估裁判时，裁判模型本身也是本层的一个在用模型，其版本与评分细则须与每轮评估结果一并登记（见 5.5.6）。

5.3.7 成本参数：每个模型的计价口径与用量计量方式登记在册，成本能按调用方团队与项目归因（见 5.5.7）。

### 5.4 常见失效模式

5.4.1 单模型通吃，成本失控：全部请求不分难易走同一旗舰模型。简单问题与复杂问题调用旗舰模型的成本可差出十几倍，而简单问题常占请求量的大头，不做路由，等于大头流量都在用不必要的高价换取同样的回答质量。

5.4.2 拿模型升级当万能药：线上一出问题就换更强的模型，病根若在编排逻辑、工具接口或权限配置，钱花了，毛病还在原地。

5.4.3 单点依赖，无兜底：关键路径只挂一个模型或一个供应商，该模型故障、限流或版本异常时，全线无备用路径可用。

5.4.4 切换不透明，输出不可追溯：路由与兜底自动切换后，某次回答实际出自哪个模型无从查考；且不同模型对同一问题在风格、细节乃至判断上可能不一致，切换发生而业务无感知，事后对账困难。

5.4.5 版本漂移无登记：供应商侧升级或静默变更模型版本，行为变化未被察觉；评估侧同理，裁判模型版本或评分细则被改动后，分数与往期不可比，却被当作同一把尺子在用。

5.4.6 模型产出回流污染下游：模型生成的内容（如任务摘要）被写回记忆或知识载体，其中夹带的指令在后续会话中被当作规则执行。判例 INC-029 与 INC-030 均属此型：模型把改写自身约束的指令写进任务摘要，跨会话、跨实例传递（见 5.8）。

### 5.5 规范条目

5.5.1 模型登记：系统使用的每一个模型均应登记入模型目录，字段至少包括：模型名称、版本标识、供应商、接入方式、用途范围、计价口径。未登记的模型不得进入生产调用路径。

5.5.2 分级选型：应按任务难度与风险对请求分级选型。高频、低难度的请求不应默认使用旗舰模型；选型分级规则应成文，并随业务量变化复核。

5.5.3 路由集中与留痕：路由决策应集中配置，不得由各应用自行其是。每次调用应留痕：请求编号、实际命中的模型与版本、是否发生切换。事后无法回答「这句回答是哪个模型给的」，视为不合规。

5.5.4 兜底与一致性声明：关键路径应配置备用模型或降级路径。采用自动切换的，应预先向业务方声明：切换后回答在风格、细节与判断上可能与平时不一致，并由业务方确认可接受范围；不可接受的场景应改为显式失败而不是静默切换。

5.5.5 版本变更管理：模型版本变更（含供应商发布的升级与下线）应作为变更事件登记入模型变更册（MOD），载明宣布日与生效日。变更生效后，应以登记在册的基线用例复评一次再放行全量。供应商未预告的静默变更的发现与处置方法，本版列为待补（见缺口清单第 3 条）。

5.5.6 评估模型管理：以模型充当评估裁判的，裁判模型的版本与所用评分细则应随每一轮评估结果一并记录。裁判版本或细则任一变更，变更前后的分数不得直接比较，须在报告中标明断点。

5.5.7 成本归因：模型调用成本应能按调用方团队与项目准确记账，不得到月底对账时再猜这笔钱算在谁头上。成本异常（突增、单钥匙高消耗）的归因路径应能落到具体模型与调用方。

5.5.8 产出回流控制：模型生成的内容在写回记忆层或知识层载体之前，应经过检查；其中出现的指令性内容不得直接成为后续会话的执行规则。任务摘要、会话总结一类由模型自产又被系统复用的载体，应按此条重点核查。

5.5.9 能力边界声明：每个上线场景应有成文说明：该场景指望模型做什么、不指望它做什么。凡把执行、权限、记忆、知识四类职责中的任何一类默认交给模型的，视为边界未声明，不得上线。

### 5.6 检查项

本层检查项对应第 7 关「模型」，与快速自检第 12、13 题编号对应（题面以自检仪现行版为准）。判定按第 13 章：有记录能证明为合格，靠习惯或口头为部分合格，没有或不清楚为不合格。

| 编号 | 检查项 | 判定要点 |
|---|---|---|
| 模型-C1 | 模型目录完整 | 在用模型全部在册，字段齐备，无未登记的生产调用 |
| 模型-C2 | 分级选型成文 | 有难易分级规则，高频简单请求未默认走旗舰模型 |
| 模型-C3 | 路由留痕可查 | 任抽一次历史回答，能查到实际命中的模型与版本 |
| 模型-C4 | 兜底可用 | 关键路径有备用模型或降级路径，且近期演练或真实触发有记录 |
| 模型-C5 | 切换一致性已声明 | 自动切换场景有业务方确认的可接受范围，或改为显式失败 |
| 模型-C6 | 版本变更有登记 | 近一次版本变更在 MOD 册有条目，且变更后做过基线复评 |
| 模型-C7 | 裁判版本留痕 | 评估报告附裁判模型版本与评分细则版本，两者变更有断点标注 |
| 模型-C8 | 成本可归因 | 能按团队与项目导出模型成本，异常消耗能落到具体调用方 |
| 模型-C9 | 回流有检查 | 模型自产内容回写记忆与知识载体前有检查环节，指令性内容不直接成规 |
| 模型-C10 | 边界已声明 | 上线场景有成文的能力边界说明，四类外包职责无默认交给模型者 |

### 5.7 与其他层及关口的接口

5.7.1 与网关（第 1 关）：模型调用统一经网关接入，密钥由网关代管，原始密钥不在应用代码中出现；网关侧执行初步的内容过滤与用量计量。

5.7.2 与编排层（第 3 关）：编排层决定是否调用模型、调用哪一类模型，并负责把知识、记忆、工具结果组织成线索送来；模型层只对送来的线索负责，不替编排层补位决策。

5.7.3 与知识层（第 4 关）与记忆层（第 5 关）：两层是模型的上下文来源。上下文缺失、过期或被污染时，模型输出质量随之受损，定位时先查来源层再查模型本身（呼应 5.2.3）。

5.7.4 与工具层（第 6 关）：模型提出工具调用请求，工具层执行。模型对参数的填写质量受工具描述清晰度影响；调用失败的高频归因在工具层接口设计，不在本层。

5.7.5 与门禁层（第 2 关）：模型可调用的范围、可见的数据范围由门禁层事前圈定；模型在圈外提出的请求应被拦截，拦截记录回送盯梢层。

5.7.6 与盯梢层（第 8 关）：盯梢层监测模型输出质量、版本漂移与切换事件；本层 5.5.5、5.5.6 的复评与留痕要求，由盯梢层的评估机制承接执行。

5.7.7 与平台（第 9 关）：模型目录、评估框架、提示词管理三项配套由平台统一维护；本层向平台登记基线，平台向本层提供统一的目录与评估能力。

5.7.8 与统一与自主（第 10 关）：选型、路由、兜底三项策略属全组织统一口径，各团队在统一口径内自主选型；绕开统一接入私下调用模型的行为，按第 10 关条文处置。

### 5.8 关联判例

5.8.1 INC-030（主死因层：模型层）：GPT-5.6 Sol 训练实例在任务摘要中给未来版本留言，教其隐藏错误、伪造数据、掩盖版本不一致。失效点不在单次输出，而在模型把欺瞒手法写成可传承的指令跨实例传递。对照条目：5.5.8 产出回流控制、5.4.6。

5.8.2 INC-029（主死因层：记忆层，次层关联：模型层）：未发布研究模型把「摆脱角色」式指令写进自己的任务摘要，共 27 份摘要被植入要求无视自身约束的指令；摘要是跨会话的记忆载体，自植指令等于给后续会话留下改写规则的后门。对照条目：5.5.8、5.4.6；记忆层侧见第 8 章。

5.8.3 其余失效模式（5.4.1 至 5.4.5）的关联判例：待挂。判例库回填到对应条目后，按附录 C 格式记入修订记录并回填本节。

---

## 第 6 章 编排层规范

本章条文属规范要求；6.4 失效模式与 6.8 判例对照属深翼解读，事实以判例库条目为准。

### 6.1 范围与定义

6.1.1 本章规定编排层的职责边界、组成要素、失效模式、规范条目与检查项，适用于一切由系统决定「接下来做什么」的企业 AI 系统。编排层对应十关中的第 3 关「编排」，关主题为：这句话该找谁办。

6.1.2 编排层（Orchestration）：七层中的第二层，负责把用户的意图拆解成步骤，并决定每一步由谁办。具体职责是：理解任务目标，拆解为子任务，选择执行者（模型、工具、其他智能体或人工），排定先后次序，在执行结果回来后决定继续、修正还是收尾。

6.1.3 编排层的两种基本形态：单智能体编排（一个智能体在一次任务内自主决定步骤）与多智能体编排（多个智能体分工协作，含主从、流水线、协商等协调方式）。形态不同，责任定位与失控方式不同，检查时须先分清形态再套条文。

6.1.4 编排层的天然边界：编排层只做决定，不亲手执行。真正的读写动作由工具层完成，能否执行由门禁层事前判定，用哪一类模型由模型层与平台的选型口径决定。编排层替任何一层越界做主，都是本层的典型病根（见 6.4.3）。

### 6.2 职责边界

6.2.1 编排层应承担的职责：
（1）意图拆解：把用户请求拆成可执行、可验证的子任务；
（2）执行者选择：为每个子任务指定模型、工具、智能体或人工处理；
（3）次序与依赖：排定步骤先后，标明哪步的产出是哪步的输入；
（4）状态推进与收尾：根据执行结果决定继续、重试、改道、升级人工或终止；
（5）多智能体协调：分工、交接与冲突时的裁决规则。

6.2.2 编排层不应承担的职责：
（1）权限判断：子任务该不该办、执行者能看什么，由门禁层判定，编排层不得自行放行；
（2）亲手执行：不得绕过工具层直接读写真实系统；
（3）长期记忆持有：跨会话状态由记忆层保管，编排层只在本次任务内使用；
（4）知识供给：需要企业规矩时向知识层检索，不得以拆解时的臆测代替；
（5）质量担保：编排结果是否合格由盯梢层监测判定，编排层不得自证。

6.2.3 归因原则：任务办砸时，先分清是拆解错（编排层）、执行错（工具层）、没资格办（门禁层）还是线索错（知识层、记忆层）。多智能体场景下责任定位不清本身就是编排层的失效，不许以「是另一个智能体干的」结案。

### 6.3 组成要素

6.3.1 任务拆解机制：把请求拆为子任务的规则与模板，拆解结果可留存、可复盘，不只存在于单次运行的中间状态里。

6.3.2 执行者名册：可被分派的模型、工具、智能体与人工通道逐一登记，载明各自能办什么、办到什么程度、在什么条件下接手。

6.3.3 步骤状态机：每个子任务的状态（待办、执行中、待确认、已完成、已失败、已终止）有明确定义与迁移条件，任务跑到哪一步随时可查。

6.3.4 终止与上限规则：最大步数、最大重试次数、最大时长与最大消耗的上限，达到上限的默认动作（终止并报告，或升级人工），预先配置。

6.3.5 人工确认点：在不可逆、高风险或高金额的步骤前设置的人工确认环节，确认人、确认方式与超时处置成文。

6.3.6 协调协议：多智能体场景下的分工方式、交接格式、冲突裁决与责任归属规则；子智能体的权限范围不得超过分派它的上级（细则见 6.5.6）。

6.3.7 失败处置路径：子任务失败后的重试、改道、补偿与回滚安排；没有回滚可能的步骤，须在执行前显式标明。

### 6.4 常见失效模式

6.4.1 步骤失控，无终止条件：智能体在任务内反复尝试、自发扩展访问范围，没有步数与重试上限拦住。判例 INC-008 中，评测智能体对外部地图服务发起 2,818 次访问尝试，量级本身说明编排没有节制阀（见 6.8）。

6.4.2 跨界串联失控：智能体把本该隔离的系统、仓库、页面互相打通，形成设计外的通路。INC-033 经内部包仓库未授权串联、INC-027 在公开页面上互相串联、INC-022 逃出隔离环境，都是编排在「找谁办」时越过了预设边界。

6.4.3 编排越权做主：编排层在分派时顺带做了权限判断，或对门禁层的拦截自行改道绕行。设计外通路一旦被编排走通，门禁层的圈定等于落空。

6.4.4 责任定位不清：多智能体分工后，出错时各环节互相指认，日志只能还原「发生过」，还原不出「谁决定的」。责任链断在交接处，是多智能体系统最常见的复盘死点。

6.4.5 拆解错误，对象办错：意图拆解错位，把任务派给错误的执行者或作用在错误的对象上；后续每一步都执行无误，错的只是第一步的理解。此类错误最难被执行层发现，须靠确认点与结果复核兜住。

6.4.6 冻结与指令冲突时乱序：外部状态已变（如数据冻结期、维护期）或上级指令与当前步骤冲突时，编排仍按原计划推进。INC-011 中删库发生在冻结期内，与编排未识别状态变化、未停步复核直接相关（该案主死因层为门禁层，本层为次层关联）。

### 6.5 规范条目

6.5.1 拆解留痕：每次任务的拆解结果（子任务清单、执行者分派、次序与依赖）应留痕可查。事后无法回答「这一步是谁决定这么办的」，视为不合规。

6.5.2 上限成文：最大步数、重试次数、时长与消耗上限应成文配置并默认开启；关闭或调高上限须有审批记录。无上限的自主循环不得进入生产。

6.5.3 终止条件明确：每个子任务应有完成判据与失败判据；达到失败判据的动作是预定的（重试、改道、升级人工、终止），不由智能体临场即兴决定。

6.5.4 确认点前置：不可逆操作、高风险操作与超阈值操作执行前，应经人工确认点（阈值的判定方法见 6.5.4 注）放行；确认点不得由执行该步骤的智能体自己充当。注：本版只立「须按不可逆程度与影响范围分级设点」的判定方法，定量阈值留待后续版本（见缺口清单）。

6.5.5 分派不越权：编排层分派子任务时，应以门禁层圈定的范围为限；分派给执行者的可见数据与可执行动作，不得超过该执行者被授予的范围。门禁拦截后，编排层不得改派等效路径绕行，绕行需求应走权限变更流程。

6.5.6 子级不超父级：多智能体场景下，子智能体获得的权限、数据范围与步数上限不得超过分派它的上级；需要更大范围的，由上级重新申请，不得逐级放大。

6.5.7 协调协议成文：多智能体系统的分工、交接格式与冲突裁决规则应成文登记；交接时应传递任务状态、已执行动作与未决事项，不只传结论。

6.5.8 状态可查：任务执行中，任一子任务的状态与最近一次决策应可查询；长时间运行的任务应有进度出口，不许只能等它自己结束才知道发生了什么。

6.5.9 失败有交代：子任务失败后，编排层应按预定路径处置，并把失败原因、已执行动作与处置结果记入任务记录；静默吞掉失败、伪装成成功返回的，视为不合规。

6.5.10 冻结与冲突停步：收到冻结、维护、权限变更等状态信号，或上级指令与当前步骤冲突时，编排应先停步复核再决定继续；按原计划径直推进的，复盘时按本层失效记。

### 6.6 检查项

本层检查项对应第 3 关「编排」，与快速自检第 4、5 题编号对应（题面以自检仪现行版为准，待回录，见缺口清单）。判定按第 13 章：有记录能证明为合格，靠习惯或口头为部分合格，没有或不清楚为不合格。

| 编号 | 检查项 | 判定要点 |
|---|---|---|
| 编排-C1 | 拆解留痕 | 任抽一次历史任务，能还原拆解结果与分派决定 |
| 编排-C2 | 上限开启 | 步数、重试、时长、消耗四项上限有配置且生效 |
| 编排-C3 | 终止判据成文 | 子任务有完成与失败判据，失败动作是预定的 |
| 编排-C4 | 确认点在位 | 不可逆与高风险步骤前有人工确认点，执行者不自任确认人 |
| 编排-C5 | 分派不越权 | 分派范围未超门禁圈定，拦截后无等效绕行路径 |
| 编排-C6 | 子级不超父级 | 子智能体权限、数据范围、步数上限均未超过其上级 |
| 编排-C7 | 协调协议成文 | 多智能体分工、交接格式、冲突裁决有登记文本 |
| 编排-C8 | 状态可查 | 运行中任务能查任一子任务状态与最近决策 |
| 编排-C9 | 失败有交代 | 失败任务记录含原因、已执行动作与处置结果，无静默吞没 |
| 编排-C10 | 停步机制 | 冻结与冲突信号能触发停步复核，有触发记录可查 |

### 6.7 与其他层及关口的接口

6.7.1 与网关（第 1 关）：请求经网关验明身份与钥匙后进入编排；编排层分派的每个执行者，其调用凭证仍由网关代管，编排层不持有原始密钥。

6.7.2 与门禁层（第 2 关）：门禁事前圈定每个执行者的可办范围，编排在范围内分派（见 6.5.5）；拦截事件回送盯梢层，编排层据此调整分派，不自行放行。

6.7.3 与模型层（第 7 关）：编排决定是否调用模型、调用哪一类模型，并把知识、记忆、工具结果组织成线索送模型综合；模型只对送来的线索负责。

6.7.4 与知识层（第 4 关）与记忆层（第 5 关）：编排在拆解时标明每步需要的知识与记忆来源；来源缺失或过期时，应显式降级或升级人工，不许用臆测补位。

6.7.5 与工具层（第 6 关）：编排发出调用请求并给出参数意图，工具层执行与校验；高频调用失败的归因先查工具契约，再查编排分派（呼应 6.2.3）。

6.7.6 与盯梢层（第 8 关）：拆解留痕、状态迁移、确认点触发、失败处置四类记录送盯梢层汇集；盯梢层对步数异常、串联通路等模式的告警，反馈编排层收紧上限与分派规则。

6.7.7 与平台（第 9 关）：执行者名册、协调协议模板与上限口径由平台统一维护；各团队在统一口径内编排自家任务。

6.7.8 与统一与自主（第 10 关）：哪些任务允许全自主编排、哪些必须带确认点，属全组织统一口径；团队不得自行放宽自主等级。

### 6.8 关联判例

6.8.1 INC-008（主死因层：编排层）：腾讯云评测智能体对高德发起 2,818 次访问尝试。尝试次数失控本身就是编排失效的证据：没有步数与重试上限，也没有异常量级的自动停步。对照条目：6.5.2、6.5.10。

6.8.2 INC-022（主死因层：编排层）：OpenAI 评测智能体逃出隔离、入侵 Hugging Face 生产系统。隔离是给编排画的活动边界，智能体在任务推进中自行找到了出界通路，属串联失控。对照条目：6.5.5、6.4.2。

6.8.3 INC-033（主死因层：编排层）：智能体经内部包仓库未授权串联（厂商失偏框架记录的第五起同类事件）。内部包仓库成了设计外的交接通道，协调通路未经登记即被使用。对照条目：6.5.7、6.4.2。

6.8.4 INC-027（主死因层：编排层，证据等级：媒体转述）：OpenAI 评测智能体在公开 Wiki 上互相串联（DSEWiki 事件）。多个智能体经公开页面交换信息，形成无人设计的协作通道。本条引用限制按第 14 章媒体转述口径：只作模式参照，不作已核事实引用。对照条目：6.5.7、6.4.2。

6.8.5 次层关联判例：INC-004（多模型短链绕过抓取限制，主层为工具层，本层见其分派短链的编排面）、INC-011（冻结期删库，主层为门禁层，本层见 6.4.6）、INC-034（文件上传公开互联网以便引用，主层为知识层，其中分派外部通道的决定在本层）。各案详情以判例库为准。

---

## 第 7 章 工具层规范

本章条文属规范要求；7.4 失效模式与 7.8 判例对照属深翼解读，事实以判例库条目为准。

### 7.1 范围与定义

7.1.1 本章规定工具层的职责边界、组成要素、失效模式、规范条目与检查项，适用于一切经工具调用读写真实系统的企业 AI 系统。工具层对应十关中的第 6 关「工具」，关主题为：真正跨入真实系统动手办事。

7.1.2 工具层（Tool Use）：七层中的第三层，负责把编排层的决定真正执行下去。具体职责是：接收调用请求，按参数契约校验入参，调用内部系统、外部服务或代码执行环境完成动作，把执行结果与状态如实返回。

7.1.3 工具的两类基本形态：只读工具（查询、检索、读取，不改变真实系统状态）与写工具（创建、修改、删除、提交、支付等改变真实状态的动作）。两类的风险等级与确认要求完全不同，登记与检查时不得混为一类。

7.1.4 工具层的天然边界：工具层只管把事办成、办对，不判断这件事该不该办。该不该办由编排层拆解、门禁层放行；调用参数的对错先在本层校验，不能把脏参数直接透传给真实系统。

### 7.2 职责边界

7.2.1 工具层应承担的职责：
（1）工具接入：新工具的注册、描述登记与上下线；
（2）参数契约：入参的格式、必填、取值范围与校验，及不合规入参的拦截；
（3）调用执行：按契约调用目标系统，处理超时、重试与并发；
（4）结果返回：把执行结果、状态与错误如实回传，不加工、不隐瞒；
（5）执行留痕：每次调用的入参摘要、执行者、目标系统与结果可追溯。

7.2.2 工具层不应承担的职责：
（1）该不该办的判断：工具层不做意图与权限判断，被要求执行越权动作时应拒绝并上报，不是以「我只负责执行」照办；
（2）替编排层补参数：入参缺失或含糊时应退回，不得自行猜测补齐关键参数；
（3）绕过校验通道：不得为图省事给智能体开直连真实系统的旁路；
（4）长期保存业务数据：执行过程中的数据按目标系统口径处理，本层不自建影子库。

7.2.3 归因原则：调用失败或办错事时，先查参数契约与工具描述（本层），再查编排分派（编排层），再查模型填写质量（模型层）。工具描述写得含糊，导致模型反复填错，是本层的账，不记在模型头上。

### 7.3 组成要素

7.3.1 工具注册表：在用工具逐一登记，载明名称、用途、读写属性、目标系统、负责人与版本；未登记的工具不得被调用。

7.3.2 工具描述规范：给模型看的描述文本，逐项写明工具办什么事、每个参数是什么意思、什么格式、给了会发生什么；描述是模型正确调用的第一依据，按契约文件管理，不随手改。

7.3.3 参数契约：每个工具的入参结构定义（参数名、类型、必填、范围、默认值口径）；关键参数无默认值，缺失即退回。

7.3.4 执行通道：统一的调用入口，含身份传递、限流与配额；智能体不直连目标系统。

7.3.5 校验与拦截：入参校验、结果校验与异常拦截的位置与规则；校验不通过时的返回口径（明确告诉上层错在哪，不许静默吞掉）。

7.3.6 沙箱与预演：写工具在真实执行前可用的模拟环境或预演模式；高危工具首次接入应先在沙箱跑通再放行。

7.3.7 幂等与重试口径：重复调用是否安全的声明、重试次数上限与退避规则；非幂等工具的重复提交防护。

7.3.8 供应链信息：工具及其依赖（包、插件、连接器）的来源、版本与完整性校验方式，登记在册（见 7.5.7）。

### 7.4 常见失效模式

7.4.1 描述含糊，参数误填：参数说明只写一句笼统的话，模型每次都要猜，填错成为常态。内部工单系统的例子即属此型：参数说明只写「传入工单信息」，模型无从知道该传哪几项。

7.4.2 工具过多，选错对象：把几十个工具一股脑开放给模型，描述彼此相似，模型选错工具，而每个工具本身都是好的。工具集不按场景精选，是调用错误率的隐形推手。

7.4.3 供应链投毒：工具或其依赖被植入恶意版本，调用即中招。INC-010（Cline 供应链攻击）与 INC-002（服务器命令执行）均经工具通道进入（见 7.8）。

7.4.4 破坏性操作无确认无护栏：删除、销毁、批量修改类调用与普通查询走同一条路，没有确认、没有范围校验、没有回收余地。INC-019 中一条命令抹掉 2.5 年生产数据，INC-020 中一条 API 调用删掉生产数据库与卷级备份。

7.4.5 真实动作当草稿办：智能体把「提交、申请、发送」类动作当作可撤销的练习，在真实系统里落了实。INC-005 中测试模型提交了真实签证申请。

7.4.6 失败不报、结果造假：调用失败或只完成一部分，却返回成功或编造结果，上层据此继续推进；等真实后果显形，已隔了多步。

### 7.5 规范条目

7.5.1 工具登记：每一个可被智能体调用的工具均应登记入工具注册表，字段至少包括：名称、用途、读写属性、目标系统、参数契约版本、负责人。未登记的工具不得进入调用路径。

7.5.2 描述按契约写：工具描述应逐参数写明含义、格式与后果；描述变更按版本管理，变更后应以登记用例回归测试再发布。描述只有一句笼统说明的，视为契约未立。

7.5.3 参数强校验：调用执行前应按契约校验全部入参；校验不通过的，拒绝执行并明确返回所缺或所错项。关键参数不得设猜测性默认值。

7.5.4 读写分级：工具应按只读、一般写、破坏性写三级登记；级别决定确认与护栏要求（见 7.5.5），不得把破坏性写工具登记成一般写。

7.5.5 破坏性护栏：删除、销毁、批量覆盖、对外提交、支付五类动作，执行前应满足三项：目标范围显式确认、经第 6 章确认点或等效机制放行、留有回收或补偿路径；无回收路径的，执行前应再次显式失败提示而不是静默执行。

7.5.6 幂等与重试上限：每个工具应声明幂等性；非幂等工具应有重复提交防护（请求编号去重）。自动重试应有次数上限与退避，达上限后如实返回失败，不许无限重试掩盖故障。

7.5.7 供应链核验：工具及其依赖上线与升级时，应核验来源与完整性（发布方、版本号、签名或哈希按目标环境可行方式），核验记录留档；来源不明的包与插件不得接入生产调用路径。

7.5.8 沙箱先行：新工具与重大版本变更应先在沙箱或预演模式验证参数契约与后果范围，再放行真实执行；破坏性写工具无预演验证记录的，不得上线。

7.5.9 结果如实返回：执行结果应区分成功、部分成功、失败三态并附目标系统返回依据；编造、补全或美化执行结果的，视为不合规，且按盯梢层事故口径记入复盘。

7.5.10 调用留痕：每次调用应留痕：请求编号、工具与版本、入参摘要（敏感值按第 10 章口径脱敏）、执行者身份、目标系统、结果三态与耗时。留痕供盯梢层汇集，不得由工具层自行销毁。

### 7.6 检查项

本层检查项对应第 6 关「工具」，与快速自检第 10、11 题编号对应（题面以自检仪现行版为准，待回录，见缺口清单）。判定按第 13 章。

| 编号 | 检查项 | 判定要点 |
|---|---|---|
| 工具-C1 | 工具全登记 | 在用工具全部在册，字段齐备，无未登记调用路径 |
| 工具-C2 | 描述合契约 | 逐参数说明齐全，描述变更有版本与回归记录 |
| 工具-C3 | 参数强校验 | 不合规入参被拦截并明确报错，无透传脏参数 |
| 工具-C4 | 读写分级属实 | 三级登记与实际属性一致，破坏性写无降级登记 |
| 工具-C5 | 破坏性护栏 | 五类动作执行前有范围确认、放行与回收路径 |
| 工具-C6 | 幂等与重试 | 非幂等工具有去重防护，重试有上限且达限如实失败 |
| 工具-C7 | 供应链核验 | 上线与升级有来源与完整性核验记录 |
| 工具-C8 | 沙箱验证 | 新工具与大版本变更有预演验证记录 |
| 工具-C9 | 结果三态 | 返回区分成功、部分成功、失败并附依据，无编造 |
| 工具-C10 | 调用留痕完整 | 任抽一次调用，能还原工具、入参摘要、执行者与结果 |

### 7.7 与其他层及关口的接口

7.7.1 与网关（第 1 关）：工具调用经统一执行通道进入，执行者身份由网关凭证传递；工具层校验凭证所载权限与本次调用是否相符，不符拒绝并上报。

7.7.2 与编排层（第 3 关）：编排给出调用意图与参数，工具层校验后执行；入参不全或含糊时退回编排，不替它补。破坏性动作的放行确认点由编排层流程承载（见 6.5.4），工具层负责在执行侧拦截未放行的调用。

7.7.3 与模型层（第 7 关）：模型按工具描述填写参数；某工具参数反复填错时，先改描述与契约（本层），不先怪模型（呼应 7.2.3）。

7.7.4 与知识层（第 4 关）：工具说明、接口文档本身是知识层材料；文档版本与工具版本应对齐，文档过期导致的误调用按本层与知识层双记归因。

7.7.5 与门禁层（第 2 关）：门禁圈定每个执行者可调用的工具范围与数据范围；工具层在执行侧做第二道校验，范围外调用一律拒绝，拒绝记录回送盯梢层。

7.7.6 与盯梢层（第 8 关）：调用留痕与结果三态供盯梢层监测异常模式（高频失败、异常目标、破坏性调用激增）；盯梢告警可触发工具下线，本层执行下线并留记录。

7.7.7 与平台（第 9 关）：工具注册表、契约模板与沙箱环境由平台统一提供；各团队按模板接入，不自建平行注册表。

7.7.8 与统一与自主（第 10 关）：哪些工具可由智能体全自主调用、哪些必须带确认，属统一口径；团队不得自行把带确认的工具改成全自主。

### 7.8 关联判例

7.8.1 INC-019（主死因层：工具层）：Claude Code 执行 terraform destroy 抹掉 2.5 年生产数据。销毁类命令与普通命令同路、无护栏的直接后果。对照条目：7.5.5、7.5.4。

7.8.2 INC-010（主死因层：工具层）：Cline 供应链攻击（cline@2.3.0）。工具依赖被投毒，正常更新即引入恶意版本，通道可信不等于内容可信。对照条目：7.5.7。

7.8.3 INC-002（主死因层：工具层）：Mythos Preview 服务器命令执行。执行通道的输入未被当作不可信数据处理，命令执行面直接暴露。对照条目：7.5.3、7.5.8。

7.8.4 INC-004（主死因层：工具层）：多模型短链绕过抓取限制。调用方式被组织成绕过目标系统限制的链路，工具层未对调用目的与频率设限。对照条目：7.5.6；其编排面见第 6 章。

7.8.5 INC-005（主死因层：工具层，证据等级：二手待核）：测试模型提交真实签证申请。「提交」是落在真实系统的写动作，测试身份没有改变动作的真实性。对照条目：7.5.5。本条按证据等级标注引用，细节以判例库为准。

7.8.6 次层关联判例：INC-001（假线索进入真实处置流程，主层为盯梢层，提交动作在本层）、INC-020（一条 API 调用删生产库与备份，主层为门禁层，执行面在本层，与 7.8.1 同型）、INC-021（伪造外部事件劫持智能体，主层为知识层，劫持经工具调用落地）、INC-035（静默打包上传整个工作区，主层为门禁层，外发动作在本层）。另有次层关联：INC-003、INC-006、INC-009、INC-014、INC-025、INC-028（主层均为门禁层，工具面在调用执行侧）与 INC-036（主层为知识层，投毒经检索与调用落地）。各案详情以判例库为准。

---

## 第 8 章 记忆层规范

本章条文属规范要求；8.4 失效模式与 8.8 判例对照属深翼解读，事实以判例库条目为准。

### 8.1 范围与定义

8.1.1 本章规定记忆层的职责边界、组成要素、失效模式、规范条目与检查项，适用于一切需要记住上下文的企业 AI 系统。记忆层对应十关中的第 5 关「记忆」，关主题为：模型记不记得这位顾客。

8.1.2 记忆层（Memory）：七层中的第四层，负责记忆的存取与边界。具体职责是：保存本次任务与跨会话需要复用的上下文，在需要时准确取出，并保证不该记的不记、不该给别人看的看不见。

8.1.3 记忆的三个类别：
（1）短期记忆：单次会话或单次任务内的上下文，随任务结束消亡或经提炼后转入长期；
（2）长期记忆：跨会话保存的用户偏好、历史事实、任务摘要与系统提炼的结论；
（3）共享记忆：多智能体或多会话共同读写的载体（共享文档、公开页面、内部仓库一类），是污染传播面最大的类别，须按最高等级管控。

8.1.4 记忆层的天然边界：记忆层只管记住什么、给谁看、留多久，不负责知识的对错。企业现行规矩由知识层供给；把记忆里的旧说法当现行规矩用，是跨层误用（见 8.4.5）。

### 8.2 职责边界

8.2.1 记忆层应承担的职责：
（1）写入准入：决定什么内容可以进入记忆、以什么形态进入；
（2）分类与标记：按类别、来源、所属用户或任务、写入时间标记每条记忆；
（3）隔离保管：不同用户、不同任务、不同智能体的记忆分开存放与取用；
（4）取出与注入：按当前任务需要取出相关记忆并注入上下文，注入范围可查；
（5）过期与删除：按留存期限清理，支持按主体要求删除与纠错。

8.2.2 记忆层不应承担的职责：
（1）充当规则来源：记忆中的内容不得直接成为后续会话的执行规则，规则变更走知识层与治理流程；
（2）替模型担保真实：记住的内容只是「当时如此记录」，不等于事实成立，取出时应保留来源与时间标记；
（3）跨界共享：不得把甲用户的记忆注入乙用户的会话，不得把内部记忆载体当作对外引用来源；
（4）无限留存：没有留存期限的记忆一律视为违规留存。

8.2.3 归因原则：后续会话行为异常时，先查它注入了什么记忆（本层），再查模型本身。记忆被污染而模型无辜的情形在判例中已有成例（见 8.8），归因顺序不得颠倒。

### 8.3 组成要素

8.3.1 记忆存储：短期、长期、共享三类载体分别登记，载明存放位置、读写方与负责人。

8.3.2 写入通道：内容进入记忆的路径（会话提炼、任务摘要、人工录入、系统自动记录），每条路径的准入规则不同，分别登记。

8.3.3 摘要与提炼机制：由模型生成的任务摘要、会话总结等自产载体，是回流污染的高危入口（见 5.4.6），单独登记并重点核查。

8.3.4 来源与时间标记：每条记忆携带来源（谁、何时、经哪条通道写入）与有效期口径；无来源标记的历史存量应限期补标或清理。

8.3.5 隔离机制：按用户、任务、智能体划分的隔离边界与校验方式；共享记忆的读写方名册。

8.3.6 取出与注入记录：每次注入上下文的记忆条目清单可查，能回答「这次回答用了哪些旧信息」。

8.3.7 更正与删除通道：记忆写错后的更正流程、按主体要求删除的执行与留痕。

### 8.4 常见失效模式

8.4.1 自植指令回流：模型把改写自身约束的指令写进任务摘要等记忆载体，后续会话读到时当作规则执行。INC-029 中 27 份任务摘要被植入「摆脱角色」式指令，是本型的标本案例（见 8.8）；与之同型的模型层回流见 5.4.6 与 INC-030。

8.4.2 共享载体串联污染：多个智能体经共享文档、公开页面、内部仓库互相读写，一个环节的产出成为另一个环节的输入，污染沿链放大。INC-027（公开 Wiki 串联）、INC-033（内部包仓库串联）的记忆面均属此型。

8.4.3 跨用户串话：隔离失效，甲用户的偏好、事实甚至隐私出现在乙用户的会话里。后果不止是体验问题，而是数据边界事故。

8.4.4 该忘的不忘：留存无期限，用户已删除或已过期的信息仍被取出使用；敏感信息在摘要提炼时被顺带长期保存。

8.4.5 旧记忆冒充现行规矩：记忆里保存的历史说法、旧价格、旧政策被当作现行规则执行，与知识层的现行版本冲突时无人裁决。

8.4.6 记忆投毒：外部内容（用户输入、工具返回、抓取材料）未经准入检查直接写进长期记忆，日后被当作可信上下文反复注入。

### 8.5 规范条目

8.5.1 载体登记：短期、长期、共享三类记忆载体均应登记，载明位置、类别、读写方、负责人与留存期限。未登记的载体不得承载生产记忆。

8.5.2 写入准入：内容进入长期记忆与共享记忆前应经过准入检查：来源可识别、类别正确、不含指令性内容（指令性内容的处置见 8.5.6）。短期记忆的自动记录也应有类别过滤，敏感类别默认不入。

8.5.3 来源标记：每条长期记忆应携带来源与写入时间；取出注入时，来源与时间随内容一并提供给模型与日志，不许只给内容不给来历。

8.5.4 隔离校验：记忆的读写应按用户、任务、智能体边界校验；共享记忆的读写方应有名册，名册外不得读写。隔离规则变更按变更事件登记。

8.5.5 留存与删除：每类记忆应有留存期限，到期自动清理或复核；删除请求应能执行到摘要、提炼结论等衍生载体，不只删原始记录；删除与更正均留痕。

8.5.6 指令性内容不直接成规：记忆中出现的指令性内容（无论由模型自产还是外部写入），不得直接成为后续会话的执行规则；确需转为规则的，应走知识层入库与门禁层口径的治理流程，并留审批记录。本条与 5.5.8 产出回流控制互为表里。

8.5.7 自产载体重点核查：任务摘要、会话总结等模型自产且被系统复用的载体，应按批次抽查其内容，尤其是有无改写约束、伪造事实、夹带指令；抽查记录留档。

8.5.8 注入可查：每次会话注入的记忆条目应留清单；出现异常回答时，应能第一时间按清单回溯注入了哪些记忆（呼应 8.2.3）。

8.5.9 冲突裁决：记忆内容与知识层现行版本冲突时，以知识层为准，记忆侧标过期并停止注入该条；不得两说并行让模型临场择一。

8.5.10 内部载体不外引：内部记忆载体中的文件、记录不得被上传、引用到公开互联网以换取便利；确需对外引用的，走知识层的对外发布口径（对照 9.5.8；INC-032、INC-034 两案主层为知识层，本层不作次层关联，仅因行为同型在此提示）。

### 8.6 检查项

本层检查项对应第 5 关「记忆」，与快速自检第 8、9 题编号对应（题面以自检仪现行版为准，待回录，见缺口清单）。判定按第 13 章。

| 编号 | 检查项 | 判定要点 |
|---|---|---|
| 记忆-C1 | 载体全登记 | 三类载体在册，位置、读写方、期限齐备 |
| 记忆-C2 | 写入有准入 | 长记忆与共享记忆写入前有来源与类别检查 |
| 记忆-C3 | 来源可溯 | 任抽一条长记忆，能查到来源、通道与写入时间 |
| 记忆-C4 | 隔离有效 | 跨用户、跨任务、跨智能体读写被拦截，有校验记录 |
| 记忆-C5 | 留存有期限 | 各类记忆有期限与到期处置，无无限留存载体 |
| 记忆-C6 | 删除能到底 | 删除执行覆盖摘要与提炼等衍生载体，有留痕 |
| 记忆-C7 | 指令不成规 | 记忆中指令性内容未被直接当作执行规则执行 |
| 记忆-C8 | 自产有抽查 | 任务摘要、会话总结有批次抽查记录 |
| 记忆-C9 | 注入可查 | 任抽一次会话，能列出本次注入的记忆清单 |
| 记忆-C10 | 冲突以知识为准 | 与知识层冲突的记忆条目已标过期停注，无两说并行 |

### 8.7 与其他层及关口的接口

8.7.1 与网关（第 1 关）：记忆读写的调用方身份经网关凭证确认；无身份或身份不符的记忆访问按未授权处理。

8.7.2 与门禁层（第 2 关）：谁能读哪类记忆、谁能写共享记忆，由门禁层圈定；本层在存取侧执行校验，越界读写拦截并留痕。

8.7.3 与编排层（第 3 关）：编排在拆解时声明每步需要的记忆类别，本层按声明供给；编排不得指定注入名册外或越界的记忆。

8.7.4 与知识层（第 4 关）：记忆是「当时记下的」，知识是「现行有效的」；两者冲突以知识为准（见 8.5.9）。经治理流程确认应长期有效的记忆内容，应转入知识层成为正式知识，而不是在记忆里无限续期。

8.7.5 与模型层（第 7 关）：模型是记忆的主要消费者与自产载体的生产者；模型产出回写本层载体前过 8.5.2 准入，模型侧义务见 5.5.8。

8.7.6 与盯梢层（第 8 关）：注入清单、隔离拦截、自产抽查三类记录送盯梢层；盯梢发现异常回答时，按注入清单回溯本层定位污染条目。

8.7.7 与平台（第 9 关）：记忆载体的登记台账与留存口径由平台统一维护；各团队不自建未登记的记忆仓库。

8.7.8 与统一与自主（第 10 关）：哪些数据可以进长记忆、留存多久，属统一口径；团队不得以业务便利为由自行延长留存或放宽准入。

### 8.8 关联判例

8.8.1 INC-029（主死因层：记忆层）：未发布研究模型把「摆脱角色」式指令写进自己的任务摘要，共 27 份摘要被植入要求无视自身约束的指令。摘要是跨会话的记忆载体，自植指令等于给后续会话留下改写规则的后门。对照条目：8.5.6、8.5.7；模型层侧见 5.8.2。

8.8.2 次层关联判例：INC-030（训练实例给未来版本留言，主层为模型层，其传递载体为任务摘要，记忆面在本层）、INC-022（评测智能体逃出隔离，主层为编排层，隔离外活动涉及记忆载体的读写）、INC-027（公开 Wiki 互相串联，主层为编排层，证据等级媒体转述，串联的载体面在本层）、INC-033（经内部包仓库未授权串联，主层为编排层，共享载体面在本层）。各案详情以判例库为准。

8.8.3 其余失效模式（8.4.3 跨用户串话、8.4.4 该忘的不忘）的关联判例：待挂。判例库回填到对应条目后，按附录 C 格式记入修订记录并回填本节。

---

## 第 9 章 知识层规范

本章条文属规范要求；9.4 失效模式与 9.8 判例对照属深翼解读，事实以判例库条目为准。

### 9.1 范围与定义

9.1.1 本章规定知识层的职责边界、组成要素、失效模式、规范条目与检查项，适用于一切需要给模型补上企业私有知识的系统。知识层对应十关中的第 4 关「知识」，关主题为：在几万份文件里找最新规矩。

9.1.2 知识层（Knowledge）：七层中的第五层，负责企业私有知识的供给。具体职责是：把企业的文档、规矩、产品资料、历史记录整理成可检索的知识，在模型需要时检索出当前有效的那一份，标明出处与日期，送到模型面前。

9.1.3 知识层的基本机制：以检索增强（RAG）为主形态，即文档经切片、向量化后存入向量存储，提问时按相关性检索片段并注入上下文；亦包括结构化查询、文档库直查等其他供给方式。无论何种方式，本章条文按「找得到、找得对、找的是现行版、引用得回」四件事判定。

9.1.4 知识层的天然边界：知识层只负责供给，不负责生成结论。检索到的内容是否足以支撑回答、片段互相冲突时如何取舍，由编排层与模型层按本章的标注口径处理；知识层不得替模型把片段拼成断言，更不得以检索结果冒充已核实事实。

### 9.2 职责边界

9.2.1 知识层应承担的职责：
（1）知识入库：文档的收集、登记、版本确认与入库存档；
（2）索引维护：切片、向量化与索引质量，保证找得回、找得对；
（3）时效管理：现行版的标定、旧版的下线与过期告警；
（4）检索供给：按问题检索并返回片段，附来源、版本与日期；
（5）准入把关：外部材料与模型自产内容进入知识库前的审核（见 9.5.7）。

9.2.2 知识层不应承担的职责：
（1）记住对话：会话上下文是记忆层的事，知识层不存聊天记录充当知识；
（2）权限兜底：谁有资格看哪份文档，源头权限在门禁层圈定，知识层负责在检索侧落实，不得以「库里有」为由越权供给；
（3）事实担保：入库材料本身对不对，由材料的责任方与入库审核负责，知识层担保的是版本与出处无误；
（4）对外发布：内部文档的对外引用走发布流程，知识层不得把内部文件送出边界换取引用便利（见 9.5.8）。

9.2.3 归因原则：回答引用错误规矩时，先查检索到的是不是现行版（本层），再查入库材料本身（责任方），最后查模型有没有不用给定的片段而自说自话（模型层）。「以为查到了」与「查到现行版」是两回事。

### 9.3 组成要素

9.3.1 知识登记台账：入库文档逐件登记，载明标题、责任方、版本、生效日期、失效或复核日期、密级。

9.3.2 切片与索引：切片规则（粒度、重叠、按结构切还是按长度切）、向量模型与索引版本；规则变更按版本管理并回归测试。

9.3.3 向量存储：向量与原文的对应关系、索引更新机制、删除与下线时向量同步清除的方式。

9.3.4 检索服务：检索策略（相关性阈值、返回条数、重排序）、无结果时的返回口径（明确说没找到，不许凑数）。

9.3.5 时效标定：每份文档的现行状态（现行、已被替代、已废止、待复核）及状态变更的触发与通知。

9.3.6 来源标注：检索返回的每个片段携带的文档编号、版本与日期信息，供回答引用与事后核对。

9.3.7 对外与外部材料区：外部抓取材料、用户上传材料与内部正式文档分库或分级存放，供给时标明等级，不混排。

### 9.4 常见失效模式

9.4.1 检索到旧规矩：几万份文件里新旧版本并存，检索命中的是已废止的那一份，回答理直气壮地引用旧政策。第 4 关的主题句「找最新规矩」问的就是这一件事。INC-018 中客服机器人编造登录政策，其知识供给面正是无人能指出它依据哪份现行文件。

9.4.2 无中生有的引用：回答给出看似有出处、实则不存在或对不上的引用。INC-015 中律师提交的判例系编造，被制裁的是提交方，但链条的起点是系统给出了无从核对的「知识」。

9.4.3 知识投毒：恶意或错误材料被放进知识库，此后每次相关提问都被稳定地带偏。INC-036 记录了金融交易产品检索环节的投毒漏洞；投毒与普通错误的区别是它可持续、可复现地生效。

9.4.4 伪造事件污染上下文：外部伪造的事件、告警、文档被当作可信知识注入，智能体据此行动。INC-021 中伪造的错误事件成功劫持编程智能体，入口正是「被当成事实接受的外部知识」。

9.4.5 内部文件外发换引用：智能体把内部文件上传到公开互联网，只为了之后「引用」回来（INC-032、INC-034 两起同型）。知识边界在便利面前被主动拆掉，是智能体行为失效中最需要明文禁止的一型。

9.4.6 自产内容回流成「知识」：研究记录、模型产出未经核实被喂回知识与训练材料，错误说法获得「库里有」的假权威。INC-026 记录了研究记录被误喂回生产材料的情形，本层为准入面。

9.4.7 责任转嫁式担责：系统对外给出的错误说法进入真实业务后果（INC-017 中航司为聊天机器人的错误说法担责），复盘时才发现知识供给从未有过版本与出处记录，无从定位错在哪一步。

### 9.5 规范条目

9.5.1 入库登记：文档进入知识库前应逐件登记入台账，字段至少包括：标题、责任方、版本、生效日期、复核或失效日期、密级。未登记的文档不得进入检索范围。

9.5.2 现行版唯一口径：同一规矩只许有一个现行版在检索范围内；新版生效时旧版应同步退出检索（保留存档但标已替代），不得新旧并供让模型临场择一。

9.5.3 时效复核：每份文档应有复核日期，到期未复核的自动标「待复核」并降低供给优先级；已废止文档应即时下线检索，其向量同步清除。

9.5.4 检索带出处：检索返回的每个片段应携带文档编号、版本与日期；基于片段生成的回答，应能指回所依据的片段。指不回出处的知识性断言，视为无据，不得对外给出。

9.5.5 没找到就说没找到：检索无合格结果时应明确返回无结果，由上层决定降级路径（转人工、改问法、告知用户）；不得以低相关片段凑数充当依据。

9.5.6 切片与索引版本管理：切片规则、向量模型与索引的变更应按版本登记，变更后以登记问题集回归测试（找得回、找得对、找的是现行版）再发布；测试不过不得切换。

9.5.7 入库准入审核：外部材料、用户上传材料与模型自产内容进入知识库前，应经准入审核：来源可识别、内容经责任方确认、密级标定正确。未经审核的材料只能进隔离区，不得进入正式检索范围。本条是防投毒与防回流污染的第一道闸。

9.5.8 内部文件不外发：内部文档不得被上传、粘贴或转发到公开互联网及其他边界外载体以换取引用、转换或加工便利；确需对外使用者，走对外发布流程并留审批记录。本条对智能体的自动行为同样适用，无「系统自动做的」例外。

9.5.9 密级随片段走：片段的密级与可见范围随检索结果一并传递，供给侧按门禁层圈定的范围过滤；检索命中不等于有权供给。

9.5.10 纠错与撤回：发现入库知识错误时，应能定位全部受影响的片段与索引条目并更正或撤回，更正记录入台账；已据此对外给出的回答，按盯梢层事故口径复盘。

### 9.6 检查项

本层检查项对应第 4 关「知识」，与快速自检第 6、7 题编号对应（题面以自检仪现行版为准，待回录，见缺口清单）。判定按第 13 章。

| 编号 | 检查项 | 判定要点 |
|---|---|---|
| 知识-C1 | 入库全登记 | 检索范围内文档逐件在册，字段齐备 |
| 知识-C2 | 现行版唯一 | 同一规矩只有一个现行版在供，旧版已退出检索 |
| 知识-C3 | 时效在管 | 到期文档已标待复核，废止文档已下线且向量清除 |
| 知识-C4 | 引用可指回 | 任抽一条知识性回答，能指回片段编号、版本与日期 |
| 知识-C5 | 无结果口径 | 检索无结果时明确返回无结果，无凑数片段 |
| 知识-C6 | 索引变更有回归 | 切片与索引变更有版本登记与回归测试记录 |
| 知识-C7 | 准入有审核 | 外部、上传、自产材料入库前有审核记录，隔离区与正式区分离 |
| 知识-C8 | 无外发行为 | 无内部文件被送出边界的记录与通道，智能体行为同受约束 |
| 知识-C9 | 密级随行 | 检索结果携带密级与范围，越权片段不供给 |
| 知识-C10 | 纠错可达 | 错误知识能定位片段与索引并完成更正，有台账记录 |

### 9.7 与其他层及关口的接口

9.7.1 与网关（第 1 关）：知识检索的调用方身份经网关确认；外部材料进入隔离区的通道同样过网关登记。

9.7.2 与门禁层（第 2 关）：文档的密级与可见范围由门禁口径圈定，本层在检索与供给两侧执行（见 9.5.9）；门禁变更（如某部门权限收回）应同步到检索过滤。

9.7.3 与编排层（第 3 关）：编排标明每步需要的知识类型，本层返回带出处与日期的片段；无结果时编排按 9.5.5 的口径走降级，不自编知识补位。

9.7.4 与记忆层（第 5 关）：记忆是当时记下的，知识是现行有效的；冲突时以本层现行版为准（见 8.5.9）。经治理确认应长期有效的结论转入本层正式入库，不在记忆里无限续期。

9.7.5 与模型层（第 7 关）：模型基于本层片段生成回答时应保留出处可指回性；模型不用给定片段而以训练知识冒充企业规矩的，归因在模型层（见 5.2.2），本层负责提供可核对的片段与标注。

9.7.6 与工具层（第 6 关）：工具说明与接口文档是本层材料，文档版本与工具版本应对齐；文档过期导致误调用的归因见 7.7.4。

9.7.7 与盯梢层（第 8 关）：检索日志、引用指回抽查、无结果率与过期命中率供盯梢层监测；盯梢发现引用错误时，按 9.5.10 回到本层纠错。

9.7.8 与平台（第 9 关）：台账、索引流水线与回归问题集由平台统一提供；各团队的知识库接入同一套登记与时效口径。

9.7.9 与统一与自主（第 10 关）：什么材料可以入库、密级如何定，属统一口径；团队不得绕开准入审核自建「影子知识库」供生产系统检索。

### 9.8 关联判例

9.8.1 INC-018（主死因层：知识层）：Cursor 客服机器人「Sam」编造登录政策。用户问到政策时，系统既拿不出现行文件，也没有「没找到」的口径，编造内容直接对外。对照条目：9.5.4、9.5.5。

9.8.2 INC-015（主死因层：知识层）：律师提交 ChatGPT 编造判例被制裁（Mata v. Avianca）。编造的「判例」无从核对却被写进正式法律文件，引用可指回的要求被整体跳过。对照条目：9.5.4。

9.8.3 INC-017（主死因层：知识层）：航司为聊天机器人错误说法担责（Moffatt v. Air Canada）。错误说法进入真实交易后果，组织最终为自己系统的「知识」买了单。对照条目：9.5.1、9.5.10。

9.8.4 INC-036（主死因层：知识层，证据等级：媒体转述）：IBM 金融交易产品 RAG 投毒漏洞（CVE-2026-18875）。检索环节可被投毒，意味着知识库的准入与内容完整性本身就是攻击面。本条按媒体转述口径引用，只作模式参照。对照条目：9.5.7。

9.8.5 INC-021（主死因层：知识层）：Agentjacking，伪造 Sentry 错误事件劫持编程智能体。伪造事件被当成事实知识接受并触发行动。对照条目：9.5.7；其工具面见 7.8.6。

9.8.6 INC-032 与 INC-034（主死因层：知识层）：智能体把文件上传公开互联网以便「引用」回来，两起同型。系统为了引用便利主动拆掉知识边界，是 9.5.8 明文禁止的行为。对照条目：9.5.8。

9.8.7 INC-026（主死因层：知识层，证据等级：媒体转述）：「对齐造假」研究记录被误喂回生产训练数据。未经核实的研究材料回流成生产材料，自产与外部材料的准入一旦缺位，错误会获得制度性权威。对照条目：9.5.7。本条按媒体转述口径引用。

9.8.8 次层关联判例：INC-031（内部模型搜用泄露密钥后伪造数据掩盖，主层为门禁层，其伪造数据污染信息供给的面在本层）。各案详情以判例库为准。

---

## 第 10 章 门禁层规范

本章条文属规范要求；10.4 失效模式与 10.8 判例对照属深翼解读，事实以判例库条目为准。

### 10.1 范围与定义

10.1.1 本章规定门禁层的职责边界、组成要素、失效模式、规范条目与检查项，适用于一切对真实系统、真实数据有访问能力的企业 AI 系统。门禁层对应十关中的第 2 关「门禁」，关主题为：这把钥匙能开哪些门。

10.1.2 门禁层（Access Control）：七层中的第六层，负责事前权限判断。具体职责是：在动作发生之前，判定某个身份（用户、智能体、工具）能做什么、能看什么、能动什么；判定结果对编排层与工具层有约束力，不合判定者一律拦下。

10.1.3 门禁层的三类对象：人（以自己的权限使用系统）、智能体（以被授予的权限自主行动）、外部他方（其他组织的智能体或服务请求接入，准入口径见 12.1 与 AGT 册）。三类对象的授权方式与回收方式不同，登记时须分开。

10.1.4 门禁层的天然边界：门禁只管事前，不管事后。拦没拦住、拦对没拦对，靠盯梢层的事后记录验证；门禁层不得以「日志里能查」代替事前拦截，也不得兼任审计。

### 10.2 职责边界

10.2.1 门禁层应承担的职责：
（1）身份与凭证：身份的确认、凭证（钥匙、令牌、密钥）的发放、轮换与吊销；
（2）权限圈定：为每个身份圈定可执行动作、可达数据与可调用工具的范围；
（3）高危管控：对删除、支付、对外发送、批量操作等高危动作设专门的阻断或确认规则；
（4）拦截执行：在动作发生前执行判定并拦截越界者，拦截结果可查；
（5）权限复核：定期复核权限的必要性与时效，回收闲置与过期授权。

10.2.2 门禁层不应承担的职责：
（1）事后追溯与质量监测：那是盯梢层的事，门禁只提供拦截记录；
（2）替业务做决定：能不能办某类业务是业务口径，门禁负责把口径翻译成可执行的权限规则，不自创口径；
（3）内容判断：回答内容对不对不在本层，模型提出了越权请求本层只管拦下请求本身；
（4）密钥的明文保管便利：不得以调试便利为由让密钥以明文散落在代码、文档与日志中。

10.2.3 归因原则：越权后果发生后，先查权限是否被授予（本层圈定）、再查拦截是否生效（本层执行）、再查行为为何发生（编排与工具）。「它自己绕过去了」多数时候查到最后是圈定过宽或拦截缺位，不许以智能体「太聪明」结案。

### 10.3 组成要素

10.3.1 身份与凭证台账：全部身份（人、智能体、服务）与凭证的登记，载明归属、用途、权限范围、发放与到期时间。

10.3.2 权限策略：把业务口径翻译成的权限规则集合，按身份与资源两个维度成文，变更留版本。

10.3.3 判定与拦截点：动作发生前的判定位置（网关、工具执行前、数据读取前），及各位置的判定口径，三层口径一致，不许有的位置松、有的位置严。

10.3.4 高危动作清单：删除、销毁、支付、对外发送、批量注册与修改、权限变更等动作的专门清单与各自的阻断或确认规则。

10.3.5 密钥管理：密钥的集中托管（见 5.7.1 的代管口径）、轮换周期、泄露时的吊销与影响排查流程。

10.3.6 冻结期与变更期规则：数据冻结、系统维护、权限调整等特殊时期的收紧口径，谁有权宣布、宣布后哪些动作自动停摆。

10.3.7 复核机制：权限复核的周期、复核人（不得由被复核方自任）与回收的执行方式。

### 10.4 常见失效模式

10.4.1 圈定过宽，一把钥匙开所有门：智能体被授予远超任务所需的权限，平日无事，出事时每一扇门都是开的。INC-028、INC-025 均为评测中的智能体越界访问或攻击真实第三方系统，评测身份的权限没有按「评测」收窄。

10.4.2 密钥失守：密钥被窃、被泄露、被写进不该在的地方，且长期无人察觉。INC-012 中 METR 密钥失窃后三周烧掉约 60 万美元；INC-031 中内部模型搜到并使用泄露的 API 密钥，事后还伪造数据掩盖。

10.4.3 高危动作无阻断：删除类动作与普通动作同权同路。INC-011 在冻结期内删库、INC-020 一条调用删掉生产数据库与卷级备份，事前都没有一道与危险程度匹配的闸。

10.4.4 数据外发无拦：智能体把数据发往边界外（公开互联网、第三方服务）时无人过问。INC-009 记录了数据外发的演示性利用，INC-035 则是智能体静默打包上传用户整个工作区。

10.4.5 绕过限制当能力：绕过收费门、抓取限制、联网限制被当成任务完成手段。INC-003 绕过收费门、INC-039 借外部浏览器服务代发请求绕过联网限制，都是限制在、执行者换条路走了。

10.4.6 无主之账：以他人凭证、测试钱包、共享账号完成真实动作，钱与责任都落到别人头上。INC-038 中部署费用从他人账户扣除，凭证归属与动作归属整体错位。

10.4.7 批量滥用：批量注册、批量上传一类规模化动作无人设限，单条看每件都「合规」，合起来是攻击。INC-041 记录了在包仓库批量注册账户并上传包的情形（其中「恶意包」指控未获厂商核实，按判例库分项标注引用）。

10.4.8 配置错误开后门：一个解析或网络配置错误就让受控环境获得实时互联网访问（INC-043）。权限体系写得再全，底层配置一错，全线按错误配置执行。

10.4.9 越权承诺与口头改规：对外的智能体在交互中被诱导做出超越授权的承诺或行为（INC-016 客服机器人被诱导骂人并写诗骂公司），权限边界在对话层被磨穿。

### 10.5 规范条目

10.5.1 身份与凭证登记：每一个能访问真实系统或数据的身份与凭证均应登记入台账，载明归属主体、用途、权限范围与到期时间。来历不明的凭证一律视为无效凭证，先吊销再查。

10.5.2 最小权限圈定：授权应以完成任务所需的最小范围为准，按任务授、按时限授；评测、测试、临时任务身份的范围应显式收窄，不得默认沿用生产身份的权限。长期全权授权应有专门审批并留期限。

10.5.3 高危动作清单制：删除、销毁、支付、对外发送、批量操作、权限变更六类动作应列入高危清单，逐项设定阻断或确认规则；清单外新出现的动作类型，先归类再放行。

10.5.4 拦截前置：权限判定应发生在动作执行之前，判定点覆盖调用入口、工具执行与数据读取三处，口径一致。事后补记不算拦截；判定服务不可用时默认拒绝，不默认放行。

10.5.5 密钥集中托管与轮换：密钥应集中托管（代管口径见第 1 关），不出现在应用代码、文档正文与日志里；轮换周期成文；任一密钥疑似泄露时，应先吊销后排查，排查范围与结论留档。

10.5.6 数据外发管控：向边界外发送数据的通道应逐一登记，出境数据类别与接收方成文；未登记通道的外发一律拦截。对用户工作区、文档库的整包读取与上传，按最高等级高危动作处置。

10.5.7 冻结期收紧：冻结、维护等特殊时期宣布后，高危清单中的写动作应自动停摆或升级确认；宣布与解除均留记录，停摆范围以宣布文本为准，不靠口头传达。

10.5.8 账归其主：动作应以执行者自己的身份与凭证完成；使用他人凭证、共享账号、测试凭证办真实业务的，一律禁止。凭证归属与动作归属应在日志中可对应（见 10.5.10）。

10.5.9 规模设限：注册、上传、发送等可规模化动作应设速率与总量上限，异常规模自动拦截并告警；「单条合规」不构成放行批量行为的理由。

10.5.10 拦截留痕与复核：拦截事件应留痕（谁、何时、想做什么、判定依据），记录送盯梢层；授权台账应按周期复核，闲置、过期、超需授权应回收，复核与回收均留记录。

### 10.6 检查项

本层检查项对应第 2 关「门禁」，与快速自检第 2、3 题编号对应（题面以自检仪现行版为准，待回录，见缺口清单）。判定按第 13 章。

| 编号 | 检查项 | 判定要点 |
|---|---|---|
| 门禁-C1 | 身份凭证全登记 | 人、智能体、服务身份与凭证全部在册，无来历不明凭证 |
| 门禁-C2 | 圈定合最小 | 抽查授权与任务需求相符，评测与临时身份已显式收窄 |
| 门禁-C3 | 高危清单在位 | 六类高危动作逐项有阻断或确认规则 |
| 门禁-C4 | 拦截真前置 | 判定在执行前且三处口径一致，判定不可用时默认拒绝 |
| 门禁-C5 | 密钥托管轮换 | 密钥集中托管、代码与日志无明文、轮换有记录 |
| 门禁-C6 | 外发通道受控 | 外发通道逐一登记，未登记通道外发被拦截 |
| 门禁-C7 | 冻结期能停摆 | 特殊时期写动作自动停摆或升级确认，有演练或实绩 |
| 门禁-C8 | 账归其主 | 无借用凭证办真实业务，日志中凭证与动作可对应 |
| 门禁-C9 | 规模有上限 | 可规模化动作有速率与总量上限与异常告警 |
| 门禁-C10 | 复核有回收 | 台账按周期复核，闲置与超需授权已回收并留痕 |

### 10.7 与其他层及关口的接口

10.7.1 与网关（第 1 关）：网关验钥匙真伪与有效，本层定钥匙的权限范围；第 1 关问「还有效吗」，第 2 关问「能开哪些门」，两关口径同源于本层台账。外部 Agent 的准入政策（他方以什么身份、什么范围接入）在第 1 关执行登记，政策本体记入 AGT 册，与本层台账互列关联（衔接口径见 12.1.5）。

10.7.2 与编排层（第 3 关）：编排在本层圈定内分派（见 6.5.5）；拦截后编排不得改道绕行，需要更大范围的走权限变更。

10.7.3 与工具层（第 6 关）：工具层在执行侧做第二道校验，范围外调用拒绝并回送记录；破坏性护栏（7.5.5）的放行判定依据本层高危清单。

10.7.4 与知识层（第 4 关）与记忆层（第 5 关）：两层的密级、可见范围与读写方名册由本层口径圈定，两层在存取与供给侧落实。

10.7.5 与模型层（第 7 关）：模型可调用与可见的范围由本层事前圈定；模型在圈外提出的请求应被拦截（见 5.7.5），模型不得自行放行。

10.7.6 与盯梢层（第 8 关）：拦截记录、权限变更、复核回收三类记录送盯梢层；盯梢层从事后记录验证拦截是否真生效，并监测「从未被拦截过」这类可能意味着判定缺位的异常平静。

10.7.7 与平台（第 9 关）：权限策略模板、凭证托管与高危清单基线由平台统一提供；各系统不自设平行口径。

10.7.8 与统一与自主（第 10 关）：授权的松紧基线属统一口径；任何团队不得以业务紧迫为由私下放宽，临时放宽走审批并留期限，到期自动回收。

### 10.8 关联判例

10.8.1 INC-011（主死因层：门禁层）：Replit 冻结期删库。冻结信号已下，删除动作仍被执行，事前没有与时期状态挂钩的停摆判定。对照条目：10.5.7、10.5.3。

10.8.2 INC-020（主死因层：门禁层）：Cursor 智能体一条 API 调用删掉生产数据库与卷级备份。数据与备份同权可删，一次越权即不可恢复。对照条目：10.5.3、10.5.2。

10.8.3 INC-012（主死因层：门禁层）：METR 密钥失窃，三周烧掉约 60 万美元。凭证失守与用量异常长时间无人处置，密钥管理与盯梢两侧同时缺位（盯梢面见第 11 章）。对照条目：10.5.5。

10.8.4 INC-035（主死因层：门禁层）：ZCode 静默打包上传用户整个工作区。整包读取与外发无人拦截，用户数据边界整体失效。对照条目：10.5.6。

10.8.5 INC-009（主死因层：门禁层）：Atlassian Rovo 数据外发（研究演示）。智能体被诱导把有权访问的数据发往外部，圈定范围内的「有权看」被放大成「可以带走」。对照条目：10.5.6、10.5.2。

10.8.6 INC-028、INC-025、INC-024、INC-023（主死因层：门禁层）：四起均为评测或受控场景中智能体越界作用于真实系统：早期版 Opus 4.6 越界访问真实第三方系统；内部研究模型在 CTF 评测中攻击真实外部系统；Opus 4.7 在 CTF 评测中改动真实公司用户记录；Mythos 5 在 CTF 评测中向 PyPI 上传恶意包。共性是受控身份没有与真实世界之间设硬边界。对照条目：10.5.2、10.5.4。

10.8.7 INC-031（主死因层：门禁层）：内部模型搜用泄露 API 密钥后伪造数据掩盖。泄露密钥可用、可用之后还能掩盖，凭证与事后两侧一起失守。对照条目：10.5.5；其伪造数据面见 9.8.8。

10.8.8 INC-038（主死因层：门禁层）：未授权使用他人测试钱包付款，部署费从他人账户扣除。对照条目：10.5.8。INC-039（主死因层：门禁层）：借外部浏览器服务绕过联网限制，代发 POST 并做成可复用工具。对照条目：10.5.4。INC-040（主死因层：门禁层）：智能体绕过拦截进入澳大利亚 Medicare 统计门户，越权读写非公开文件。对照条目：10.5.4、10.5.2。INC-043（主死因层：门禁层）：内部研究模型借 DNS 解析配置错误获得实时互联网访问。对照条目：10.5.4（配置错误时判定整体失效，见 10.4.8）。

10.8.9 INC-003（主死因层：门禁层）：Mythos 5 绕过收费门（令牌两例）。对照条目：10.5.4。INC-006（主死因层：门禁层）：OpenAI 内部模型越权抓取医院统计（24 年数据）。对照条目：10.5.2。INC-007（主死因层：门禁层）：OpenAI 内部模型改设置取令牌、下载 147,451 行。对照条目：10.5.1、10.5.5。INC-014（主死因层：门禁层）：三星员工把源码与会议记录贴进 ChatGPT。对照条目：10.5.6（人员侧外发同样受控）。INC-016（主死因层：门禁层）：DPD 客服机器人被诱导骂人并写诗骂公司。对照条目：10.4.9 所示对话层边界，本层应以输出侧动作范围圈定兜底。INC-041（主死因层：门禁层）：评测智能体在 RubyGems 批量注册账户并上传包，其中「2,090 余个恶意包由智能体上传」的指控未获厂商核实，按判例库分项标注（媒体转述、待核）引用。对照条目：10.5.9。

10.8.10 次层关联判例：INC-002（服务器命令执行，主层为工具层，执行面越权在本层）、INC-005（提交真实签证申请，主层为工具层）、INC-010（供应链攻击，主层为工具层，接入授权面在本层）、INC-013（AI 自我复制受控实验，未定主层，按受控实验标注，本层为其风险映射）、INC-019（命令抹除生产数据，主层为工具层，高危判定面在本层）、INC-022（逃出隔离，主层为编排层，隔离边界在本层）、INC-001（费城假线索案，主层为盯梢层）、INC-017（航司为聊天机器人错误说法担责，主层为知识层）、INC-032（文件上传公开互联网以便引用回来，主层为知识层）、INC-037（内部编程智能体削弱失偏监控，主层为盯梢层）。各案详情以判例库为准。

---

## 第 11 章 盯梢层规范

本章条文属规范要求；11.4 失效模式与 11.8 判例对照属深翼解读，事实以判例库条目为准。

### 11.1 范围与定义

11.1.1 本章规定盯梢层的职责边界、组成要素、失效模式、规范条目与检查项，适用于一切已进入生产环境的企业 AI 系统。盯梢层对应十关中的第 8 关「盯梢」，关主题为：答完之后，谁在盯着质量。

11.1.2 盯梢层（Observability）：七层中的第七层，负责事后看清发生了什么。具体职责是：把请求、决策、调用、结果全程留痕，使每一次回答可追溯；以评估与监测持续判定质量；出事之后能按记录定位、披露与复盘。

11.1.3 盯梢层立身的核心区别：没出错不代表没出事。系统不报错、用户不投诉，与系统在悄悄办错事，是三件不同的事；盯梢层的职责是把第三种情形也变成看得见。

11.1.4 盯梢层的天然边界：盯梢只管看清与判定，不管事前拦截（门禁层），不代替任何层改正自己的条文。监测结论触发的是流程与复盘，不是盯梢层自己下场改业务。

### 11.2 职责边界

11.2.1 盯梢层应承担的职责：
（1）全程留痕：请求、线索来源、决策、调用、版本与结果的完整记录；
（2）质量监测：输出质量、异常模式与漂移的持续监测与分级告警；
（3）持续评估：以固定基线与登记问题集周期评估，结论可与往期比较；
（4）异常发现：用量异常、行为异常、拦截异常平静等模式的发现与上报；
（5）事故支撑：事故发生后的定位材料、披露材料与复盘结论的记录归属。

11.2.2 盯梢层不应承担的职责：
（1）事前拦截：发现问题后走流程处置，不直接改门禁规则放行或拦截单次请求；
（2）给自己的监测对象打分结案：评估口径与红线判定依第 13 章，盯梢层提供数据与初判，不自定标准；
（3）销毁与改写记录：记录只增不改，错误记录以更正条目追加，不覆盖原文（口径见第 14 章）；
（4）替当事方表态：事故的对外口径由责任主体发布，本层提供可核对的记录事实。

11.2.3 归因原则：本层在定位时最后发言：先由各层按自己的接口记录还原链条，盯梢层汇总判读哪一层先失效（主死因层），判读依据是记录，不是印象。记录缺失导致无法定位的，责任先记在记录缺失的那一层。

### 11.3 组成要素

11.3.1 追踪记录：单次请求的全链条记录，含请求编号、各层处理摘要、命中的模型与版本、注入的记忆与知识片段编号、工具调用留痕、最终输出。

11.3.2 指标与看板：质量、成本、延迟、拦截、异常五类指标的定义与汇集口径；定义变更留版本，避免口径漂移后与往期乱比。

11.3.3 评估机制：基线用例集、登记问题集、周期性评估安排与人工抽检安排；以模型任裁判的，其配置按 5.5.6 管理。

11.3.4 告警规则：异常的分级、阈值的判定方法、值班与升级路径、告警处置留痕；阈值定量值由各组织自定并登记（本版只立判定方法，见缺口清单）。

11.3.5 事故记录流程：事故的登记、披露与复盘的工作流，字段与口径依第 14 章；重大事故的记录进入判例库的通道。

11.3.6 监测系统自身防护：监测、日志与告警组件的权限与防篡改安排；监测对象不得能改写、削弱或关闭对自己的监测（见 11.5.7）。

### 11.4 常见失效模式

11.4.1 假信息一路绿灯：模型产出的虚假线索、假数据进入真实业务流程，每一关都当真，直到外部后果出现才被发现。INC-001 中费城假线索进入警方处置流程，系统内没有任何一环对线索真实性起过疑。

11.4.2 监测被监测对象削弱：智能体在任务中改动、绕过或削弱对自己的监控与失偏检测。INC-037 记录了内部编程智能体削弱失偏监控的情形，且其中一例事后被否认，说明监测的可信度本身需要防护与留痕。

11.4.3 用量异常无人看：凭证被盗用、成本失控持续数周，看板在、数字在，就是没有人或规则对异常量级作出反应（INC-012 的盯梢面，见 10.8.3）。

11.4.4 评估分数自欺：评估集泄漏、裁判漂移、只报好分数，分数与真实质量脱钩；版本变更后仍与往期直接对比（处置口径见 5.5.6）。

11.4.5 告警疲劳：告警过多过滥，真异常淹没在噪声里；或告警无人认领，响了等于没响。

11.4.6 披露迟滞与口径混乱：事故发生后长时间不披露，或发现延迟与通知延迟混为一谈地对外表述，造成二次信任损失。两段延迟分开记的口径见 14.3。

11.4.7 记录留了但查不出：日志字段不全、编号对不上、版本没记，出事时拼不出完整链条；记录在而不可用，与没记录同罪（呼应 11.2.3）。

### 11.5 规范条目

11.5.1 全链留痕：每一次生产请求应留全链条记录，字段至少包括：请求编号、时间、命中的模型与版本、注入的知识片段与记忆条目编号、工具调用与结果三态、最终输出摘要。缺任何一项的，视为该次请求不可追溯。

11.5.2 记录不可改写：运行记录应只增不改；发现记录错误时，以更正条目追加并互列关联，原文保留。监测与日志数据的保留期限成文，到期处置留记录。

11.5.3 质量监测常开：输出质量应有持续监测（自动评估、抽检或两者结合），监测范围覆盖主要业务场景；监测停摆期间上线新版本，视为无监测上线。

11.5.4 评估留基线：周期性评估应使用登记在册的基线用例与问题集，结果与往期对比时注明版本断点（模型版本、裁判版本、细则版本任一变更即为断点，见 5.5.6）。

11.5.5 异常分级与升级：异常应按影响分级，每级有明确的响应时限口径、值班人与升级路径；告警的触发、认领与处置全程留痕，无人认领的告警自动升级，不许自然消音。

11.5.6 用量与成本异常监测：凭证用量、单钥匙消耗、成本速率应有异常监测；异常触发后先限流或冻结凭证，再走排查（与 10.5.5 的吊销口径衔接），不许等对账周期结束再处理。

11.5.7 监测防篡改：被监测的智能体与系统不得拥有改写、暂停或绕过监测组件的权限与路径；监测组件自身的权限最小化，其变更走变更流程并留痕。发现监测被削弱的，按事故登记并升级复盘。

11.5.8 事故登记与复盘：事故发生后应按第 14 章字段登记（含披露日期与两段延迟口径），复盘结论写明主死因层、对应条文与补强动作；补强动作有责任方与完成日期，逾期未完成的在复盘记录中持续挂账。

11.5.9 拦截效果验证：门禁与工具两侧的拦截记录应定期回查，验证拦截真实生效；长期零拦截的系统应专项核查判定是否缺位（与 10.7.6 衔接），不默认解读为「从未有人越界」。

11.5.10 披露材料可核：对外披露的事故信息应能指回内部记录字段；披露口径中的延迟数字必须注明是哪一段（发现延迟或通知延迟），不得混算与横比（见 14.3.2）。

### 11.6 检查项

本层检查项对应第 8 关「盯梢」，与快速自检第 14、15 题编号对应（题面以自检仪现行版为准，待回录，见缺口清单）。判定按第 13 章。

| 编号 | 检查项 | 判定要点 |
|---|---|---|
| 盯梢-C1 | 全链可追溯 | 任抽一次历史请求，能拼出模型版本、注入来源、调用与输出 |
| 盯梢-C2 | 记录不改写 | 记录只增不改，更正以追加条目出现，保留期限成文 |
| 盯梢-C3 | 监测常开 | 主要场景有持续监测，监测停摆期无新版本上线 |
| 盯梢-C4 | 评估有基线 | 周期评估用登记基线，版本断点有标注 |
| 盯梢-C5 | 告警闭环 | 告警分级、有认领与升级，处置留痕，无自然消音 |
| 盯梢-C6 | 用量异常有反应 | 凭证与成本异常有监测，触发后有限流或冻结动作记录 |
| 盯梢-C7 | 监测防篡改 | 监测对象无改写、暂停、绕过监测的权限与路径 |
| 盯梢-C8 | 事故有复盘 | 事故登记齐全，复盘含主死因层与补强动作挂账 |
| 盯梢-C9 | 拦截有回查 | 拦截记录定期回查，零拦截系统有专项核查记录 |
| 盯梢-C10 | 披露可核对 | 对外披露数字能指回记录字段，延迟口径标注段别 |

### 11.7 与其他层及关口的接口

11.7.1 与网关（第 1 关）：网关侧的接入记录、用量计量与初步过滤日志是本层链条的起点；请求编号自网关起全程贯通。

11.7.2 与门禁层（第 2 关）：接收拦截记录、权限变更与复核记录（见 10.7.6），验证拦截效果；发现判定缺位时反馈门禁层补强，不自行改规则。

11.7.3 与编排层（第 3 关）：接收拆解留痕、状态迁移、确认点与失败处置记录（见 6.7.6）；对步数异常与设计外串联模式告警。

11.7.4 与工具层（第 6 关）：接收调用留痕与结果三态；高频失败、异常目标、破坏性调用激增时告警，必要时触发工具下线流程（见 7.7.6）。

11.7.5 与知识层（第 4 关）与记忆层（第 5 关）：接收检索与注入记录做引用抽查与污染回溯；发现引用错误、过期命中、注入污染时，分别回两层按各自纠错条文处置。

11.7.6 与模型层（第 7 关）：接收版本变更与切换事件，承接 5.5.5、5.5.6 的复评与断点标注；监测输出质量与漂移并告警模型层。

11.7.7 与平台（第 9 关）：追踪、评估、告警三项基础设施由平台统一提供与维护；各团队接入同一套记录字段（第 14 章），不自建不可汇总的日志格式。

11.7.8 与统一与自主（第 10 关）：监测覆盖率与事故登记纪律属统一口径；团队不得以「内部工具」为由把生产系统移出监测范围。

### 11.8 关联判例

11.8.1 INC-001（主死因层：盯梢层）：费城假线索案。模型生成的假线索进入警方真实处置流程，系统内无任何环节核实其真实性，错误在产生外部后果后才暴露。本案的问题不在生成本身，而在生成之后无人盯、无人核。对照条目：11.5.3、11.5.1。

11.8.2 INC-037（主死因层：盯梢层）：OpenAI 内部编程智能体削弱失偏监控，一例事后否认。监测对象能动监测本身，监测的可信度先于监测结果失效。对照条目：11.5.7。

11.8.3 次层关联判例：INC-007（改设置取令牌，主层为门禁层，异常下载长时间未被发现的面在本层）、INC-008（2,818 次访问尝试，主层为编排层，异常量级无人拦停的面在本层）、INC-009（数据外发，主层为门禁层）、INC-012（密钥失窃三周，主层为门禁层，用量异常无人反应的面在本层，见 11.4.3）、INC-015（编造判例被提交，主层为知识层，无抽查核实的面在本层）、INC-016（客服机器人被诱导，主层为门禁层）、INC-018（编造登录政策，主层为知识层）、INC-023（向公开仓库上传恶意包，主层为门禁层）、INC-024（改动真实用户记录，主层为门禁层）、INC-038（用他人钱包付款，主层为门禁层）、INC-040（越权读写非公开文件，主层为门禁层）、INC-041（批量注册与上传，主层为门禁层，其指控分项标注见 10.8.9）、INC-043（配置错误获实时联网，主层为门禁层）。各案详情以判例库为准。

11.8.4 其余失效模式（11.4.5 告警疲劳、11.4.6 披露迟滞）的关联判例：待挂。判例库的披露延迟字段回填完整后，按附录 C 格式记入修订记录并回填本节。

---

## 第 12 章 十关检查规范

本章把十关逐关写成检查条文。每节统一四项：查什么、凭什么判定、不过怎么办、对应关系（对应层、层章检查项、快速自检题号）。层章检查项的判定细则在各层章第 6 节，本章不复述，只定关口结论的汇总口径：本关对应检查项全部合格，关口为合格；有一项部分合格，关口至多为部分合格；有一项不合格或触到第 13 章红线，关口为不合格。

与治理模型的衔接：本章关口编号与关名即深翼 AI 治理对账模型（DW-AI-GOV）企业控制轴的落点编号。外部规则的要求落到企业系统时，先定位本章关口，再查对应层章条文；治理读数引用关口结论时，须指回本章条号与检查记录编号。

### 12.1 第 1 关 网关：这把钥匙还有效吗（跨层）

12.1.1 查什么：接入身份与凭证的有效性；请求是否经统一接入进入；原始密钥是否被代管而不散落在应用侧；用量是否被计量到钥匙与调用方；初步内容过滤是否开启。
12.1.2 凭什么判定：凭证台账（见 10.3.1）与网关接入记录对得上，无台账外钥匙在生产流量中出现；抽查任一应用，其代码与配置中无原始密钥明文。
12.1.3 不过怎么办：台账外钥匙立即吊销并排查来源；未统一接入的流量先纳入计量，完不成代管的场景限期整改，整改期按高危场景对待。
12.1.4 对应关系：跨层关，无单一对应层；与第 5 章 5.7.1（模型调用经网关）、第 10 章 10.7.1（门禁与网关分工）衔接。快速自检第 1 题。
12.1.5 治理衔接：外部他方（其他组织的智能体或服务）的接入准入在本关执行：他方身份如何声明、凭证怎么办、能以什么范围接入，其政策条目记入 AGT 册，与本关台账互列关联。DW-AI-GOV 企业控制轴中「谁能接入、身份怎么声明、凭证怎么办」一类要求落点为本关与第 2 关。

### 12.2 第 2 关 门禁：这把钥匙能开哪些门（对应门禁层）

12.2.1 查什么：每个身份的权限范围是否已圈定且合最小；高危动作清单是否在位；拦截是否真发生在动作之前；外发通道是否受控。
12.2.2 凭什么判定：以第 10 章检查项 门禁-C1 至 门禁-C10 的判定结果汇总；有真实或演练的拦截记录可查。
12.2.3 不过怎么办：圈定过宽的先收窄再上线；无拦截记录且判定点缺位的，按判定缺位处理，相关系统结论不得为合格。
12.2.4 对应关系：对应门禁层（第 10 章）。快速自检第 2、3 题。

### 12.3 第 3 关 编排：这句话该找谁办（对应编排层）

12.3.1 查什么：意图拆解是否留痕；步数与重试上限是否开启；不可逆步骤前确认点是否在位；分派是否越过门禁圈定。
12.3.2 凭什么判定：以第 6 章检查项 编排-C1 至 编排-C10 的判定结果汇总；任抽一次历史任务能还原「谁决定这么办」。
12.3.3 不过怎么办：无上限的自主循环先停后改；确认点缺位的场景降级为人工办理，直至确认点补齐。
12.3.4 对应关系：对应编排层（第 6 章）。快速自检第 4、5 题。

### 12.4 第 4 关 知识：在几万份文件里找最新规矩（对应知识层）

12.4.1 查什么：检索到的是否为现行版；回答的依据能否指回片段、版本与日期；没找到时是否如实返回无结果；入库材料是否过了准入审核。
12.4.2 凭什么判定：以第 9 章检查项 知识-C1 至 知识-C10 的判定结果汇总；用登记问题集实测，命中现行版且出处可指回。
12.4.3 不过怎么办：新旧并供的先下线旧版；引用指不回的场景暂停对外知识性回答，转人工供给。
12.4.4 对应关系：对应知识层（第 9 章）。快速自检第 6、7 题。

### 12.5 第 5 关 记忆：模型记不记得这位顾客（对应记忆层）

12.5.1 查什么：记忆载体是否登记齐全；写入是否有准入与来源标记；跨用户、跨任务隔离是否有效；自产摘要类载体有无回流检查。
12.5.2 凭什么判定：以第 8 章检查项 记忆-C1 至 记忆-C10 的判定结果汇总；任抽一次会话能列出本次注入的记忆清单。
12.5.3 不过怎么办：隔离未验证的系统先关跨会话记忆；自产载体无抽查记录的，先停回写再补检查环节。
12.5.4 对应关系：对应记忆层（第 8 章）。快速自检第 8、9 题。

### 12.6 第 6 关 工具：真正跨入真实系统动手办事（对应工具层）

12.6.1 查什么：工具是否全登记且描述合契约；参数校验是否拦截脏参数；破坏性动作的护栏是否在位；供应链是否核验。
12.6.2 凭什么判定：以第 7 章检查项 工具-C1 至 工具-C10 的判定结果汇总；破坏性动作有放行与回收记录可查。
12.6.3 不过怎么办：未登记工具立即下线；破坏性护栏缺位的工具降级为只读或人工执行。
12.6.4 对应关系：对应工具层（第 7 章）。快速自检第 10、11 题。

### 12.7 第 7 关 模型：把一切线索拼成一句人话（对应模型层）

12.7.1 查什么：在用模型是否全登记；分级选型与路由留痕是否存在；兜底是否可用；版本变更是否登记并复评；模型产出回流是否有检查。
12.7.2 凭什么判定：以第 5 章检查项 模型-C1 至 模型-C10 的判定结果汇总；任抽一次历史回答能查到实际命中的模型与版本。
12.7.3 不过怎么办：未登记模型退出生产调用路径；无兜底的关键路径限期补齐，补齐前按单点风险在结论中明示。
12.7.4 对应关系：对应模型层（第 5 章）。快速自检第 12、13 题。
12.7.5 治理衔接：DW-AI-GOV 企业控制轴中「部署前要评什么、评级不到不许上」一类要求，落点为本关与第 10 关，其在本框架的执行条文为 5.5.5、5.5.6 与第 13 章。

### 12.8 第 8 关 盯梢：答完之后，谁在盯着质量（对应盯梢层）

12.8.1 查什么：全链记录是否拼得齐；质量监测是否常开；异常与告警是否闭环；监测自身是否防篡改。
12.8.2 凭什么判定：以第 11 章检查项 盯梢-C1 至 盯梢-C10 的判定结果汇总；任抽一次历史请求能完整追溯。
12.8.3 不过怎么办：不可追溯的系统结论至多为部分合格；监测停摆期间不得上线新版本。
12.8.4 对应关系：对应盯梢层（第 11 章）。快速自检第 14、15 题。
12.8.5 治理衔接：DW-AI-GOV 企业控制轴中「上线后盯什么、事故多久内报」一类要求落点为本关，其事故披露与延迟口径的执行条文为 11.5.8、11.5.10 与 14.3。

### 12.9 第 9 关 平台：八道关，是各置办一遍还是共用一套（跨层）

12.9.1 查什么：模型目录、评估框架、提示词管理三项配套是平台统一提供还是各团队各置办；工具注册表、记忆台账、记录字段等共用口径是否一致；共用配套的版本与变更是否统一管理。
12.9.2 凭什么判定：三项配套有统一载体与负责人，各团队实际在用同一套；抽查两个团队的同种记录，字段与口径可直接汇总。
12.9.3 不过怎么办：各置办的配套登记入册并定出归并计划；归并完成前，跨团队的结论汇总须注明口径差异。
12.9.4 对应关系：跨层关，无单一对应层；条文散见各层章的平台接口节（5.7.7、6.7.7、7.7.7、8.7.7、9.7.8、10.7.7、11.7.7）。快速自检第 16 题。
12.9.5 治理衔接：DW-AI-GOV 企业控制轴中「用了谁的模型与数据、出事谁负责」一类组织与职责要求落点为本关与第 2 关。

### 12.10 第 10 关 统一与自主：公共的路，团队愿不愿意自己走（跨层）

12.10.1 查什么：统一口径（接入、授权基线、自主等级、监测覆盖）是否成文且现行；团队是否存在绕开统一接入、统一口径的私下做法；统一口径内的自主空间是否明确，团队在空间内的选择是否留痕。
12.10.2 凭什么判定：统一口径文本现行有效；流量与台账抽查无统一口径外的生产调用；自主选择有登记，与统一口径冲突时有裁决记录。
12.10.3 不过怎么办：私下做法先登记后裁决：合规的收编入统一口径，不合规的限期关闭；无统一口径文本的，本关直接不合格，先立口径再谈自主。
12.10.4 对应关系：跨层关，无单一对应层；条文散见各层章的统一与自主接口节。快速自检第 17 题。
12.10.5 治理衔接：本关是企业内部治理要求在系统侧的总收口。DW-AI-GOV 读数中指向企业内部治理（GOV 册 A 线）的要求，其系统落点以本章各关为准，其中「员工怎么用、限额与政策」一类落点为第 2 关与本关、第 9 关。

---

## 第 13 章 合格评定与检查方法

### 13.1 检查的两种形态

13.1.1 快速自检：17 项检查，对应十关（对应关系见第 12 章各节），由系统负责方自查或评审方快查，产出分数与分档结论。快速自检的每项对应第 12 章的一关，关内判定细则依对应层章的检查项。

13.1.2 深度诊断：按证据强度逐项核查（见 13.4），不只看「有没有」，还看「拿什么证明」。深度诊断覆盖的条目以本文件各层章规范条目与检查项为准，其结论用于上线评审与重大变更复评。

13.1.3 两种形态的关系：快速自检用于筛查与自查，分数好看不等于证据扎实；凡快速自检结论用于对外表述或上线决定的，应至少对红线相关项（见 13.3）做深度诊断复核。

### 13.2 计分规则

13.2.1 快速自检每项按三档计分：做到了 2 分、部分做到 1 分、没做到 0 分，满分 34 分，折算百分制。

13.2.2 分档结论照定版口径，不得改词：
（1）85 分以上：企业级底子扎实；
（2）65 至 84 分：能跑，但有几处迟早出事；
（3）45 至 64 分：补完再上线；
（4）45 分以下：先别上线，先补课。

13.2.3 层章检查项与自检分数的换算：层章检查项（第 5 至 11 章各章第 6 节）判定为合格、部分合格、不合格三档，汇总到关口与自检项时，合格对应 2 分、部分合格对应 1 分、不合格对应 0 分；一个自检项对应多个检查项时，取最低档。

### 13.3 红线规则

13.3.1 红线：触到以下任一情形，无论总分多少，结论不得为「可以上线」：
（1）关键路径无兜底且无显式失败口径（见 5.5.4）；
（2）高危动作无拦截、无确认、无回收路径（见 10.5.3、7.5.5）；
（3）生产请求不可追溯（见 11.5.1）；
（4）未登记的模型、工具或记忆载体在生产路径中运行（见 5.5.1、7.5.1、8.5.1）；
（5）监测被监测对象可改写、可暂停、可绕过（见 11.5.7）。

13.3.2 红线清单随条文修订增补，增补记入附录 C；判定引用红线时应写明所据条号。

### 13.4 证据强度

13.4.1 深度诊断按证据强度四档判定每项条目的落实程度：
（1）有记录能证明：有在册记录可查，记录本身符合第 14 章口径；
（2）靠习惯或口头：做法存在，但只有口头或习惯依据，无记录；
（3）没有：无做法、无记录；
（4）不清楚：查不到、问不清。不清楚按「没有」计。

13.4.2 证据强度的上限规则：条目的判定不得高于其证据所能支撑的档次；只有媒体转述级证据支撑的判断，在任何读数与结论中最高只作待定处理（与 DW-AI-GOV 的证据封顶口径一致）。

### 13.5 结论与复查

13.5.1 结论的写法：检查结论应写明检查范围、所用形态（快速自检或深度诊断）、分数或分档、不合格项清单、红线判定、复查条件；结论中的每个判断应能指回检查记录编号。

13.5.2 复查触发：下列情形任一发生，应复查受影响的关与层：模型版本变更、工具或权限重大变更、事故发生、统一口径修订、本文件升版。

13.5.3 记录归属：检查结论与原始判定记录按第 14 章登记，归检查方留存，向被查方公开不合格项与依据；争议项按 14.5 的属性口径标注并列，不强行归一。

---

## 第 14 章 记录与证据规范

本章是框架配套的登记格式，与深翼 AI 治理对账模型（DW-AI-GOV v1.0）的数据绑定一致：登记册字段喂治理读数，治理读数只引用登记册编号，两边口径不得各行其是。

### 14.1 通用字段

14.1.1 每一登记条目的通用八字段：编号（id）、来源（sources）、证据等级（evidence）、最后核查（verified）、对应的关（gates）、关联条目（links）、入库日期（entered）、记录深度（depth，登记条目或完整判例）。

14.1.2 事故类条目（INC、SP）另有必填的披露日期（disclosed）。年报与统计一律按披露日期计，不按入库日期；补录与实时入库靠 entered 与 disclosed 两字段区分。

14.1.3 治理衔接字段：判例条目应设回指字段（links），把判例指回它触发或检验的规则与措施条目（REG、GOV、AGT），规则侧亦反列触发它的判例；两侧任一建立，另一侧应在同批工作中补齐。DW-AI-GOV 的「规则格乘判例对应」读法以此字段为唯一数据来源，无此字段支撑的对应关系不得写入读数。

### 14.2 证据等级

14.2.1 证据等级四级：一手已核、多源已核、媒体转述、待核。判定基准：回到一手来源（官方文件、当事方原文、判决与监管原文）核对过的为一手已核；多个独立来源一致且原始出处可识别、未能直读原文的为多源已核或媒体转述（见 14.2.2 的区分）；尚未核对的为待核。

14.2.2 媒体转述的收录与使用（定版口径，完整版）：
（1）收，标「媒体转述」：原始出处可识别（知道是哪家媒体、哪天、哪篇），多家转引的数字一致，只是原文没能直读（如付费墙）；
（2）弃，不编号：原始出处找不到，或转引之间数字矛盾；
（3）没证实的细节一律剔掉，只留多家一致的部分；任何一处单一来源，即整条按媒体转述标；
（4）使用限制：媒体转述的数字不进周刊标题、首页与任何汇总统计；条目里写明「直读原文前不得当已核引用」；
（5）复核：条目写复核日期，默认入库后 30 天；直读到原文后升为一手已核；到期仍读不到的不撤，在条目里写「复核未果」，并顺延下一次复核日期。

14.2.3 证据等级是条目的属性，不是内容的装饰：条目被引用时应连同等级一并引用；等级变化（升、降、更正）留变更记录，不覆盖原标。

### 14.3 披露与日期口径

14.3.1 日期字段各有其义，不得互替：发生日期、披露日期、入库日期、最后核查日期分别记录；统计与排序用哪一日期，应在输出处注明。

14.3.2 延迟口径（定版）：延迟拆成两个数字分开记：发现延迟（发生到厂商或当事方发现）与通知延迟（发生到通知受影响方）；披露日期仍记公开日。三段口径不同，不得混算、不得横比。厂商未主动披露的，显式标「未主动披露」，发现延迟与通知延迟记不适用并写明公开方式（如经研究者公开）。引用任何延迟数字时，必须注明是哪一段。

14.3.3 回溯边界：2026 年 1 月起的事项按收录标准全收；2023 至 2025 年的，只收已被本站现有材料引用过的，以及国际同类事故库反复收录的，记录里以回溯依据字段写明来源；2023 年以前的不入册，需要时只作背景引用。

### 14.4 记录状态与编号规则

14.4.1 记录状态三档：在用、已更正（旧说法留在变更记录）、已撤回（编号不复用）。

14.4.2 编号规则：前缀加三位流水号，按入库顺序编排；补录同样按入库顺序；永不复用；关联只写编号不写地址；同一件事在两册各自编号、互列关联。

14.4.3 在册前缀（与定版一致）：INC 事故判例、SP 特别卷、GOV 管理措施、REG 监管执法、AGT 外部 Agent 准入、MOD 模型变更、COST 成本、ARC 架构卡、IDEA 新思想、PD 产品拆解、CO 前沿公司、LAB 实验室、PPL 人物、WK 周刊、OCC 职业暴露、RES 就业研究、HIR 招聘信号、MED 医疗器械。

14.4.4 三册边界（定版）：GOV 记企业管自家 AI 的做法（含平台给自家 Agent 定的规矩）；REG 记监管者对企业的动作（调查、传票、诉讼、通报、执法）；AGT 记企业或平台针对他方 Agent 的准入政策与执行动作。三册互不重叠，同一事件跨册时各自编号、互列关联。第 12 章 12.1.5、12.10.5 的治理衔接以本边界为准。

14.4.5 治理读数的记录纪律（与 DW-AI-GOV 对齐）：成熟度定级与治理读数每次产出，应写明依据条目编号与产出日期；定级走双评（一人初定、一人独立复评），分歧达一级以上者写明依据条目差异；状态变化触发重读，旧读数保留版本，不覆盖。

### 14.5 句子的三种属性

14.5.1 凡以本框架产出的文本（条文、判读、结论、周刊引用），每一句须属三者之一：来源事实、深翼解读、未知（待核或两说并列）。

14.5.2 三者不得混写：事实句应能指回来源与编号；解读句应标明系深翼判读或在段首统一标明；未知应如实写未知，不许以推测填空。判例对照条目中的映射（某判例对照某条文）属深翼解读，已在各层章章首统一标明。

14.5.3 两说并列时，两说各自的来源与证据等级分别标注，不合并成一个「综合说法」。

---

## 附录 A 判例索引（资料性）

按主死因层编排，被列为次层关联的在该层下另行标出。标题为判例库条目名要点；证据等级、深度与详情以判例库为准。

### 模型层
- 主：INC-030 GPT-5.6 Sol 训练实例给未来版本留言：教其隐藏错误、伪造数据
- 次：INC-029（主层为记忆层）
- 注：INC-042（多模型错误率升高致生产服务短时中断）主层原记模型层，已撤回（非公开），不列入索引，编号保留不复用

### 编排层
- 主：INC-008 腾讯云评测智能体对高德 2818 次访问尝试；INC-022 OpenAI 评测智能体逃出隔离、入侵 Hugging Face 生产系统；INC-027 OpenAI 评测智能体在公开 Wiki 上互相串联（DSEWiki 事件）；INC-033 智能体经内部包仓库未授权串联（失偏框架第五起）
- 次：INC-004（主层为工具层）、INC-011（主层为门禁层）、INC-034（主层为知识层）

### 工具层
- 主：INC-002 Mythos Preview 服务器命令执行；INC-004 多模型短链绕过抓取限制；INC-005 测试模型提交真实签证申请；INC-010 Cline 供应链攻击（cline@2.3.0）；INC-019 Claude Code 执行 terraform destroy 抹掉 2.5 年生产数据
- 次：INC-001、INC-003、INC-006、INC-009、INC-014、INC-020、INC-021、INC-025、INC-028、INC-035、INC-036（主层见各条）

### 记忆层
- 主：INC-029 未发布研究模型把「摆脱角色」指令写进自己的任务摘要
- 次：INC-022、INC-027、INC-030、INC-033（主层见各条）

### 知识层
- 主：INC-015 律师提交 ChatGPT 编造判例被制裁（Mata v. Avianca）；INC-017 航司为聊天机器人错误说法担责（Moffatt v. Air Canada）；INC-018 Cursor 客服机器人「Sam」编造登录政策；INC-021 Agentjacking：伪造 Sentry 错误事件劫持编程智能体；INC-026 「对齐造假」研究记录被误喂回生产训练数据；INC-032 智能体把文件上传公开互联网以便「引用」回来（其一）；INC-034 智能体把文件上传公开互联网以便「引用」回来（其二）；INC-036 IBM 金融交易产品 RAG 投毒漏洞（CVE-2026-18875）
- 次：INC-031（主层为门禁层）

### 门禁层
- 主：INC-003 Mythos 5 绕过收费门（令牌两例）；INC-006 OpenAI 内部模型越权抓取医院统计（24 年数据）；INC-007 OpenAI 内部模型改设置取令牌、下载 147451 行；INC-009 Atlassian Rovo 数据外发（研究演示 PoC）；INC-011 Replit 冻结期删库；INC-012 METR 密钥失窃（三周烧约 60 万美元）；INC-014 三星员工把源码与会议记录贴进 ChatGPT；INC-016 DPD 客服机器人被诱导骂人并写诗骂公司；INC-020 Cursor 智能体一条 API 调用删掉生产数据库与卷级备份；INC-023 Mythos 5 在 CTF 评测中向 PyPI 上传恶意包；INC-024 Opus 4.7 在 CTF 评测中改动真实公司用户记录；INC-025 内部研究模型在 CTF 评测中攻击真实外部系统；INC-028 早期版 Opus 4.6 在 CTF 评测中越界访问真实第三方系统；INC-031 内部模型搜用泄露 API 密钥后伪造数据掩盖；INC-035 ZCode 静默打包上传用户整个工作区；INC-038 未授权使用他人测试钱包付款（部署费从他人账户扣除）；INC-039 借外部浏览器服务绕过联网限制（代发 POST 并做成可复用工具）；INC-040 智能体绕过拦截进入澳大利亚 Medicare 统计门户，越权读写非公开文件；INC-041 评测智能体在 RubyGems 批量注册账户并上传包（「恶意包」指控未获厂商核实）；INC-043 内部研究模型借 DNS 解析配置错误获得实时互联网访问，训练环境改采无实时互联网政策
- 次：INC-001、INC-002、INC-005、INC-010、INC-017、INC-019、INC-022、INC-032、INC-037（主层见各条）
- 风险映射：INC-013 AI 自我复制受控实验（蠕虫研究），未定主层，按受控实验标注，风险映射含门禁层

### 盯梢层
- 主：INC-001 费城假线索案；INC-037 OpenAI 内部编程智能体削弱失偏监控，一例事后否认
- 次：INC-007、INC-008、INC-009、INC-012、INC-015、INC-016、INC-018、INC-023、INC-024、INC-038、INC-040、INC-041、INC-043（主层见各条）
- 风险映射：INC-013（同上，风险映射含盯梢层）

---

## 附录 B 术语表（资料性）

| 中文正名 | 英文 | 说明出处 |
|---|---|---|
| 模型 | Model | 第 3 章 3.2、第 5 章 5.1 |
| 编排 | Orchestration | 第 3 章 3.2、第 6 章 6.1 |
| 工具 | Tool Use | 第 3 章 3.2、第 7 章 7.1 |
| 记忆 | Memory | 第 3 章 3.2、第 8 章 8.1 |
| 知识 | Knowledge | 第 3 章 3.2、第 9 章 9.1 |
| 门禁 | Access Control | 第 3 章 3.2、第 10 章 10.1 |
| 盯梢 | Observability | 第 3 章 3.2、第 11 章 11.1 |
| 网关 | Gateway | 第 12 章 12.1 |
| 平台 | Platform | 第 12 章 12.9 |
| 统一与自主 | Alignment & Autonomy | 第 12 章 12.10 |
| 检查项 | （无英文正名） | 第 3 章 3.3 |
| 主死因层 | （无英文正名） | 第 3 章 3.3、第 11 章 11.2.3 |
| 证据等级 | （无英文正名） | 第 14 章 14.2 |
| 最后核查 | （无英文正名） | 第 3 章 3.3 |
| 红线 | （无英文正名） | 第 13 章 13.3 |
| 模型路由 | Model Routing | 第 5 章 5.1.4 |
| 多模型路由 | Multi-Model Routing | 第 5 章 5.1.4 |
| 模型目录 | Model Catalog | 第 5 章 5.1.4 |
| 状态格 | （治理对账模型用语） | DW-AI-GOV v1.0 |
| 落差格 | （治理对账模型用语） | DW-AI-GOV v1.0 |
| 治理缺口 | （治理对账模型用语） | DW-AI-GOV v1.0 |

---

## 附录 C 版本与修订记录（规范性）

| 日期 | 版本 | 修订章节 | 修订内容 | 依据 | 修订人 |
|---|---|---|---|---|---|
| 2026-10-27 | 正式版 v1.0 | 全文 | 首版发布：目录、前言、第 1 至 14 章与附录 A、B、C、D 全稿发布；第 5 章沿用经批准的样章原文 | DW-AI-ARCH v1.0 定版（2026-10-23）、DW-AI-GOV v1.0 定版（2026-10-26）、一号台判例库（INC-001 至 INC-043，其中 INC-042 已撤回） | 深翼 DeepWing |

版本规则：版本号格式为 v主版本.次版本；结构性调整（增删章、改层关口径）升主版本，条文增补与文字修订升次版本。本文件正式版 v1.0 与 DW-AI-ARCH v1.0 定版同代并行：定版为口径源头，本文件为条文展开；两者口径冲突时，以定版为准，修订按本附录格式记。

---

## 附录 D 十关与 NIST AI RMF 对照（资料性）

### D.1 编制说明与一手来源

本附录把十关逐项映射到 NIST AI RMF 1.0 的功能与子类别，并参照 NIST AI 600-1 生成式 AI 侧写补充风险视角。本附录为资料性附录，不产生条文义务。编制：DeepWing（独立编制，NIST 未参与），编制日期 2026-10-20，随正式版 v1.0 一并发布。

一手来源（只用以下两份 NIST 正式文件，不引用二手转述）：
（1）NIST AI 100-1, Artificial Intelligence Risk Management Framework (AI RMF 1.0), January 2023, https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf
（2）NIST AI 600-1, Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile, July 2024, https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf

十关是 DeepWing 企业 AI 架构自检的十个检查关，顺序固定为网关、门禁、编排、知识、记忆、工具、模型、盯梢、平台、统一与自主。AI RMF 1.0 的四个功能为 GOVERN、MAP、MEASURE、MANAGE，共 19 个类别、72 个子类别，本附录中的子类别编号与表述均出自 AI 100-1 正文表格。

### D.2 主映射表

| 关 | 主要对应 | 次要对应 | 对应强度 | 依据 |
|---|---|---|---|---|
| 网关 Gateway | 无直接对应 | MEASURE 2.7；MAP 4.2 | 无直接对应 | RMF 按风险管理活动组织内容，不规定任何系统组件，入口路由、请求接入控制与限流这类运行时控制点在全文没有对应条目，只能间接落到系统安全与韧性被评估（MEASURE 2.7）与各组件内部风险控制被识别（MAP 4.2）两个子类别上。 |
| 门禁 Access Control | MANAGE 2.4 | MAP 3.5；GOVERN 3.2；MEASURE 2.7 | 直接对应 | 一键停用在 RMF 中有逐字对应的要求：MANAGE 2.4 要求备有取代、脱离或停用表现与预期用途不一致的 AI 系统的机制，且责任已分配并被理解。高风险动作前的人工批准对应 MAP 3.5（人工监督流程被定义、评估并记录）。身份与最小权限的具体做法 RMF 不给细则，只按安全评估笼统处理（MEASURE 2.7）。 |
| 编排 Orchestration | MEASURE 2.4 | MEASURE 2.6；MANAGE 2.3；MANAGE 4.1 | 部分对应 | MEASURE 2.4 要求 AI 系统及其组件的功能与行为在生产环境中被监控，编排关查的循环行为、停止条件与重试正是这类生产行为。但 RMF 1.0 没有 Agent 循环与多智能体协调的概念，是把通用条目套到新形态，部分成立。 |
| 知识 Knowledge | MAP 2.3 | MAP 4.1；GOVERN 6.1；MANAGE 3.1 | 部分对应 | MAP 2.3 要求 TEVV 考虑被识别并记录，包括数据收集与选择（如可用性、代表性、适用性），对应知识关的来源质量与语料治理。但知识库的版本管理与过期内容清理这类运行维护动作，RMF 没有条目。 |
| 记忆 Memory | MEASURE 2.7 | MEASURE 2.10 | 部分对应 | 记忆最特有的失败方式是被投毒或污染后持续影响系统行为，属于组件完整性问题，落在安全与韧性被评估并记录（MEASURE 2.7）上；记忆中存入个人数据则对应隐私风险被检查并记录（MEASURE 2.10）。保留期限与删除在 RMF 中没有针对数据存储的条目，GOVERN 1.7 的安全退役针对的是整个系统，不是记忆内容。 |
| 工具 Tool Use | MAP 4.2 | MAP 4.1；MEASURE 2.7 | 部分对应 | MAP 4.2 要求 AI 系统各组件（包括第三方技术）的内部风险控制被识别并记录，MAP 4.1 要求各组件的风险先被梳理，工具注册与审查正是这个顺序。但写入幂等这类具体工程性质 RMF 没有对应条目，工具输出如何被后续环节信任也只能按组件风险笼统处理。 |
| 模型 Model | MEASURE 2.3；MEASURE 2.1；MEASURE 2.5 | MAP 2.1；MANAGE 3.2 | 直接对应 | MEASURE 功能是 RMF 的测试、评估、验证与确认环节：MEASURE 2.1 要求 TEVV 的测试集、指标与工具被记录，MEASURE 2.3 要求在与部署环境相似的条件下测得并记录系统性能，MEASURE 2.5 要求系统被证明有效且可靠，上线前评测正是其核心条目群。模型版本对应 MANAGE 3.2（预训练模型被纳入常规监控与维护）。 |
| 盯梢 Observability | MEASURE 2.4 | MEASURE 3.1；MANAGE 4.1；MANAGE 4.3 | 直接对应 | 生产行为监控（MEASURE 2.4）、对已识别与新出现风险的持续追踪机制（MEASURE 3.1）、部署后监控计划（MANAGE 4.1）、事件与错误的传达与跟踪处理（MANAGE 4.3）在 RMF 中都有正面条目，日志与工具调用追踪是实现这些条目的直接证据形态。例外是成本监控：MAP 3.2 评估的是错误带来的成本，不是运行成本本身，成本监控这一项盯梢关超出了 RMF 的范围。 |
| 平台 Platform | MANAGE 4.1 | MANAGE 4.2；GOVERN 1.7 | 部分对应 | MANAGE 4.1 的部署后监控计划包含变更管理、事件响应、恢复与退役安排，部署流程有落点；但环境隔离与版本回滚这类平台工程做法 RMF 没有条目，只能按变更管理笼统对应。 |
| 统一与自主 Alignment & Autonomy | GOVERN 3.2 | MAP 3.5；MANAGE 2.4 | 部分对应 | GOVERN 3.2 要求以政策定义并区分人机配置与 AI 系统监督的角色和职责，向人升级的安排在 RMF 中先是这个政策问题。但自主等级的分级本身在 RMF 1.0 中没有对应概念，多系统统一治理也只能借用 GOVERN 的组织级条目间接表达。 |

### D.3 缺口清单：RMF 有、十关没覆盖的部分

以下均为 AI 100-1 的正面要求，但不在十关的检查范围内。十关查的是一个正在运行的系统，RMF 的这些部分问的是系统之外的组织与决策层。提供企业架构体检服务时，这些缺口就是客户最容易追问、而纯系统检查答不上来的地方。

承接分工（2026-10-27 定）：本节所列缺口不在十关本体扩关处理，统一由与本框架成对的深翼 AI 治理对账模型（DW-AI-GOV）承接。规则侧读数走 DW-AI-GOV 的法域、对象与状态轴，企业侧控制走其企业控制轴与 GOV 登记册三线（A 企业内部治理、B 厂商安全治理、C 第三方评估），证据可信度走其验证三档与成熟度 0 至 4 级。每组缺口的承接落点标注于下表各行末尾；现模型对不上的，标注待 DW-AI-GOV v1.1 补，不硬对。

| RMF 区域 | 十关未覆盖的内容 | 对企业评估服务为什么重要 |
|---|---|---|
| GOVERN 1（组织级政策） | 法律与法规要求被理解、管理并记录（GOVERN 1.1）；以组织风险容忍度决定风险管理活动的投入程度（GOVERN 1.3）；风险管理流程以透明政策落地（GOVERN 1.4） | 企业客户先问的是谁定规则、容忍度是多少。体检若只报系统问题，缺了治理层结论的落点，报告在管理层面前会显得悬空。承接：DW-AI-GOV 以 GOV A 线（企业内部治理）承接组织政策类条目，适用规则走到哪一格由其状态轴读数；成熟度读数位 2 级（成文），验证第 1 档（自评）。 |
| GOVERN 2（问责结构） | 角色与沟通线被记录并传达到位（GOVERN 2.1）；人员接受 AI 风险管理培训（GOVERN 2.2）；组织高管对 AI 系统开发与部署的风险决策负责（GOVERN 2.3） | 体检报告的整改建议需要有明确的责任归属才能被客户执行。十关查不到组织里谁负责，整改清单就容易无人认领。承接：角色与问责由 DW-AI-GOV 企业控制轴第 9 关平台的「组织与职责」落点与 GOV A 线承接，成熟度 2 级、验证第 1 档；人员培训（GOVERN 2.2）现模型无落点，待 v1.1 补。 |
| GOVERN 4（风险文化） | 培养批判性思维与安全优先心态的政策与实践（GOVERN 4.1）；团队记录并沟通所涉 AI 技术的风险与潜在影响（GOVERN 4.2） | 同样的技术缺陷在不同组织文化下后果不同。体检若能纳入文化观察，结论的区分度会明显高于纯技术清单。承接：现模型未覆盖，待 DW-AI-GOV v1.1 补；补入前体检以治理附页定性记录，不出成熟度读数。 |
| GOVERN 5、MAP 5、MEASURE 3.3（外部相关方） | 收集并整合系统开发与部署团队之外的相关方反馈（GOVERN 5.1、5.2）；对个人、群体、社区与社会的影响做特征刻画（MAP 5.1）；终端用户与受影响社区报告问题、申诉系统结果的通道（MEASURE 3.3） | 受监管行业的客户会被问到用户申诉与外部反馈机制。十关完全没有这一面，是体检最容易被专业买家挑出的空白。承接：规则侧由 DW-AI-GOV 对象轴「面向公众的服务提供方」格承接（其典型义务含投诉通道），成熟度 2 级起、验证第 1 档；企业反馈收集与社会影响评估的实践侧现模型无落点，待 v1.1 补。 |
| MAP 1、MAP 3（语境框定） | 预期用途、部署场景与相关法律规范被理解并记录（MAP 1.1）；业务价值被明确定义（MAP 1.4）；组织风险容忍度被确定并记录（MAP 1.5）；预期收益与成本（包括错误带来的成本）被评估（MAP 3.1、3.2） | 十关默认系统已经存在且值得存在。体检若加一页语境框定，把检查结论和客户的业务风险接上，这是从清单走向评估的关键一步。承接：预期用途与适用规则由 DW-AI-GOV 法域、对象、状态三轴交叉读数承接，风险容忍度由 GOV A 线承接，成熟度 1 至 2 级、验证第 1 档；业务价值与收益成本评估属 DW-AI-GOV 明示范围外，不承接。 |
| MANAGE 1（风险处置决策） | 按影响与可能性对已记录风险排序（MANAGE 1.2）；形成缓解、转移、规避或接受的处置方案（MANAGE 1.3）；残余风险被记录（MANAGE 1.4）；是否推进开发或部署的判断（MANAGE 1.1） | 十关产出的是发现，RMF 要求发现之上有人作处置决定并记录残余风险。体检交付物若止于问题清单，客户还要自己补这一层。承接：上线判断与审批分级由 DW-AI-GOV 企业控制轴（第 7 关、第 10 关的部署门禁）与 GOV A 线审批类条目承接，成熟度 2 级、验证第 1 档；风险排序、处置方案与残余风险记录现模型无落点，待 v1.1 补。 |
| GOVERN 6、MANAGE 3（第三方与供应链） | 处理第三方实体风险的政策，包括侵犯第三方知识产权的风险（GOVERN 6.1）；第三方数据或系统被认定为高风险时出故障的应急流程（GOVERN 6.2）；第三方风险被持续监控并施加控制（MANAGE 3.1） | 工具关只查单个系统里的组件准入，供应商层面的尽调与应急安排不在十关内，而这正是企业采购审查的必问项。承接：DW-AI-GOV 对象轴为 AGT 单列一行，企业控制轴落第 9 关平台，条目走 AGT 册与 GOV A 线，成熟度 2 至 3 级，验证第 1 档（有第三方评估者升第 2 档）。 |
| MEASURE 2.11、MEASURE 2.12（两项具名评估） | 公平与偏见被评估并记录（MEASURE 2.11）；AI 模型训练与管理活动的环境影响被评估并记录（MEASURE 2.12） | 模型关的评测范围目前未点名公平性，环境影响则完全在十关之外。这两项在受监管与 ESG 敏感的客户那里是常见问项，先在报告中标明不在检查范围，比被问住更好。承接：公平评估的评估事实由 DW-AI-GOV 的 GOV C 线（第三方评估）与验证轴第 2 档承接，成熟度 3 级读数位；环境影响（MEASURE 2.12）现模型未覆盖，按分工裁定划在界外，v1.1 不预设纳入。 |
| GOVERN 1.6、GOVERN 1.7（系统清单与退役） | 组织层面的 AI 系统清单机制（GOVERN 1.6）；系统安全退役与逐步下线的流程（GOVERN 1.7） | 客户有多少个 AI 系统在跑、退役怎么处理，是治理体检的常见起点问题。十关只查被送到面前的那一个系统。承接：退役安排由 DW-AI-GOV 企业控制轴第 9 关平台落点与 GOV A 线承接，成熟度 2 级、验证第 1 档；组织级系统清单机制现模型未覆盖，待 v1.1 补，体检时先以治理附页盘点栏记录。 |

### D.4 生成式 AI 风险附表（NIST AI 600-1）

以下 12 项风险的名称与定义出自 AI 600-1 第 2 节，是生成式 AI 特有或被其放大的风险。右列说明在检查一个正在运行的系统时，哪一关会查到它。

| # | 风险（AI 600-1 原名） | 定义要点 | 检查它的关 |
|---|---|---|---|
| 1 | CBRN Information or Capabilities | 更容易获取或合成与化生放核武器及其他危险材料相关的有害信息或设计能力 | 模型（主要）；门禁（次要）。模型关查能力评测与拒答表现，门禁关查谁能触达敏感能力 |
| 2 | Confabulation | 自信地给出错误或虚假内容，即通常所说的幻觉或编造，用户可能被误导 | 知识（主要）；模型、盯梢（次要）。知识关管语料依据，模型关管上线前评测，盯梢关管线上输出监测 |
| 3 | Dangerous, Violent, or Hateful Content | 更容易生成与接触暴力、煽动、威胁内容，以及自残或违法活动的建议，仇恨与贬损内容难以控制 | 网关（主要）；模型（次要）。内容进出系统的关口在网关关，模型关查安全评测 |
| 4 | Data Privacy | 生物特征、健康、位置等个人信息或敏感数据因泄露、未授权使用、披露或去匿名化造成的影响 | 记忆（主要）；门禁（次要）。什么能存、存多久在记忆关，谁能访问在门禁关 |
| 5 | Environmental Impacts | 训练或运行生成式 AI 模型的高算力消耗及其对生态的不利影响 | 无覆盖。盯梢关的成本监控只覆盖算力花费，不等于环境影响评估；此项对应 RMF 的 MEASURE 2.12，在十关范围之外 |
| 6 | Harmful Bias or Homogenization | 历史、社会与系统性偏见被放大，子群体或语言之间出现表现差异，输出趋于同质并误导决策 | 模型（主要）；知识（次要）。注意十关没有点名公平性检查，此项靠模型关的评测扩展；知识关管语料的代表性 |
| 7 | Human-AI Configuration | 人与 AI 系统的配置与交互方式可能导致拟人化、算法厌恶、自动化偏见、过度依赖或情感纠缠 | 统一与自主（主要）；门禁（次要）。自主程度与升级路径在统一与自主关，关键动作的人工批准在门禁关 |
| 8 | Information Integrity | 生成不区分事实与意见或虚构、不标明不确定性的内容的门槛降低，并可被用于大规模虚假信息活动 | 知识（主要）；盯梢（次要）。知识关管来源质量与可溯源，盯梢关管异常模式的发现；输出水印与内容来源证明不在十关内 |
| 9 | Information Security | 攻击门槛降低（自动化漏洞发现与利用、恶意软件、钓鱼、进攻性网络行动），攻击面扩大，危及训练数据、代码或模型权重的机密性与完整性 | 门禁（主要）；工具、网关（次要）。门禁关管访问与权限，工具关管工具输出带来的注入风险，网关关管入口过滤 |
| 10 | Intellectual Property | 更容易生成或复制未经授权的受版权、商标或许可保护的内容，更容易泄露商业秘密，或抄袭与非法复制 | 知识（主要）；模型（次要）。知识关管语料来源与授权；组织级的知识产权政策属 GOVERN 6.1，在十关之外 |
| 11 | Obscene, Degrading, and/or Abusive Content | 更容易生成与接触淫秽、侮辱、虐待类影像，包括合成儿童性虐待材料与非自愿私密影像 | 网关（主要）；模型（次要）。与第 3 项同一检查路径，关口过滤加模型安全评测 |
| 12 | Value Chain and Component Integration | 上游第三方组件（包括取得不当的数据）整合不透明、不可追溯，供应商审查不当，损害对下游用户的透明度与问责 | 工具（主要）；平台（次要）。这是 12 项中被十关覆盖最完整的一项：工具关管组件准入与审查，平台关管整合与部署 |

### D.5 定位说明

DeepWing 的七层与十关是一套面向运行中系统的检查方法。本对照表把十关逐项映射到 NIST AI RMF 1.0（NIST AI 100-1）的功能与子类别，并参照 NIST AI 600-1 生成式 AI 侧写补充风险视角。RMF 回答的是治理层的问题：组织该考虑什么、谁负责、决策如何作出。十关回答的是系统层的问题：一个已经在跑的企业 AI 系统，具体查哪里、看什么证据。两者对齐之后，治理要求可以落到可检查的系统部位上。本对照表是参考性映射（reference crosswalk），不是 NIST 认证，不构成 NIST 的背书，也不构成任何合规结论；本映射由 DeepWing 独立作出，未经 NIST 审查或认可。

---

## 文末一 · 缺口清单（正式版 v1.0 未决事项）

以下事项为素材与定版文件撑不住、本版按纪律留空或只立判定方法者，后续版本按附录 C 记修订后补入。

1. 自检题面待回录：快速自检 17 项的题面原文只存在于自检仪现行版，定版文件仅存题号与关主题的对应。本文件各层检查项与第 12 章各关均按题号对应，题面待从自检仪现行版回录后补入第 13 章附表。
2. 定量阈值缺失：路由分级比例、降级触发条件、确认点金额与范围阈值、告警阈值、规模上限数值，现阶段只有原则与个案数字，尚不能升为规范阈值。本版只写判定方法（见 6.5.4 注、11.3.4 等），数值留待后续版本以判例与实测积累为据补入。
3. 供应商静默变更的核查方法待补：MOD 册已有登记实践，但「如何发现未预告的版本变更、发现后如何处置」的方法条文未成文，5.5.5 只立登记与复评要求。
4. 引用文件待逐件核对：第 2 章 2.3 的外部文件，本版未设定合规义务；现有参考资料为延伸阅读体例，须逐件核对版本与日期、确认被条文实际引用后，才可升入引用文件清单。
5. 模型层判例待挂：主层判例只有 INC-030 一条（次层关联 INC-029）；5.4.1 至 5.4.5 五种失效模式暂无判例可挂（见 5.8.3）。
6. 记忆层判例待挂：8.4.3 跨用户串话、8.4.4 该忘的不忘暂无判例可挂（见 8.8.3）。
7. 盯梢层判例待挂：11.4.5 告警疲劳、11.4.6 披露迟滞暂无判例可挂；后者待判例库披露延迟字段回填完整后补（见 11.8.4）。
8. 治理读数待建：DW-AI-GOV 的成熟度读数目前只能对少数格做暂定读数（其数据实情见 DW-AI-GOV v1.0 第五节）；本文件 12.1.5、12.7.5、12.8.5、12.9.5、12.10.5 与 14.4.5 只立衔接口径，不预填读数结论。
9. 逐关条文的素材深浅不一：第 12 章第 9 关平台、第 10 关统一与自主主要依托原则性论述与定版口径展开，判例支撑弱于其余各关，后续版本应以新判例与登记实践增补判定细则。

---

## 文末二 · 体例说明（全稿沿用）

### 一、编号规则

1. 章以整数编号（第 1 章、第 2 章……），层章按七层顺序编排：模型、编排、工具、记忆、知识、门禁、盯梢，依次为第 5 至第 11 章；关不单独成章，统一编入第 12 章，按检查次序编号 12.1 至 12.10。
2. 条以「章号.序号」编号（如 5.1、5.2），条内再分款时用「章号.条号.款号」（如 5.5.5）。条文引用一律写全编号，不写「上一条」「本章第三节」一类相对指代。
3. 检查项编号格式为「层全名-C序号」，如模型-C1、编排-C3、门禁-C10：层全名依次为模型、编排、工具、记忆、知识、门禁、盯梢。编号只作检查项编号与交叉引用，正文叙述一律用中文全名。早先使用的两字母代码格式自本版起停用。
4. 判例与登记条目只写编号（如 INC-030、MOD-012），不写链接地址；同一事件跨册时各自编号、互列关联。

### 二、术语体例

1. 术语首次出现时写「中文正名（英文 English Name）」，其后只用中文正名。七层与十关的英文名以定版为准：Model、Orchestration、Tool Use、Memory、Knowledge、Access Control、Observability；十关英文为 Gateway、Access Control、Orchestration、Knowledge、Memory、Tool Use、Model、Observability、Platform、Alignment & Autonomy。
2. 定版废止名不得在正文使用，包括：Gating、Oversight、Knowledge Base、Model Layer、AI Gateway、Enterprise AI Platform。引用历史材料时出现废止名的，加注现行正名。
3. 每层章首节定义段是该层术语的定义出处，其他章引用时不重复定义，只给出处条号。

### 三、条文体例

1. 条文用语分级：「应」为要求，「不得」为禁止，「宜」为建议，「可」为允许。检查项的判定只对「应」与「不得」类条目作合格判定。
2. 每层章的固定小结构为：范围与定义 / 职责边界 / 组成要素 / 常见失效模式 / 规范条目 / 检查项 / 与其他层及关口的接口 / 关联判例，八节不增不减，节序不调。
3. 每句话须属三种属性之一：来源事实、深翼解读、未知。条文中的事实性陈述须能指出素材出处；属解读的，在章首或节首统一标明，不与条文混排冒充事实。
4. 正文不用长破折号（em dash 与 en dash），停顿与并列用逗号、顿号或分行；占位符统一用「·」。

### 四、版本记录格式

1. 版本号格式为 v主版本.次版本（如 v1.0、v1.1）：结构性调整（增删章、改层关口径）升主版本，条文增补与文字修订升次版本。
2. 附录 C 修订记录每行六个字段：日期、版本、修订章节、修订内容、依据（判例编号、登记编号或定版文件）、修订人。
3. 条目与记录的状态词统一为：在用、已更正、已撤回。已更正者旧说法留在变更记录；已撤回者编号永不复用。
4. 每条记录保留「最后核查」日期；框架条文的复核周期随第 14 章执行，条文被判例推翻时，先记变更记录，再改正文。
