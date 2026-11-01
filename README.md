# DeepWing

Independent AI intelligence and research platform.
独立 AI 情报与研究平台。

DeepWing tracks AI from promise to reality: it records the technology as it evolves, verifies corporate promises against primary sources, analyses deployment results, and follows up on what was claimed until the outcome is known. The canonical home of everything in this repository is the website, [deepwingai.com](https://deepwingai.com). This repository is the public mirror for citation and reuse: framework text, public register data, and version history.

DeepWing runs three intelligence desks under one verification standard:

- Desk 1: enterprise AI architecture （一号台：企业 AI 架构）
- Desk 2: AI jobs and careers （二号台：AI 就业与职业）
- Desk 3: medical AI （三号台：医疗 AI）

A shared method layer sits across the desks: evidence grading, source verification, promise tracking, and reconciliation of claims against outcomes.

## What this repository contains

- `framework/`: the full text of DW-AI-ARCH, the DeepWing Framework formal edition: seven layers and ten gates for enterprise AI systems, 385 numbered clauses and 70 check items.
- `data/`: public register data exported from the website registers, in CSV. The first export is the Desk 1 incident case register (public set). See `data/README.md` for fields, sources, and update cadence.
- `CHANGELOG.md`: the version history of this repository and of the assets it mirrors.
- `LICENSE`: CC BY 4.0.

## How to cite

Framework: DeepWing. DW-AI-ARCH: A Seven-Layer, Ten-Gate Framework for Enterprise AI, Formal Edition v1.0. 2026. Deposit copy: Zenodo, DOI [10.5281/zenodo.23715226](https://doi.org/10.5281/zenodo.23715226).

Register data: cite the register and the entry ID as shown on the website, for example "DeepWing, Desk 1 Incident Case Register, INC-001, deepwingai.com/cases". Entry IDs in this repository are the public IDs of the website register.

## Evidence grades

Every register entry carries one of four evidence grades, shown on the website in Chinese and English:

- Primary-source verified （一手已核）: the claim was checked against the primary source itself.
- Multi-source verified （多源已核）: independent sources agree and were cross-checked.
- Media-reported （媒体转述）: the claim rests on media reporting and has not been verified against a primary source.
- Pending verification （待核）: recorded, not yet verified.

## License

The contents of this repository are published under CC BY 4.0. You may reuse them with attribution to DeepWing and a link to deepwingai.com or to the DOI above.

## What is not here

This repository holds the public knowledge layer only. It does not contain, and will not contain:

- source code of the DeepWing tools (quick check, deep diagnosis, the agent-fit judge, cost tools);
- scoring logic or grading weights used by those tools;
- question-to-case mapping data;
- cost model parameters;
- unpublished working registers or candidate entries that have not passed review.

Those are product-side assets. They stay on the website, where the tools themselves are free to use.

## 中文说明

深翼 DeepWing 是独立 AI 情报与研究平台，设三个情报台（企业 AI 架构、AI 就业与职业、医疗 AI），共用一套核查标准：证据分级、来源核查、承诺追踪与对账。本仓库是网站公开层的镜像，供引用与复用：框架正式版全文、公开登记册数据与版本历史，授权为 CC BY 4.0。工具代码、计分逻辑、题目与判例映射、成本模型参数与未公开登记册不在本仓库内。

## Contact

hi@deepwingai.com
