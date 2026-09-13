---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

# Craig Hagerman

**AI/ML Engineering Manager**

Hamilton, Ontario, Canada | [linkedin.com/in/craighagerman](https://www.linkedin.com/in/craighagerman)

------

## Summary

Engineering leader who builds and runs AI/ML teams. Eleven-plus years shipping production machine learning, NLP, and generative AI systems, and roughly six years leading engineering and data science teams across four organizations. I have built an AI function from zero twice, run two simultaneous cross-functional product teams twice, and led distributed teams across four countries.

My work sits at the point where team leadership and technical judgment meet. I hire the team, set the architecture and the quality bar, hold the delivery commitment, and stay close enough to the system to make the hard technical calls and to unblock engineers when they are stuck. I do not carry feature tickets; I own design decisions, review code and architecture, remove obstacles, and represent the work to executives.

Recent focus is production multi-agent LLM systems - orchestration, retrieval, agentic tooling, and evaluation - delivered under real safety, privacy, and regulatory constraints. Recurring pattern across my career: enter a domain I do not know (health, retail, media, fintech, defense), build or inherit a team, and get a system into production.

------

## Leadership Scope at a Glance

| Organization                 | Role                                       | Leadership scope                                             |
| ---------------------------- | ------------------------------------------ | ------------------------------------------------------------ |
| Loblaw Digital               | Engineering Manager, AI/ML                 | Built a cross-functional team from zero to roughly 12 (AI/ML, data, backend, frontend, product, design), including a core AI engineering team of 3. Reports to the SVP of Engineering. Primary technical point of contact for a board-priority initiative. |
| Jobscan                      | Head of AI                                 | Led a new AI/ML function as its first leader. Directed 4 engineers (2 AI engineers plus 2 part-time backend developers). Reported directly to the owner with weekly AI strategy 1:1s. |
| Exchange Solutions           | Director of Engineering, Data Science & ML | Hired, managed, and mentored a team of data scientists, data engineers, and analysts across two simultaneous cross-functional product teams. Distributed across Toronto, Calgary, India, and Lebanon. Reported to the VP of Analytics; attended C-suite leadership meetings. |
| Uncharted Software           | Lead ML Engineer                           | Led ML methodology and data science on the commercial team. Mentored new hires and junior data scientists, interviewed data science candidates, and directed ML efforts on other teams. |
| Cornerstone Academic College | Director of Academics                      | Supervised a teaching staff of under twelve; owned curriculum design and academic operations. Non-technical, director-level people leadership. |

Roughly fifteen years of teaching and university lecturing sits underneath all of this - self-directed curriculum and project ownership, supervising teaching assistants, budget management, and a long habit of explaining difficult technical material to people who do not share my background.

------

## Leadership Philosophy

### How I manage

Collaborative and democratic, with a strong mentoring streak and a clear point of view about where the work is going. I consult the team on direction so their voices genuinely shape it, then hold the line on the decision once it is made. My aim is a team where competent, low-ego people have room to do their best work and know exactly what "good" looks like.

In practice that means:

- **Regular, two-way 1:1s.** Open-ended questions rather than status recitals. "What is one thing that would make your work easier?" surfaces more than any dashboard.
- **Clear expectations, stated out loud.** Transparency about priorities, deadlines, and how decisions get made. When priorities change, I explain why - unexplained change is the main source of team anxiety.
- **Modelled vulnerability.** I say when I do not know something, admit mistakes and what I learned, and bring the team into finding the answer. A manager who is never wrong produces engineers who hide problems.
- **Blameless problem-solving.** Code review is about the code. Post-mortems are about the system. Recognition is public and covers collaborative contributions, not just individual heroics.

### Radical candor, not comfortable silence

Care personally and challenge directly. Honest, constructive guidance beats praise that costs nothing, and I ask the team to give me the same in return. The failure mode I watch for in myself is being warm at the expense of being clear, so I try to name a problem the first time I see it rather than the third.

### Trust but verify

Hire competent people, align on the goal, and give them room. Trust is granted in increments and earned with evidence - both technical skill and team play. Scope and autonomy expand as people demonstrate they can carry them, which also means I notice early when they cannot.

### Hiring and the talent bar

Building a team from zero at Loblaw Digital, hiring into an existing team at Exchange Solutions, and interviewing data science candidates at Uncharted have given me a consistent view that the bar is a technical judgment call that the hiring manager has to personally own. It cannot be delegated to a rubric. I look for demonstrated production delivery over credentials, evidence that a candidate can explain a decision and its tradeoffs, and low-ego in a working session. A strong interview conversation is not a hiring signal on its own.

### Team enablement, not just mentoring

Individual mentoring matters, but capability has to spread wider than a 1:1. Things I have actually done for team-wide uplift:

- Co-designed a shared internal AI assistant scaffold at Loblaw Digital - a common service, orchestration, and CI baseline - now adopted by several internal AI teams, turning one team's architecture into org-level leverage.
- Founded and led a monthly cross-organization AI roundtable at Jobscan, deliberately extending beyond the engineering team.
- Started and ran a machine learning reading group and data science reading club at Uncharted, plus internal tutorials and onboarding recipe books for the ML pipeline.
- Ran lunch-and-learns and internal technical talks on deep learning for NLP, explainable AI, AutoML, and topic modeling.

### Just enough structure

I like OKRs for surfacing long-term goals. I believe agile ceremony should unblock developers rather than perform progress, so I adapt the process to the team - fewer standups, no-meeting blocks - rather than running rituals for their own sake. Bias for action: if something needs doing, do it or raise it, and I expect the same.

------

## Experience

### Loblaw Digital - Engineering Manager, AI/ML

| **Oct 2025 - Present** | Toronto (Remote) | Health tech and retail media |

Hired to stand up and lead a new AI engineering team for a board-priority conversational AI initiative in the company's pharmacy business, reporting directly to the SVP of Engineering. Loblaw Digital is enterprise-scale but operates with startup pace and aggressive deadlines.

**Team and delivery leadership**

- Built the cross-functional team from zero to roughly twelve people spanning AI/ML, data, backend, frontend, product, and design, including a core AI engineering team of three. Owned hiring, technical direction, and delivery accountability.
- Took the assistant from kickoff to a security-tested, code-frozen MVP in roughly one quarter, in a regulated healthcare context with a security review gate.
- Served as primary technical point of contact for the initiative: weekly touchpoints with senior vice presidents and directors, with board updates flowing through the director of strategy.
- Led a second AI initiative in parallel - a retail-media analytics assistant for advertisers and vendors - delivered to production-ready in under four months on the shared internal platform scaffold.
- Stayed hands-on where a manager should be: architecture and design ownership, design and code review, and clearing infrastructure, CI/CD, and deployment blockers for the team rather than carrying feature work myself.
- Co-designed the shared internal AI assistant scaffold now adopted across several internal AI teams, establishing common patterns for service structure, agent orchestration, and CI/CD.

**Technical direction**

- Set the architecture: a multi-agent orchestration graph on a supervisor-worker pattern spanning a dozen-plus clinical domains, with three distinct flow types - standard retrieval-augmented generation, multi-intent execution with dependency-aware parallelism, and an iterative tool-reasoning loop. Chose this over a single iterative-reasoning design to hold latency and answer depth for the common multi-part question.
- Owned the safety posture for a regulated healthcare product: a no-model semantic crisis prefilter on the fast path, model-based safety verification at medium confidence, content moderation with provider fallback, deterministic routing, and clinically verified static responses for hard-stop cases.
- Enforced protected health information and personal data controls at the service boundary, with masking on observability paths and consent-gated access to sensitive records before the agent ever sees them.
- Directed a hybrid retrieval layer combining keyword and dense vector search with reranking and query-type routing, over hundreds of ingested clinical sources, with inline citations validated against the generated response.
- Established the quality bar with an offline evaluation harness covering node-level metrics, model-as-judge scoring, and end-to-end faithfulness testing, and set a factual-accuracy release gate meaningfully above the published domain baseline, which the team met before release.
- Kept all safety-critical logic in the retail-media assistant deterministic - tool selection, data guardrails, query-pattern blocking, and organization-level access control - with the language model generating prose only and never controlling data access. Expanded its analytics tool layer across three phased releases.

### Jobscan - Head of AI

| **Feb 2024 - Aug 2025** | Seattle (Remote) | HR and careers SaaS |

Led the company's AI and ML function, reporting directly to the owner with weekly AI strategy 1:1s. Player-coach: began as functional lead and grew into directing four engineers.

- Built a new AI/ML function that the CEO publicly credited, at a quarterly all-hands, as a key driver of the company's year-over-year revenue growth.
- Contributed to an estimated 8 to 10 percent improvement in user retention over the period.
- Owned the strategic pivot from bespoke in-house models to an LLM-first, agentic roadmap, and served as the internal technical arbitrator on AI direction.
- Founded and led a monthly cross-organization AI roundtable to raise AI fluency outside the engineering team.
- Stayed technically hands-on: built a resume-to-job semantic search engine solo using embeddings and a vector database; stood up an in-house model server to reduce third-party API dependence for selected workloads; fine-tuned encoder models and built sequence-to-sequence document parsing models; built a horizontally scaling document parser and a multi-turn career-coach assistant.

### Exchange Solutions - Director of Engineering, Data Science & Machine Learning

| **Sep 2021 - Dec 2023 | Toronto | Retail loyalty and personalization SaaS |

Directed data science and machine learning for a retail loyalty personalization business. Hired, managed, and mentored a team of data scientists, data engineers, and analysts as a hands-on player-coach across two simultaneous cross-functional product teams, each with its own product and client partners.

- Led a distributed team across Toronto, Calgary, India, and Lebanon, coordinating across time zones and contract structures.
- Reported to the VP of Analytics with weekly touchpoints with the VP of Product and the CTO, and attended C-suite leadership meetings.
- Served as technical lead on weekly client and account-manager calls for both products - answering technical questions, gathering feedback, and turning it into roadmap.
- Re-architected the batch offer personalization product, serving roughly one million loyalty members, from a SQL-only pipeline to a modular Python pipeline on AWS, replacing bespoke sort functions with an ensemble scoring engine over vectorized offer and customer attributes. Offer completion and attributed revenue rose by a few percentage points.
- Cut a core batch job from six to ten hours in Snowflake to roughly ten minutes by re-architecting it as a parallelized AWS pipeline, reducing per-run processing cost to tens of dollars.
- Rebuilt the real-time e-commerce personalization product as a modular, A/B-tested pipeline with multi-arm bandit experimentation, moving from static business rules toward real-time inference and improving average order value by roughly five percent.
- Built a transformer sequence model to predict a customer's next interaction and likely next purchase, and delivered a generative AI self-serve client portal producing grounded natural-language answers, charts, and narrative from natural-language questions.

### Uncharted Software - Lead ML Engineer & Data Science Consultant

| **Jan 2019 - Aug 2021** | Toronto | Enterprise SaaS, CRM, fintech |

Led ML methodology and data science on the commercial team across a portfolio of enterprise engagements. Six years total at Uncharted across its research and commercial phases.

- Mentored new hires and junior data scientists, interviewed data science candidates, ran ML and DS reading groups and internal tutorials, and consulted on and directed ML efforts for other teams.
- Built the machine learning engine powering an enterprise customer-experience platform on Spark and Databricks: customer journey analytics, intent classification, real-time interaction management, and journey orchestration. The platform held Forrester Wave Leader status three years running, and the vendor was acquired by Medallia for more than $300M in 2022.
- Delivered bespoke ML and data-strategy engagements for more than twenty enterprise clients including Bloomberg, Fidelity, Cigna, Infor, Refinitiv, RBC, Scotiabank, Payments Canada, and the British Columbia Securities Commission.
- Led client-facing pre-sales, RFP presentations, workshops, and project kickoffs, with weekly touchpoints with a client CTO and Chief Solutions Officer and quarterly in-person sessions.
- Worked fully remote across Eastern and UK time zones for the duration.

### Uncharted Software - NLP / Software Engineer (Research)

| **Jan 2015 - Jan 2019** | Toronto | DARPA and government research |

- Data scientist and algorithm designer on DARPA programs including XData, QCR, TellFinder, and Provenant, later supervising other researchers on the program.
- Built multilingual social-media text analytics, custom NLP classifiers, and a novel non-parametric topic-modeling approach for signal generation and crisis nowcasting.
- Built high-throughput social-firehose parsing and TensorFlow sentiment and topic-modeling pipelines supporting government and law-enforcement analytics.
- Multilingual NLP work spanning Arabic and Russian morphological analysis, transliteration and lemmatization, sentiment lexicon induction, entity detection and disambiguation, and query expansion served through a GoLang API.

### Wattpad - Research Scientist, NLP (Industy Internship)

| **May 2014 - Dec 2014** | Toronto | Consumer social and media |

- Built a story recommendation engine with Kafka integration in the recommendation pipeline, plus writing-style and reading-level similarity models and a concept knowledge graph assembled from Wikipedia and Freebase.
- Researched long-tail and cold-start recommendation problems. Reader engagement and click-through improved.

------

## Selected Case Studies

### Conversational healthcare AI assistant (Loblaw Digital)

**Problem.** Deliver a consumer-facing health assistant inside a national pharmacy retailer's digital product, where a wrong answer is a clinical risk and the data involved is protected health information.

**Approach.** A multi-agent orchestration graph on a supervisor-worker pattern, with distinct flow types for simple retrieval questions, multi-part questions with dependencies between them, and questions requiring iterative tool reasoning. Safety was designed as layers rather than a single filter: a fast deterministic prefilter, model-based verification only where the signal was ambiguous, content moderation, and clinically verified static responses for crisis cases. Privacy was enforced at the service boundary rather than inside the agent.

**Result.** Kickoff to initial MVP in roughly one quarter with a core engineering team of four inside a cross-functional group of about twelve. The evaluation harness and release gate built alongside it became the team's quality mechanism, and the underlying service scaffold was adopted by several other internal AI teams.

**My role.** Engineering manager. Team build, hiring, architecture ownership and review, delivery accountability, executive and board-facing communication.

### Batch offer personalization at scale (Exchange Solutions)

**Problem.** A new client needed personalized loyalty offers rather than mass campaigns: ten offers per customer per week across three optimization objectives, honoring complex business rules such as mutual exclusivity, no-repeat, repurchase cycles, and vendor-funded quotas. The existing product sorted on a single metric through a pure-SQL implementation that grew less scalable with every enhancement, with no ML inputs and eyeball-only evaluation.

**Approach.** Let SQL do aggregation and joins; move transforms, processing, and modeling into ordered Python stages. Replace bespoke sort functions with an ensemble scoring engine that turns raw attributes into engineered features and distance measures per objective, so selection methods become weight configurations rather than new code, and any input can later be upgraded to an estimator. Re-architect the batch job onto a parallelized AWS event pipeline.

**Result.** Runtime fell from six to ten hours to roughly ten minutes at tens of dollars per run. Offer completion and attributed revenue rose by a few percentage points. Vectorizing the attributes opened up distance-based and latent-similarity approaches for later iterations.

**My role.** Lead and primary architect, roughly half hands-on.

### Real-time offer personalization (Exchange Solutions)

**Problem.** Inherited an immature real-time product eight months after launch: on-premise, manually curated models that took six months or more to build, no personalization, and simplistic optimization.

**Approach.** Refactored the business-rules codebase into modular, unit-tested components, aligned direction with data science and external stakeholders, and built a phased roadmap - modular pipeline with A/B testing, then heuristics, then batch models on static data, then batch models on real-time data, then real-time inference. Added multi-arm bandit experimentation and a transformer sequence model for next-action prediction.

**Result.** More relevant offers at presentment, with suppression when no offer was warranted. Validated offline and online. Average order value improved by roughly five percent.

**My role.** Lead across the product team.

### Customer journey intelligence platform (Uncharted / enterprise CX vendor)

**Problem.** Move a customer experience platform from descriptive analytics toward predictive and prescriptive: reveal each customer's evolving intent, cluster journeys, predict goals, recommend the next action, and orchestrate across channels in real time.

**Approach.** An ML engine on Spark and Databricks: intent discovery through feature extraction and path-similarity prediction, cohort analysis using statistical tests to decide whether two customer populations genuinely differ, journey clustering research spanning probabilistic suffix trees, hidden Markov models and matrix factorization, sequence embeddings over user paths, and Markov and MDP forecasting of how many customers reach intent versus drop off. Explainable-AI visualization for the tree ensembles.

**Result.** Contributed to Forrester Wave Leader status three years running. 

**My role.** Lead, algorithm and pipeline designer, data scientist.

### Data strategy and a FinTech index (A national payment clearing and settlement infrastructure agency)

**Problem.** A modernizing national payments organization needed a data-strategy roadmap, and separately wanted an index tracking non-fiat and payments securities.

**Approach.** Stakeholder meetings, workshops, and interviews alongside data exploration, modeling, and visualization. For the index, defined the constituent securities and a rebalancing method at set intervals.

**Result.** A ranked, prioritized roadmap plus a draft data-governance framework and proposed new data products, and a hosted API through which the organization could publish the index.

**My role.** Consultant and data-strategy lead.

### Natural language generation over tabular data (large global insurance company)

**Problem.** Reduce the manual burden on analysts writing chart commentary and calling out notable data.

**Approach.** Outlier and saliency analysis feeding a ranking and selection pipeline that identifies likely-salient data points, then a natural language generation model that drafts editable auto-comments.

**Result.** Lower analyst cognitive load through a rank, select, and comment pipeline. Related peer-reviewed work followed.

**My role.** Owned the commentary and NLG portion; other teams owned UX, design, and frontend.

### Social media analytics for defense research (DARPA)

**Problem.** Gauge the radicalization potential of social media messages across several languages, understand how adversary propaganda works and how effective counter-responses are, and trace manipulation narratives in real time and at scale.

**Approach.** Multilingual sentiment analysis, topic modeling, time-series and anomaly analysis, named entity recognition, radicalization classifiers, neologism analysis, and query expansion, later extended to narrative-level analysis with tone and emotion detection, clustering, abstractive summarization, and narrative visualization.

**Result.** Tooling that let analysts see how information was being used by adversaries, identify the radicalization process and radicalized individuals, and support crisis nowcasting.

**My role.** Data scientist and algorithm designer, later supervisor.

------

## Technical Depth

**Languages.** Python, SQL, Scala. Also Java, JavaScript, R, Go.

**Generative AI and LLMs.** LangGraph, LangChain, Langfuse. Multi-agent and supervisor-worker architectures, ReAct tool-reasoning loops, multi-intent planning with dependency-aware parallel execution, function calling and tool use, structured outputs, MCP tooling. Hybrid retrieval-augmented generation combining BM25, dense vectors, and reranking. Prompt engineering. Self-hosted serving with vLLM, Hugging Face Transformers. Production model providers: GPT and Gemini.

**LLM evaluation.** Node-level evaluation, model-as-judge scoring, end-to-end faithfulness testing, tool-call regression, golden-set release gates, synthetic evaluation dataset generation.

**AI safety and privacy engineering.** Semantic crisis prefilters, content moderation, deterministic guardrails and routing, PHI and PII masking, consent-based data gating, prompt injection detection.

**Machine learning and deep learning.** PyTorch, TensorFlow, Keras, scikit-learn, Spark MLlib. Transformers and sequence models, BERT and encoder fine-tuning, sequence-to-sequence, CNNs, LSTMs, autoencoders. Random forests and ensembles, gradient boosting, clustering, matrix factorization, PCA and t-SNE. Recommendation through collaborative filtering, embedding similarity, and retrieval ranking. Reinforcement learning with Q-learning, Markov models, and MDPs. Multi-arm bandit experimentation, drift metrics and rebuild triggers, offline and online validation.

**Natural language processing.** Tokenization, embeddings, semantic search and similarity, information retrieval, document ranking, query expansion. Text and hierarchical classification, named entity recognition, entity linking, relationship and information extraction. Topic modeling including LDA, biterm, and non-parametric Bayesian approaches. Natural language generation, table-to-text, abstractive summarization, question answering. Sentiment, tone, stylometry, readability, coherence, coreference, and causality analysis. Morphology and syntax across English, Arabic, and Russian. Knowledge graphs and ontology learning.

**Data and infrastructure.** Spark, Databricks. AWS across six-plus years including S3, SQS, Kinesis, Lambda, and SageMaker. GCP including Vertex AI and Pub/Sub. Some Azure. Event-driven and streaming architectures with Kinesis Firehose, Kafka, Redis, and server-sent events. Snowflake, BigQuery, Postgres and pgvector, Weaviate, Qdrant, graph and NoSQL stores. Docker, Kubernetes, Helm, GitLab CI, MLflow, Weights & Biases. FastAPI.

**Statistics and data science.** Precision, recall, and F1; entropy, KL divergence, mutual information, Pearson correlation, MCMC. Hypothesis testing including chi-squared and Kolmogorov-Smirnov. Outlier and anomaly detection, feature engineering and importance, dimensionality reduction, propensity and intent modeling. Time-series trend, seasonality, forecasting and nowcasting, financial technical analysis and correlation structure.

**Domains.** Health tech, HR and careers tech, retail loyalty and personalization, retail media and adtech, CRM and customer journey orchestration, fintech and payments, financial services, insurance, news and media, defense and government research.

------

## Earlier Career

### Ritsumeikan University - Assistant Professor

**2012 - 2013 | Kyoto, Japan**

University lecturer and computational linguistics researcher. Research spanned automated machine-learning scoring of essays with feedback, second-language linguistic analysis, and cross-dataset generalization. Published roughly a dozen peer-reviewed articles and conference papers over the academic years.

### Osaka Jogakuin University - Assistant Professor

**2005 - 2013 | Osaka, Japan**

Roughly eight years as a university instructor and professor in Japan following about seven years teaching English, after arriving in Japan initially as an ESL teacher. Self-directed curriculum and project ownership, supervision of teaching assistants, and budget management. Several hundred public-speaking engagements across lectures, conferences, and presentations.

### Cornerstone Academic College - Director of Academics

**2002 - 2004 | Toronto**

Director-level academic leadership at a private college. Supervised a teaching staff of under twelve, owned curriculum design, and managed students and agent relationships. Non-technical people leadership that predates my technical career but forms part of roughly six years of formal management experience.

------

## Education

- **Master of Science in Applied Computing (MScAC), Machine Learning** - University of Toronto
- **Master of Science, Computer Science (Computational Linguistics)** - University of New England, Australia
- **Master of Arts, Applied Linguistics** - University of New England, Australia
- **Bachelor of Arts, Philosophy and Literature** - Mount Allison University

------

## Selected Publications


- Brath, R., Hagerman, C., Sorenson, E. *Dual y axes charts defended: Case studies, domain analysis and a method.* In *Integrating Artificial Intelligence and Visualization for Visual Knowledge Discovery*, 2022.
- Brath, R., Hagerman, C., et al. *VisIRML: Visualization with Interactive Machine Learning and Information Retrieval Classifier.* In *Integrating Artificial Intelligence and Visualization for Visual Knowledge Discovery*, 2022.
- Brath, R., Hagerman, C., Sorenson, E. *Why Two Y-Axes (Y2Y): Visual Correlation with Dual Axes.* IV2020.
- Hagerman, C., Brath, R. *Automated Insights on Visualizations with Natural Language Generation.* IV2021.
- Hagerman, C., Brath, R. Langevin, S. *Visual Analytic System for Subject Matter Expert Document Tagging using Information Retrieval and Semi-Supervised Machine Learning*, IV2019
- Hagerman, C. *Evaluating the Performance of Automated Part-of-Speech Taggers on an L2 Corpus.* Journal of Osaka Jogakuin, 2012
- Hagerman, C. *An Evaluation of Automated Writing Assessment.* JALT CALL Journal, 2011.
- Hagerman, C. *English language policy and practice in Japan.* Journal of Osaka Jogakuin, 2009

------

## Speaking and Community

- Presented a peer-reviewed paper at the International Conference on Information Visualisation (IV2019) in Paris.
- Founded and led a monthly cross-organization AI roundtable at Jobscan.
- Started a machine learning reading group and data science reading club at Uncharted Software.
- Internal and meetup talks including *Deep Learning for NLP*, *Explainable AI*, *AutoML*, *Text Analytics 101*, *Toronto's Place in AI's Past and Future*, and a talk on non-parametric topic modeling.
- Internal tutorials on topic modeling, notebook and dashboard tooling, and onboarding guides for ML pipelines.

------

## Selected Side Projects

- **Semantic search over a podcast archive.** Speech-to-text, speaker diarization, topic chunking, vectorization, and a vector database supporting semantic search and recommendation over a long-running film review podcast.
- **News aggregator and recommender.** A personal news collector sourcing from GDELT, social feeds, Common Crawl, and Reddit, using PageRank-style ranking and embedding similarity for recommendation.
- **Concept knowledge graph.** A WordNet-style concept map built from Wikipedia, Freebase, and Wikidata, mapping words to concepts. Began at Wattpad and continued as a personal project.
- **Election text analysis.** Social media text analysis of the 2014 US and 2015 Canadian elections, charting sentiment, tone, and volume over time with simple forecasting.