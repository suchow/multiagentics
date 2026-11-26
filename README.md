# Awesome Multiagentics [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of resources for multi-agent AI.

## Contents

- [Foundations & surveys](#foundations--surveys)
- [Orchestration frameworks](#orchestration-frameworks)
- [Communication protocols & standards](#communication-protocols--standards)
- [Environments & simulation](#environments--simulation)
- [Benchmarks & evaluation](#benchmarks--evaluation)
- [Observability & trace tooling](#observability--trace-tooling)
- [Cooperative AI, coordination & game theory](#cooperative-ai-coordination--game-theory)
- [Safety, security & failure modes](#safety-security--failure-modes)
- [Datasets](#datasets)
- [Key papers](#key-papers)
- [Researchers & labs](#researchers--labs)
- [Funders, programs & RFPs](#funders-programs--rfps)
- [Workshops, venues & communities](#workshops-venues--communities)
- [Contributing](#contributing)
- [License](#license)

## Foundations & surveys

- **[A Comprehensive Survey of Multiagent Reinforcement Learning](https://csc.csudh.edu/btang/seminar/multiagent/survey1.pdf)**: Bușoniu, Babuška, and De Schutter classify multiagent reinforcement learning across cooperative, competitive, and mixed tasks, distinguishing stability from adaptation as learning goals (2008).
- **[Distributed Constraint Optimization Problems and Applications: A Survey](https://wyeoh.github.io/assets/pdf/jair-FiorettoPY18.pdf)**: Fioretto, Pontelli, and Yeoh classify DCOP models, solution methods, and applications, including extensions for dynamic and uncertain environments (JAIR, 2018).
- **[Reasoning About Knowledge](https://mitpress.mit.edu/9780262562003/reasoning-about-knowledge/)**: Fagin, Halpern, Moses, and Vardi develop formal approaches to reasoning about agents’ knowledge and apply them to distributed systems, artificial intelligence, and game theory (MIT Press, 1995; linked paperback edition, 2004).
- **[Readings in Distributed Artificial Intelligence](https://api.pageplace.de/preview/DT0400.9781483214443_A23862463/preview-9781483214443_A23862463.pdf)**: Edited by Alan H. Bond and Les Gasser, this collection organizes early distributed AI research around task allocation, coordination, communication, uncertainty, organizational models, and implementation frameworks (Morgan Kaufmann, 1988; publisher preview).
- **[The Interdisciplinary Study of Coordination](https://crowston.syr.edu/sites/default/files/acmcs94.pdf)**: Malone and Crowston analyze coordination as managing dependencies among activities, including shared resources, producer–consumer relationships, and task–subtask relationships (ACM Computing Surveys, 1994).
- **[Exploration and Exploitation in Organizational Learning](https://hiveresearchlab.org/wp-content/uploads/2013/12/march_1991_exploration_and_exploitation_in_organizational_learning.pdf)**: James G. March models mutual learning between individuals and an organizational code and examines trade-offs between developing new knowledge and refining existing knowledge (Organization Science, 1991).

- **[Actors: A Model of Concurrent Computation in Distributed Systems](https://mitpress.mit.edu/9780262511414/actors/)**: Gul Agha formalizes actor computation through a language and mathematical model for asynchronous interaction among independently executing components (MIT Press, 1986).

- **[Handbook of Computational Social Choice](https://www.cambridge.org/core/books/handbook-of-computational-social-choice/8AF63E87F76A5FC974D5E73536C52BD6)**: Edited by Brandt, Conitzer, Endriss, Lang, and Procaccia, this reference covers voting, preference aggregation, allocation, and collective decision-making (Cambridge University Press, 2016).
- **[Rules of Encounter: Designing Conventions for Automated Negotiation among Computers](https://mitpress.mit.edu/9780262181594/rules-of-encounter/)**: Rosenschein and Zlotkin study interaction protocols for autonomous agents with different goals through game-theoretic models of negotiation (MIT Press, 1994).
- **[Strategic Negotiation in Multiagent Environments](https://mitpress.mit.edu/9780262112642/strategic-negotiation-in-multiagent-environments/)**: Sarit Kraus develops strategic negotiation methods for self-interested agents using game theory, economic models, and AI techniques (MIT Press, 2001).

- **[A Concise Introduction to Decentralized POMDPs](https://www.fransoliehoek.net/pub-html/htmlfiles/b2hd-OliehoekAmato16book.html)**: Frans A. Oliehoek and Christopher Amato introduce cooperative planning with decentralized observations and survey exact and approximate solution methods (Springer, 2016).

- **[The Society of Mind](https://www.simonandschuster.com/books/Society-Of-Mind/Marvin-Minsky/9780671657130)**: Marvin Minsky presents intelligence as the interaction of simpler mental agents, a conceptual foundation for specialist-agent architectures (1986; linked paperback edition, 1988).

- **[An Introduction to MultiAgent Systems (2nd ed.)](https://www.wiley.com/en-us/An+Introduction+to+MultiAgent+Systems,+2nd+Edition-p-9780470519462)**: Michael Wooldridge's standard textbook on classical multi-agent systems, covering agent architectures, interaction, and game-theoretic foundations (Wiley, 2009).
- **[Multiagent Systems: Algorithmic, Game-Theoretic, and Logical Foundations](https://www.masfoundations.org/)**: Shoham and Leyton-Brown's graduate textbook on the formal foundations of multi-agent systems, available as a free PDF (Cambridge University Press, 2009).
- **[Open Problems in Cooperative AI](https://arxiv.org/abs/2012.08630)**: Dafoe et al. set out a research agenda for building AI that can cooperate with humans and other agents (2020).
- **[Large Language Model based Multi-Agents: A Survey of Progress and Challenges](https://arxiv.org/abs/2402.01680)**: Guo et al. survey LLM-based multi-agent systems across agent profiling, communication, and capability growth (2024).
- **[LLM Multi-Agent Systems: Challenges and Open Problems](https://arxiv.org/abs/2402.03578)**: Han et al. catalog open problems in LLM multi-agent systems, including task allocation, reasoning, context, and memory (2024).
- **[Multi-Agent Collaboration Mechanisms: A Survey of LLMs](https://arxiv.org/abs/2501.06322)**: Tran et al. propose a framework characterizing LLM multi-agent collaboration by actors, types, structures, strategies, and coordination protocols (2025).

## Orchestration frameworks

- **[Pydantic AI](https://github.com/pydantic/pydantic-ai)**: The Pydantic team's typed Python agent framework supports agent delegation, programmatic handoffs, and graph-based coordination.
- **[Strands Agents](https://github.com/strands-agents/harness-sdk)**: An open-source agent SDK supporting agents-as-tools, graph coordination, and autonomous handoffs. Execution and handoff limits are configurable.
- **[AgentScope](https://github.com/agentscope-ai/agentscope)**: A Python agent framework supporting asynchronous agent interaction, team coordination, evaluation, and deployment.

- **[LangChain](https://github.com/langchain-ai/langchain)**: A Python framework for building LLM applications and agents by chaining together models, tools, and integrations.
- **[CrewAI](https://github.com/crewAIInc/crewAI)**: A Python framework for orchestrating role-playing autonomous agents that collaborate through Crews and event-driven Flows.
- **[LangGraph](https://github.com/langchain-ai/langgraph)**: A low-level orchestration framework from LangChain for building stateful, long-running multi-agent systems as graphs.
- **[Microsoft AutoGen](https://github.com/microsoft/autogen)**: A multi-agent conversation framework from Microsoft, now in maintenance mode with development continuing in the Microsoft Agent Framework.
- **[Microsoft Agent Framework](https://github.com/microsoft/agent-framework)**: Microsoft's multi-language framework for building production agents and multi-agent workflows in .NET and Python, positioned as the successor to AutoGen and Semantic Kernel.
- **[OpenAI Agents SDK](https://github.com/openai/openai-agents-python)**: OpenAI's Python SDK for building multi-agent workflows with handoffs, guardrails, and tracing across many LLM providers.
- **[Google Agent Development Kit (ADK)](https://github.com/google/adk-python)**: Google's code-first Python toolkit for building, evaluating, and deploying agents and multi-agent systems.
- **[CAMEL](https://github.com/camel-ai/camel)**: A Python framework for building and studying communicative multi-agent systems and large-scale agent societies.
- **[MetaGPT](https://github.com/geekan/MetaGPT)**: A multi-agent framework that assigns software-company roles to LLM agents to turn a one-line requirement into software artifacts.
- **[ChatDev](https://github.com/OpenBMB/ChatDev)**: A multi-agent platform that simulates a virtual software company in which LLM agents collaborate to develop software.
- **[Microsoft Semantic Kernel](https://github.com/microsoft/semantic-kernel)**: A model-agnostic SDK from Microsoft for integrating LLMs and building agents in C#, Python, and Java.
- **[LlamaIndex](https://github.com/run-llama/llama_index)**: A data framework for LLM applications that includes agent and multi-agent workflow capabilities over user data.
- **[AG2](https://github.com/ag2ai/ag2)**: A community-governed fork of the original AutoGen for building conversable agents and multi-agent workflows.
- **[Magentic-One](https://microsoft.github.io/autogen/stable/user-guide/agentchat-user-guide/magentic-one.html)**: A generalist multi-agent system built on AutoGen AgentChat that uses an orchestrator plus specialized agents to solve open-ended web and file tasks.
- **[OpenAI Swarm](https://github.com/openai/swarm)**: An educational, lightweight multi-agent orchestration framework from OpenAI, superseded by the OpenAI Agents SDK.

## Communication protocols & standards

- **[Agent Communication Languages: Rethinking the Principles](https://www.csc2.ncsu.edu/faculty/mpsingh/papers/mas/computer-acl-98.pdf)**: Munindar P. Singh argues for communication semantics grounded in public social interaction and commitments (Computer, 1998).
- **[Verifiable Semantics for Agent Communication Languages](https://www.cs.ox.ac.uk/people/michael.wooldridge/pubs/icmas98.pdf)**: Michael Wooldridge defines a formal framework for determining whether an independent observer can verify semantic conformance in specified agent communication systems (ICMAS, 1998).

- **[Model Context Protocol (MCP)](https://modelcontextprotocol.io/)**: An open standard, originally from Anthropic and now contributed to the Linux Foundation's Agentic AI Foundation, that connects AI applications to external data sources, tools, and prompts.
- **[Agent2Agent (A2A)](https://a2a-protocol.org/)**: An open protocol, originally developed by Google and now hosted by the Linux Foundation, that lets independent AI agents discover one another and exchange tasks and messages across vendors and frameworks.
- **[AGNTCY / Internet of Agents](https://docs.agntcy.org/)**: A Linux Foundation project, initially open-sourced by Cisco, providing infrastructure for agent discovery, identity, messaging, and observability across multi-agent systems.
- **[Agent Communication Protocol (ACP)](https://agentcommunicationprotocol.dev/)**: An open, REST-based protocol introduced by IBM's BeeAI for agent interoperability, now developed as part of A2A under the Linux Foundation.
- **[Agent Network Protocol (ANP)](https://github.com/agent-network-protocol/AgentNetworkProtocol)**: An open-source protocol using W3C Decentralized Identifiers to provide identity, encrypted communication, and capability discovery for agent-to-agent collaboration.
- **[FIPA ACL Message Structure Specification](http://www.fipa.org/specs/fipa00061/SC00061G.html)**: The 2002 FIPA standard defining the message structure of the Agent Communication Language, a historical reference for interoperable multi-agent communication.
- **[KQML](https://research.cs.umbc.edu/kqml/)**: The UMBC resource hub for the Knowledge Query and Manipulation Language, an early-1990s DARPA-sponsored language and protocol for knowledge exchange among software agents.

## Environments & simulation

- **[Google Research Football: A Novel Reinforcement Learning Environment](https://cdn.aaai.org/ojs/5878/5878-13-9103-1-10-20200513.pdf)**: Kurach et al. provide a football simulator with multiplayer and multi-agent support, full-game benchmarks, and simpler Football Academy scenarios (AAAI, 2020).
- **[The Neural MMO Platform for Massively Multiagent Research](https://arxiv.org/abs/2110.07594)**: Suarez, Du, Zhu, Mordatch, and Isola describe the 2021 MMO-inspired platform combining large agent populations, long horizons, open-ended tasks, and modular game systems (2021).

- **[How Well Can LLMs Negotiate? NegotiationArena Platform and Analysis](https://arxiv.org/abs/2402.05863)**: Bianchi et al. introduce multi-turn ultimatum, trading, and price-negotiation games between language agents (2024).
- **[AgentSociety: Large-Scale Simulation of LLM-Driven Generative Agents Advances Understanding of Human Behaviors and Society](https://arxiv.org/abs/2502.08691)**: Piao et al. simulate large populations of language-model agents in social environments for experiments on collective behavior and policy interventions (2025 preprint).

- **[Overcooked-AI](https://github.com/HumanCompatibleAI/overcooked_ai)**: A cooperative cooking environment from Carroll et al. for studying coordination with human partners and unfamiliar policies (NeurIPS, 2019).
- **[SMACv2](https://github.com/oxwhirl/smacv2)**: Ellis et al. provide procedurally generated StarCraft II micromanagement scenarios for evaluating decentralized cooperative policies under partial observability (NeurIPS, 2023).
- **[SOTOPIA environment](https://github.com/sotopia-lab/sotopia)**: The open-ended role-play environment accompanying Zhou et al.'s SOTOPIA paper, with scenarios and evaluation tooling for language-agent social interactions (ICLR, 2024).

- **[PettingZoo](https://github.com/Farama-Foundation/PettingZoo)**: A Python API standard and environment suite for multi-agent reinforcement learning, maintained by the Farama Foundation.
- **[Melting Pot](https://github.com/google-deepmind/meltingpot)**: A DeepMind suite of multi-agent reinforcement learning substrates and test scenarios for evaluating social generalization.
- **[Concordia](https://github.com/google-deepmind/concordia)**: A DeepMind library for generative agent-based social simulation using a game-master pattern.
- **[OpenSpiel](https://github.com/google-deepmind/open_spiel)**: A DeepMind collection of environments and algorithms for research in games and multi-agent reinforcement learning.
- **[Generative Agents (Smallville)](https://github.com/joonspk-research/generative_agents)**: The Stanford research codebase for generative agents that simulate human behavior in the Smallville environment.
- **[AgentVerse](https://github.com/OpenBMB/AgentVerse)**: A framework for deploying multiple LLM agents in task-solving and social-simulation environments.
- **[AI Town](https://github.com/a16z-infra/ai-town)**: A deployable starter kit for a virtual town where AI characters live, chat, and socialize.
- **[MAgent2](https://github.com/Farama-Foundation/MAgent2)**: A Farama Foundation engine and reference environments for gridworld scenarios with very large numbers of agents.
- **[JaxMARL](https://github.com/FLAIROx/JaxMARL)**: A JAX library of GPU-accelerated multi-agent reinforcement learning environments and baseline algorithms.
- **[VirtualHome](https://github.com/xavierpuigf/virtualhome)**: A Python and Unity platform for simulating multi-agent household activities via programs.
- **[AgentSims](https://github.com/py499372727/AgentSims)**: A sandbox infrastructure for evaluating LLM agents through task-based simulations in an interactive town environment.

## Benchmarks & evaluation

- **[ParaCook: On Time-Efficient Planning for Multi-Agent Systems](https://aclanthology.org/2026.findings-acl.1378/)**: Zhang et al. evaluate time-efficient parallel planning through cooking tasks with simplified actions and adjustable coordination complexity (Findings of ACL, 2026).

- **[MACRO: A Benchmark for Clarification-Aware Multi-Agent Orchestration](https://aclanthology.org/2026.emnlp-main.2061/)**: Li et al. evaluate clarification, routing, and dependent-subtask coordination in travel requests using process-level milestones and standardized sub-agent interfaces (EMNLP, 2026).
- **[The Price of Thought: A Multilingual Analysis of Reasoning, Performance, and Cost of Negotiation in Large Language Models](https://aclanthology.org/2026.findings-eacl.27/)**: Hakimov et al. compare negotiation performance, computational cost, and reasoning-language consistency across three languages and three dialogue games (Findings of EACL, 2026).

- **[Seeing the Whole Elephant: A Benchmark for Failure Attribution in LLM-based Multi-Agent Systems](https://aclanthology.org/2026.acl-long.912/)**: Chen et al. introduce TraceElephant to evaluate failure attribution using complete execution traces, including agent inputs and context (ACL, 2026).
- **[VIKI-R: Coordinating Embodied Multi-Agent Cooperation via Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2025/hash/ab16cc8f472cf94b282dbff7b99f5f8e-Abstract-Datasets_and_Benchmarks_Track.html)**: Kang et al. introduce VIKI-Bench for visually grounded cooperation across robot embodiments. They evaluate agent activation, task planning, and trajectory perception (NeurIPS, 2025).

- **[LLM-Coordination: Evaluating and Analyzing Multi-agent Coordination Abilities in Large Language Models](https://aclanthology.org/2025.findings-naacl.448/)**: Agashe et al. evaluate agent behavior in four pure coordination games and use 198 questions to examine environment comprehension, partner reasoning, and joint planning (Findings of NAACL, 2025).

- **[The Collaboration Gap: Exploration and Benchmarking of Open-World Agentic Cooperation](https://proceedings.colm.cc/paper_files/paper/2026/hash/42806406dd99e30c3796bc98b2670fa2-Abstract-Conference.html)**: Davidson et al. evaluate natural-language cooperation between homogeneous and heterogeneous agent pairs in maze tasks without prescribed communication formats (COLM, 2026 pre-proceedings).

- **[Multi-Agent Pathfinding: Definitions, Variants, and Benchmarks](https://cdn.aaai.org/ojs/18510/18510-77-22026-1-2-20210717.pdf)**: Stern et al. define common multi-agent pathfinding assumptions, objectives, and conflicts and introduce grid-based benchmark problems (SoCS, 2019).

- **[SILO-BENCH: A Scalable Environment for Evaluating Distributed Coordination in Multi-Agent LLM Systems](https://aclanthology.org/2026.acl-long.1354/)**: Zhang et al. evaluate role-free collaboration under distributed information through 30 algorithmic tasks with exact answers and three levels of communication complexity (ACL, 2026).
- **[PAC-BENCH: Evaluating Multi-Agent Collaboration under Privacy Constraints](https://aclanthology.org/2026.findings-acl.1552/)**: Park et al. evaluate multi-agent collaboration under privacy constraints and analyze coordination failures involving disclosure, abstraction, and unsupported information (Findings of ACL, 2026).

- **[PARTNR: A Benchmark for Planning and Reasoning in Embodied Multi-agent Tasks](https://proceedings.iclr.cc/paper_files/paper/2025/hash/a3cf318fbeec1126da21e9185ae9908c-Abstract-Conference.html)**: Chang et al. evaluate household human–robot collaboration through 100,000 simulated tasks with spatial, temporal, and heterogeneous capability constraints (ICLR, 2025).
- **[LLM Agents for Coordinating Multi-User Information Gathering](https://aclanthology.org/2025.findings-acl.916/)**: Jhamtani, Andreas, and Van Durme introduce PeopleJoin, which evaluates teammate discovery, information gathering, and answer synthesis across synthetic organizations (Findings of ACL, 2025).

- **[The Evaluation Substrate Matters: Benchmarking Multi-Agent Serving Substrates](https://arxiv.org/abs/2611.28671)**: Zheng et al. introduce MASSys to compare the same agent workloads across serving environments and loads using evidence on task quality, delivery, latency, cost, and failures (2026 preprint).

- **[TeamBench: Evaluating Agent Coordination under Enforced Role Separation](https://arxiv.org/abs/2605.07073)**: Kim et al. evaluate coordination under operating system-enforced separation of Planner, Executor, and Verifier roles (2026 preprint).
- **[AsynCodeBench: Benchmarking Collaboration of Asynchronous Multi-Agent Systems in Software Engineering](https://arxiv.org/abs/2609.32662)**: Zhang et al. measure whether and when cross-agent coding dependencies are satisfied through executable checks across 19 repository tasks (2026 preprint).

- **[CooperBench: Why Coding Agents Cannot be Your Teammates Yet](https://arxiv.org/abs/2601.13295)**: Khatua et al. evaluate coordination between coding agents assigned separate features that may conflict, using repository tasks with expert-written tests (2026).
- **[Collab-Overcooked: Benchmarking and Evaluating Large Language Models as Collaborative Agents](https://aclanthology.org/2025.emnlp-main.249/)**: Sun et al. evaluate communication and adaptation during collaborative task execution in an Overcooked environment (EMNLP, 2025).

- **[MultiAgentBench / MARBLE](https://github.com/ulab-uiuc/MARBLE)**: An ACL 2025 benchmark and framework that evaluates the collaboration and competition of LLM agents across coordination topologies using milestone-based metrics.
- **[REALM-Bench](https://github.com/genglongling/REALM-Bench)**: A benchmark for evaluating multi-agent systems on real-world, dynamic planning and scheduling tasks across multiple agent frameworks.
- **[AgentBench](https://github.com/THUDM/AgentBench)**: An ICLR 2024 benchmark that evaluates LLMs as autonomous agents across eight distinct interactive environments.
- **[AgentBoard](https://github.com/hkust-nlp/AgentBoard)**: A NeurIPS 2024 benchmark and analytical evaluation board for multi-turn LLM agents, reporting fine-grained progress metrics across nine tasks.
- **[AgentGym](https://github.com/WooooDyy/AgentGym)**: A framework and benchmark suite for evaluating and evolving LLM-based agents across 14 diverse interactive environments in a unified format.
- **[τ-bench / tau2-bench](https://github.com/sierra-research/tau2-bench)**: A benchmark from Sierra for tool-agent-user interaction that evaluates agents conversing with a simulated user across domains such as airline, retail, telecom, and banking.
- **[GAIA](https://huggingface.co/spaces/gaia-benchmark/leaderboard)**: A benchmark of real-world questions for general AI assistants requiring reasoning, multimodal understanding, web browsing, and tool use, with a public Hugging Face leaderboard.
- **[Inspect](https://inspect.aisi.org.uk/)**: An open-source evaluation framework from the UK AI Security Institute providing composable datasets, agents, tools, and scorers for LLM and agentic evaluations.
- **[ControlArena](https://github.com/UKGovernmentBEIS/control-arena)**: A library from the UK AI Security Institute and Redwood Research for running AI control experiments across settings, model organisms, and protocols, built on Inspect.
- **[SWE-bench](https://www.swebench.com/)**: A benchmark that tasks agents with resolving real-world GitHub issues by generating patches verified through unit tests.
- **[BrowserGym](https://github.com/ServiceNow/BrowserGym)**: A Gym environment from ServiceNow for web-task automation that unifies benchmarks such as MiniWoB, WebArena, and WorkArena.
- **[WebArena](https://github.com/web-arena-x/webarena)**: A self-hostable, realistic web environment with 812 long-horizon tasks for building and evaluating autonomous web agents.
- **[MLAgentBench](https://github.com/snap-stanford/MLAgentBench)**: A benchmark of end-to-end machine-learning experimentation tasks for evaluating language agents as AI research agents.

## Observability & trace tooling

- **[LangSmith](https://www.langchain.com/langsmith)**: Framework-agnostic SaaS platform from LangChain for tracing, evaluating, and monitoring LLM and agent applications.
- **[Langfuse](https://github.com/langfuse/langfuse)**: Open-source (self-hostable) LLM engineering platform offering tracing, evaluation, prompt management, and datasets, with OpenTelemetry integration.
- **[Arize Phoenix](https://github.com/Arize-ai/phoenix)**: Open-source AI observability and evaluation tool with native OpenTelemetry support for tracing LLM and agent applications.
- **[Weights & Biases Weave](https://github.com/wandb/weave)**: Open-source toolkit from Weights & Biases for logging, tracing, and evaluating LLM application inputs, outputs, and calls.
- **[AgentOps](https://github.com/AgentOps-AI/agentops)**: Open-source Python SDK for monitoring AI agents, with session replay, LLM cost tracking, and integrations for CrewAI, AutoGen, LangChain, and the OpenAI Agents SDK.
- **[Langtrace](https://github.com/Scale3-Labs/langtrace)**: Open-source, OpenTelemetry-based observability tool providing tracing, evaluations, and metrics for LLMs, frameworks, and vector databases.
- **[Pydantic Logfire](https://github.com/pydantic/logfire)**: Observability platform built on OpenTelemetry by the Pydantic team, with features for tracing LLM calls and agent behavior.
- **[Helicone](https://github.com/Helicone/helicone)**: Open-source LLM observability platform for monitoring, evaluating, and experimenting on traces and sessions.
- **[OpenLLMetry (Traceloop)](https://github.com/traceloop/openllmetry)**: Open-source set of OpenTelemetry-based extensions, maintained by Traceloop, for instrumenting GenAI and LLM applications.
- **[Inspect log viewer](https://github.com/UKGovernmentBEIS/inspect_ai)**: The UK AI Security Institute's evaluation framework, including a web-based log viewer for inspecting agent and evaluation transcripts.
- **[Transluce Docent](https://docent.transluce.org)**: Tool from Transluce for searching, clustering, and analyzing long agent transcripts to surface behaviors and failures.
- **[OpenTelemetry GenAI semantic conventions](https://opentelemetry.io/docs/specs/semconv/gen-ai/)**: Standard schema under OpenTelemetry defining attributes, spans, metrics, and events for generative AI and agent telemetry.
- **[OpenInference](https://github.com/Arize-ai/openinference)**: Specification and instrumentation libraries from Arize that complement OpenTelemetry to standardize tracing of AI applications.

## Cooperative AI, coordination & game theory

- **[Stochastic Games](https://bpb-us-w2.wpmucdn.com/sites.umassd.edu/dist/1/1807/files/2026/02/Stochastic-games-Shapley.pdf)**: Lloyd S. Shapley introduces games with jointly controlled probabilistic state transitions and establishes stationary optimal strategies for finite two-player zero-sum games with a positive stopping probability (PNAS, 1953).
- **[Games with Incomplete Information Played by “Bayesian” Players, I–III. Part I. The Basic Model](https://gamef21.classes.ryansafner.com/readings/Harsanyi-1967.pdf)**: John C. Harsanyi models uncertainty about other players’ payoffs and information through player types and probabilistic beliefs (Management Science, 1967).

- **[Potential Games](https://old.corelab.ntua.gr/courses/gametheory/old/1011/material/potentialgames.pdf)**: Monderer and Shapley characterize games whose unilateral payoff changes correspond to changes in a potential function, with equilibrium and improvement-path properties tied to that structure (1996).
- **[Coalition Formation among Bounded Rational Agents](https://ijcai.org/proceedings/1995/87)**: Sandholm and Lesser model coalition formation when computation has a cost and analyze how algorithm performance affects coalition value and stability (IJCAI, 1995).

- **[The Evolution of Cooperation](https://websites.umich.edu/axe/research/Axelrod%20and%20Hamilton%20EC%201981.pdf)**: Axelrod and Hamilton study conditions for reciprocal cooperation through iterated prisoner’s-dilemma strategies and evolutionary analysis (Science, 1981).
- **[Five Rules for the Evolution of Cooperation](https://pmc.ncbi.nlm.nih.gov/articles/PMC3279745/)**: Martin A. Nowak synthesizes kin selection, direct reciprocity, indirect reciprocity, network reciprocity, and group selection through model-specific cooperation conditions (Science, 2006).

- **[Non-Cooperative Games](https://cs.uwaterloo.ca/~klarson/teaching/F04-886/papers/nash51.pdf)**: John Nash defines equilibrium for finite non-cooperative games and proves its existence (1951).
- **[Subjectivity and Correlation in Randomized Strategies](https://cris.huji.ac.il/en/publications/subjectivity-and-correlation-in-randomized-strategies/)**: Robert J. Aumann introduces correlated equilibrium, in which agents can condition decisions on correlated signals (1974).
- **[A Simple Adaptive Procedure Leading to Correlated Equilibrium](https://ma.huji.ac.il/hart/papers/adapt.pdf)**: Hart and Mas-Colell introduce regret matching and prove convergence of empirical play to the correlated-equilibrium set under their finite-game assumptions (2000).

- **[Optimal Auction Design](https://pubsonline.informs.org/doi/10.1287/moor.6.1.58)**: Roger B. Myerson studies mechanism design for allocating a scarce resource among agents with private valuations (1981).
- **[Incentives in Teams](https://ranger.uta.edu/~weems/NOTES6319/PAPERSTWO/groves.pdf)**: Theodore Groves studies compensation rules for aligning decentralized organizational decisions and information reporting with a common objective (1973).
- **[A Difficulty in the Concept of Social Welfare](https://www.journals.uchicago.edu/doi/abs/10.1086/256963?journalCode=jpe)**: Kenneth J. Arrow establishes limits on aggregating individual rankings into a collective preference under specified conditions (1950).

- **[Teamwork](https://www.sri.com/publication/teamwork/)**: Cohen and Levesque formalize shared commitments and mental states in teamwork, including communication about failures and misunderstandings (1991).
- **[Collaborative plans for complex group action](https://jmvidal.cse.sc.edu/library/grosz96a.pdf)**: Grosz and Kraus develop SharedPlans for coordinating complex activities with partial plans, commitments, and delegated actions (1996).
- **[Human Computation](https://www.sigecom.org/exchanges/volume_10/3/LAW.pdf)**: Law and von Ahn survey task allocation, incentives, output aggregation, and joint human–machine problem solving; the link is their book announcement (2011).

- **[Groups of diverse problem solvers can outperform groups of high-ability problem solvers](https://pmc.ncbi.nlm.nih.gov/articles/PMC528939/)**: Hong and Page model how complementary representations and search heuristics can improve team problem solving under stated mathematical assumptions (PNAS, 2004).
- **[Evidence for a Collective Intelligence Factor in the Performance of Human Groups](https://www.chabris.com/Woolley2010a.pdf)**: Woolley et al. study human-group performance across diverse tasks and its relationship to interaction patterns. Transfer of these findings to AI teams is unverified (Science, 2010).

- **[Cooperative AI Foundation](https://www.cooperativeai.com/)**: A nonprofit foundation that funds and coordinates research aimed at improving the cooperative capabilities of AI systems.
- **[Cooperative AI: machines must learn to find common ground (Nature 2021)](https://doi.org/10.1038/d41586-021-01170-0)**: A Nature comment by Dafoe and colleagues arguing that AI research should be reconceived to address problems of cooperation.
- **[FOCAL: Foundations of Cooperative AI Lab (CMU)](https://www.cs.cmu.edu/~focal/)**: A Carnegie Mellon University lab, directed by Vincent Conitzer, developing game-theoretic foundations for cooperation among autonomous AI agents.
- **[CICERO](https://ai.meta.com/research/cicero/)**: Meta AI's agent for the game Diplomacy that combines a language model with strategic reasoning to negotiate with human players.
- **[Hanabi Learning Environment](https://github.com/google-deepmind/hanabi-learning-environment)**: A DeepMind research platform for the cooperative card game Hanabi, used as a benchmark for multi-agent coordination under imperfect information.
- **[Welfare Diplomacy](https://arxiv.org/abs/2310.08901)**: A general-sum variant of Diplomacy and open-source engine designed to benchmark and incentivize cooperative capabilities in language-model agents.
- **[GovSim / Cooperate or Collapse](https://arxiv.org/abs/2404.16698)**: A simulation platform and paper studying whether societies of LLM agents can sustainably manage shared common-pool resources.

## Safety, security & failure modes

- **[Delegated Misalignment: How Multi-Agent Structures Amplify LLM Safety Risks](https://aclanthology.org/2026.emnlp-main.398/)**: Ying et al. compare single-agent and delegated execution across six models and 49 hazardous tasks. They examine how principal and subordinate roles affect harmful behavior (EMNLP, 2026).

- **[On the Resilience of LLM-Based Multi-Agent Collaboration with Faulty Agents](https://proceedings.mlr.press/v267/huang25ay.html)**: Huang et al. inject faulty agent responses to compare collaboration structures and evaluate challenge and inspection mechanisms across four tasks (ICML, 2025).
- **[Among Us: Measuring and Mitigating Malicious Contributions in Model Collaboration Systems](https://aclanthology.org/2026.acl-long.725/)**: Yang et al. evaluate malicious model contributions across four collaboration settings and ten datasets, then test supervisory mitigation strategies (ACL, 2026).

- **[Multi-Agent Systems Execute Arbitrary Malicious Code](https://arxiv.org/abs/2503.12188)**: Triedman, Jha, and Shmatikov demonstrate control-flow hijacking through untrusted content in tested multi-agent frameworks, including code execution and data exfiltration (2025).

- **[Secret Collusion among AI Agents: Multi-Agent Deception via Steganography](https://proceedings.neurips.cc/paper_files/paper/2024/hash/861f7dad098aec1c3560fb7add468d41-Abstract-Conference.html)**: Motwani et al. formalize covert coordination through steganographic communication and study limitations of oversight countermeasures (NeurIPS, 2024).
- **[The Best-Laid SCHEMEs: Coordinated Sabotage and Monitoring in Multi-Agent Systems](https://arxiv.org/abs/2605.29178)**: Radev, Haas, Arnav, and Bernabeu-Pérez introduce SCHEME, a benchmark pairing legitimate coding tasks with instructed malicious side tasks requiring coordination among agents (2026).
- **[TAMAS: Benchmarking Adversarial Risks in Multi-Agent LLM Systems](https://aclanthology.org/2026.acl-long.1442/)**: Kavathekar et al. evaluate adversarial attacks and benign task performance across AutoGen and CrewAI configurations (ACL, 2026).

- **[ORBIT: A Framework for Multi-Agent Safety and Security Evaluations](https://arxiv.org/abs/2609.33102)**: Hagag, Anderson, Chakraborty, and Schroeder de Witt introduce an Inspect-based framework for comparing attacks, defenses, and multi-agent architectures across several scenario families (2026 preprint).
- **[ConVerse: Benchmarking Contextual Safety in Agent-to-Agent Conversations](https://aclanthology.org/2026.findings-eacl.170/)**: Gomaa, Salem, and Abdelnabi evaluate privacy leakage and security failures in multi-turn conversations between personal assistants and external service agents (Findings of EACL, 2026).
- **[A2ASecBench: A Protocol-Aware Security Benchmark for Agent-to-Agent Multi-Agent Systems](https://safo-lab.github.io/A2ASecBench/)**: Li et al. evaluate attacks on agent discovery, task handling, and artifact exchange in A2A systems alongside benign tasks (ICLR, 2026).

- **[Multi-Agent Risks from Advanced AI](https://arxiv.org/abs/2502.14143)**: A Cooperative AI Foundation technical report presenting a taxonomy of risks that arise when advanced AI agents interact, along with a research agenda.
- **[Open Challenges in Multi-Agent Security](https://arxiv.org/abs/2505.02077)**: A paper defining multi-agent security as a field and presenting a threat taxonomy and research agenda for securing networks of interacting AI agents.
- **[Why Do Multi-Agent LLM Systems Fail? (MAST)](https://arxiv.org/abs/2503.13657)**: A study introducing the Multi-Agent System Failure Taxonomy, identifying 14 failure modes across popular multi-agent LLM frameworks.
- **[MAST repository](https://github.com/multi-agent-systems-failure-taxonomy/MAST)**: The code and annotated trace dataset accompanying the "Why Do Multi-Agent LLM Systems Fail?" paper.
- **[AgentDojo](https://github.com/ethz-spylab/agentdojo)**: A dynamic benchmark environment for evaluating prompt-injection attacks and defenses against tool-using LLM agents.
- **[OWASP Agentic AI: Threats and Mitigations](https://genai.owasp.org/resource/agentic-ai-threats-and-mitigations/)**: The OWASP GenAI Security Project's threat-model reference cataloguing security risks and mitigations for agentic AI systems.
- **[OWASP Top 10 for Agentic Applications (2026)](https://genai.owasp.org/resource/owasp-top-10-for-agentic-applications-for-2026/)**: A ranked list of the most critical security risks for autonomous, tool-using AI agents, produced by the OWASP GenAI Security Project.
- **[Algorithmic Collusion by Large Language Models (Fish et al.)](https://arxiv.org/abs/2404.00806)**: A paper showing that LLM-based pricing agents can autonomously reach supracompetitive prices in oligopoly and auction settings.
- **[Artificial Intelligence, Algorithmic Pricing, and Collusion (Calvano et al.)](https://doi.org/10.1257/aer.20190623)**: An American Economic Review study demonstrating that Q-learning pricing algorithms can learn collusive strategies without communicating.

## Datasets

- **[MutualFriends](https://stanfordnlp.github.io/cocoa/)**: He, Balakrishnan, Eric, and Liang release human–human dialogues in which participants exchange information from separate knowledge bases to identify a mutual friend (ACL, 2017).
- **[DealOrNoDeal](https://github.com/facebookresearch/end-to-end-negotiator)**: Lewis et al. release negotiation dialogues involving item allocation and private agent rewards, accompanying *Deal or No Deal? End-to-End Learning of Negotiation Dialogues* (EMNLP, 2017).
- **[CraigslistBargain](https://huggingface.co/datasets/stanfordnlp/craigslist_bargains)**: He, Chen, Balakrishnan, and Liang release buyer–seller dialogues for studying strategic bargaining over products described in Craigslist listings (EMNLP, 2018).

- **[ToolBench](https://github.com/OpenBMB/ToolBench)**: Open-source instruction-tuning dataset and platform for tool learning, built from 16,000+ real-world RapidAPI APIs with single- and multi-tool scenarios.
- **[xLAM function-calling 60k](https://huggingface.co/datasets/Salesforce/xlam-function-calling-60k)**: Salesforce dataset of 60,000 verified function-calling examples generated by the APIGen pipeline across 3,673 executable APIs.
- **[APIGen-MT-5k](https://huggingface.co/datasets/Salesforce/APIGen-MT-5k)**: Salesforce dataset of 5,000 synthetic multi-turn agent trajectories produced via simulated agent-human interplay.
- **[Berkeley Function-Calling Leaderboard](https://huggingface.co/datasets/gorilla-llm/Berkeley-Function-Calling-Leaderboard)**: UC Berkeley Gorilla project's question-and-function-documentation dataset used to evaluate LLM function-calling across multiple categories.
- **[AgentInstruct (THUDM)](https://huggingface.co/datasets/THUDM/AgentInstruct)**: Dataset of 1,866 multi-turn agent interaction trajectories across six tasks, used to train the AgentLM models.
- **[Orca-AgentInstruct-1M](https://huggingface.co/datasets/microsoft/orca-agentinstruct-1M-v1)**: Microsoft dataset of 1 million synthetic instruction pairs generated by the AgentInstruct multi-agent workflow, covering skills including tool use and coding.
- **[ToolACE](https://huggingface.co/datasets/Team-ACE/ToolACE)**: Tool-learning dataset generated by a multi-agent pipeline over a pool of 26,507 APIs, covering single, parallel, dependent, and multi-turn function calls.
- **[Glaive function-calling v2](https://huggingface.co/datasets/glaiveai/glaive-function-calling-v2)**: Dataset of roughly 52,000 samples for training models on function-calling tasks, including no-call, single-call, and multi-call examples.
- **[Hermes Function-Calling V1](https://huggingface.co/datasets/NousResearch/hermes-function-calling-v1)**: Nous Research dataset of single- and multi-turn function-calling and structured JSON output samples in ShareGPT format.

## Key papers

- **[CrowdForge: Crowdsourcing Complex Work](https://smus.com/crowdforge/crowdforge-uist-11.pdf)**: Kittur, Smus, Khamkar, and Kraut organize complex human crowdsourced work through nested partition, map, and reduce tasks, with case studies in writing, decision making, and science journalism (UIST, 2011).
- **[A Two-Tier Perspective on Inference-Time Parallelism in Multi-Agent LLM Systems](https://proceedings.mlr.press/v306/xu26bb.html)**: Xu, Tian, and Jiang distinguish parallel complete-solution replicas from concurrent subtasks within a solution. They evaluate combinations through TIPEX on GAIA, examining accuracy, latency, and token use (ICML, 2026).
- **[A Theory of Fads, Fashion, Custom, and Cultural Change as Informational Cascades](https://snap.stanford.edu/class/cs224w-2010/readings/bikhchandani92fads.pdf)**: Bikhchandani, Hirshleifer, and Welch model informational cascades in which sequential decision makers follow earlier actions despite their private information. The model explains potentially mistaken and fragile conformity (1992).
- **[CooT: Learning to Coordinate In-Context with Coordination Transformers](https://proceedings.mlr.press/v306/wang26ag.html)**: Wang et al. train transformers on diverse partner-behavior trajectories. After training, coordination uses observations without parameter updates. They evaluate the method in Overcooked and Google Research Football (ICML, 2026).
- **[Group Versus Individual Training and Group Performance: The Mediating Role of Transactive Memory](https://journals.sagepub.com/doi/10.1177/0146167295214009)**: Liang, Moreland, and Argote compare group and individual training for radio assembly in three-person human groups. Better group recall and product quality are associated with transactive memory (1995).
- **[MAS-Orchestra: Understanding and Improving Multi-Agent Reasoning Through Holistic Orchestration and Controlled Benchmarks](https://proceedings.mlr.press/v306/ke26c.html)**: Ke et al. train orchestration through function-calling reinforcement learning and introduce MASBENCH to evaluate task depth, horizon, breadth, parallelism, and robustness (ICML, 2026).
- **[Evolving Interpretable Constitutions for Multi-Agent Coordination](https://proceedings.mlr.press/v306/kumar26f.html)**: Kumar et al. use LLM-driven genetic programming to evolve explicit behavioral rules for agents in a survival grid world. They evaluate productivity, survival, and conflict through a combined score (ICML, 2026).
- **[AgentSpeak(L): BDI agents speak out in a logical computable language](https://link.springer.com/chapter/10.1007/BFb0031845)**: Anand S. Rao gives AgentSpeak(L) operational and proof-theoretic semantics, connecting executable BDI agent programs with formal reasoning about their properties (MAAMAW, 1996).
- **[Beyond Correctness: Distance-Based Social Dynamics of Multi-Agent Debate](https://proceedings.mlr.press/v306/ha26a.html)**: Ha and Mitchell study answer revisions under controlled peer responses in ConceptARC, measuring changes in solution distance alongside binary correctness in two-dimensional grid tasks (ICML, 2026).
- **[Communication and Interaction in Multi-Agent Planning](https://cdn.aaai.org/AAAI/1983/AAAI83-003.pdf)**: Michael Georgeff combines separately generated plans by analyzing conflicting actions and unsafe interactions, then inserting synchronization communications. The method assumes STRIPS-style persistence and sufficiently decoupled agent effects (AAAI, 1983).
- **[A Diagnostic Study of Multi-Agent LLMs for Real-World Debates](https://proceedings.mlr.press/v306/pitre26a.html)**: Pitre et al. evaluate debate processes through engagement, responsiveness, influence balance, stability, and agent utility, alongside outcome measures (ICML, 2026).
- **[LiveCultureBench: a Multi-Agent, Multi-Cultural Benchmark for Large Language Models in Dynamic Social Simulations](https://aclanthology.org/2026.acl-long.1247/)**: Pham et al. evaluate task completion and sociocultural norm adherence in a simulated town with synthetic resident profiles, including uncertainty in model-based judgments (ACL, 2026).
- **[A Value for n-Person Games](https://www.degruyterbrill.com/document/doi/10.1515/9781400881970-018/html)**: Lloyd S. Shapley characterizes a value for cooperative characteristic-function games through axioms, addressing allocation of gains among coalition participants (1953).
- **[Asynchronous Credit Assignment for Multi-Agent Reinforcement Learning](https://ijcai.org/proceedings/2025/20)**: Liang et al. study credit assignment when agents act asynchronously, using a virtual synchrony proxy and multiplicative value decomposition to model dependencies between actions (IJCAI, 2025).

- **[The Open Agent Architecture: A Framework for Building Distributed Software Systems](https://www.tandfonline.com/doi/abs/10.1080/088395199117504)**: Martin, Cheyer, and Moran describe OAA, where facilitators match service requests with agents’ declared capabilities to coordinate heterogeneous distributed software components (Applied Artificial Intelligence, 1999).
- **[Architecture Matters for Multi-Agent Security](https://proceedings.mlr.press/v306/hagag26a.html)**: Hagag et al. compare roles, interaction topology, and memory visibility in web-agent systems. Their evaluation separates planning refusal, execution interception, and completed attacks (ICML, 2026).
- **[MaMa: A Game-Theoretic Approach for Designing Safe Agentic Systems](https://proceedings.mlr.press/v306/nother26a.html)**: Nöther, Singla, and Radanovic use adversarial search to design multi-agent systems against attacks that compromise selected agents. The design process uses feedback from the strongest attacks discovered by the search (ICML, 2026).

- **[Controlling cooperative problem solving in industrial multi-agent systems using joint intentions](https://apice.unibo.it/bin/view/Publication/IndustrialcoordinationAi75)**: Nicholas R. Jennings implements Joint Responsibility in GRATE*, specifying how cooperation starts, proceeds, and responds to difficulties. Comparative experiments concern electricity transportation management (Artificial Intelligence, 1995).
- **[AgentWebBench: Benchmarking Multi-Agent Coordination in Agentic Web](https://proceedings.mlr.press/v306/zhong26n.html)**: Zhong, Shen, and Xiong evaluate search, recommendation, question answering, and research through interactions between user agents and website-specific content agents (ICML, 2026).
- **[Benchmarking the Limits of In-Context Reinforcement Learning for Ad-Hoc Teamwork](https://proceedings.mlr.press/v306/jing26d.html)**: Jing et al. introduce ICRL4AHT to test history-conditioned adaptation to unseen teammates and layouts in Overcooked-V2 through controlled shifts and multi-episode evaluation (ICML, 2026).

- **[Multipart Pricing of Public Goods](https://ranger.uta.edu/~weems/NOTES6319/PAPERSTWO/clarke.pdf)**: Edward H. Clarke develops a multipart pricing mechanism for public goods that elicits demand information through payments based on participants’ effects on others (Public Choice, 1971).
- **[Shapley-Coop: Credit Assignment for Emergent Cooperation in Self-Interested LLM Agents](https://proceedings.neurips.cc/paper_files/paper/2025/hash/80164880902980257ef58412322fc374-Abstract-Conference.html)**: Hua et al. combine structured negotiation with Shapley-inspired contribution estimates to allocate rewards. Evaluation covers two games and a software engineering simulation (NeurIPS, 2025).
- **[Recursive Reasoning or Statistical Extrapolation? In-Context Learning in Multi-Agent Interdependent Decision-Making](https://aclanthology.org/2026.findings-emnlp.1680/)**: Liu et al. perturb interaction histories in a constructed public-goods game to test whether contextual improvements persist when historical statistical patterns change (Findings of EMNLP, 2026).

- **[Decentralised Coordination of Low-Power Embedded Devices Using the Max-Sum Algorithm](https://profs.scienze.univr.it/~farinelli/pubs/farinelli-AAMAS-08.pdf)**: Farinelli, Rogers, Petcu, and Jennings use factor-graph message passing for approximate decentralized utility optimization. Evaluation includes graph coloring and a sensor-node implementation (AAMAS, 2008).

- **[Autonomous Agents for Collaborative Task under Information Asymmetry](https://papers.nips.cc/paper/2024/hash/0534abc9e6db91683d82186ef0d68202-Abstract-Conference.html)**: Liu et al. introduce iAgents and InformativeBench to study task completion when agents access different users’ information and communicate to retrieve relevant evidence (NeurIPS, 2024).

- **[The Architecture of Complexity](https://pdodds.w3.uvm.edu/research/papers/others/1962/simon1962a.pdf)**: Herbert A. Simon analyzes hierarchy and near-decomposability in complex systems, including stronger interactions within subsystems. This is conceptual background for modular organization (1962).
- **[Multi-Agent Teams Hold Experts Back](https://proceedings.mlr.press/v306/pappu26a.html)**: Pappu et al. evaluate whether self-organizing LLM teams match their strongest member and examine failures to use identified expertise across tested teams and benchmarks (ICML, 2026).
- **[Beyond the All-in-One Agent: Benchmarking Role-Specialized Multi-Agent Collaboration in Enterprise Workflows](https://arxiv.org/abs/2605.08761)**: Yu et al. introduce EntCollabBench, a simulated organization with permission-separated roles, state-changing workflows, and policy-based approval tasks. Evaluation uses execution traces, database checks, and deterministic policy adjudication (2026 preprint).

- **[Transactive Memory: A Contemporary Analysis of the Group Mind](https://dtg.sites.fas.harvard.edu/DANWEGNER/pub/Wegner%20Transactive%20Memory.pdf)**: Daniel M. Wegner describes human-group memory as individual memory systems linked by communication, including knowledge of who stores particular information (1987).
- **[Grounding Collaborative Agents in Group Cognition](https://arxiv.org/abs/2611.29036)**: Tan et al. evaluate briefs for agents entering ongoing teams through reference-point coverage and downstream collaboration simulations across four domains (2026 preprint).
- **[TeamFusion: Supporting Open-ended Teamwork with Multi-Agent Systems](https://aclanthology.org/2026.acl-long.657/)**: Liu et al. use preference-conditioned proxy agents and structured discussion to synthesize team deliverables. They evaluate representation of members’ views on two open-ended tasks (ACL, 2026).

- **[PEAR: Planner-Executor Agent Robustness Benchmark](https://aclanthology.org/2026.findings-eacl.237/)**: Dong et al. evaluate clean-task performance and adversarial robustness in planner–executor systems, comparing component capabilities, memory placement, and attack targets across tested configurations (Findings of EACL, 2026).

- **[A Brief History of Stigmergy](https://static.ias.edu/pitp/archive/2012files/29.pdf)**: Guy Theraulaz and Eric Bonabeau explain coordination through environmental modifications and distinguish quantitative from qualitative stigmergy in social insects (Artificial Life, 1999).
- **[More Capable, Less Cooperative? When LLMs Fail at Zero-Cost Collaboration](https://proceedings.mlr.press/v306/yadav26a.html)**: Yadav, Black, and Sourbut evaluate information sharing when cooperation carries no modeled cost. Interventions distinguish communication competence from cooperation failures in their turn-based environment (ICML, 2026).
- **[ClawArena-Team: Benchmarking Subagent Orchestration and Dynamic Workflows in Language-Model Agents](https://arxiv.org/abs/2606.31174)**: Xiong et al. evaluate subagent management through 41 staged scenarios, including delegation, workspace permissions, and modality routing, with a fixed subagent pool (2026 preprint).

- **[Elements of a Plan-Based Theory of Speech Acts](https://onlinelibrary.wiley.com/doi/abs/10.1207/s15516709cog0303_1)**: Philip R. Cohen and C. Raymond Perrault model requesting and informing as planning operators and integrate communicative and physical actions within plans (Cognitive Science, 1979).
- **[Open Agent Specification: Enabling Cross-Framework Comparison of AI Agents](https://doi.org/10.1145/3786335.3813130)**: Amini et al. introduce a declarative agent specification and compare shared designs across LangGraph, CrewAI, AutoGen, and WayFlow on three benchmarks. Shared specifications preserve intended structure without requiring identical runtime behavior (ACM CAIS, 2026).

- **[The Bargaining Problem](https://jmvidal.cse.sc.edu/library/nash50a.pdf)**: John F. Nash, Jr. develops an axiomatic solution to two-person bargaining (Econometrica, 1950).
- **[Cooperation, Competition, and Maliciousness: LLM-Stakeholders Interactive Negotiation](https://proceedings.neurips.cc/paper_files/paper/2024/hash/984dd3db213db2d1454a163b65b84d08-Abstract.html)**: Abdelnabi et al. introduce scored multi-party, multi-issue negotiation games and evaluate agreement, role adherence, and interactions with greedy or adversarial participants (NeurIPS, 2024).
- **[Scaling Inference-Time Computation via Opponent Simulation: Enabling Online Strategic Adaptation in Repeated Negotiation](https://proceedings.mlr.press/v306/liu26ef.html)**: Liu et al. combine an in-context opponent model with simulated best-of-N responses to study adaptation across two forms of repeated negotiation games without parameter updates (ICML, 2026).

- **[Cooperative Coevolution: An Architecture for Evolving Coadapted Subcomponents](https://sci2s.ugr.es/sites/default/files/files/Teaching/OtherPostGraduateCourses/Metaheuristicas/ecj00.pdf)**: Potter and De Jong evolve interacting solution components in separate cooperating species. They study emergent decomposition through string matching and neural-network evolution (Evolutionary Computation, 2000).
- **[Investigating Component Contributions in Multi-Agent ML Systems](https://proceedings.mlr.press/v306/kim26ba.html)**: Kim et al. compare coordination, iterative refinement, memory, and planning in ML engineering agents through architectural ablations. They introduce K-live, a benchmark using 25 active competitions (ICML, 2026).

- **[An Iterative Method of Solving a Game](https://cs.brown.edu/courses/csci1440/labs/2023/lab01/robinson.pdf)**: Julia Robinson proves convergence of Brown’s fictitious-play procedure for empirical mixed strategies in finite two-player zero-sum games (Annals of Mathematics, 1951).
- **[Multi-Agent Reinforcement Learning: Independent vs. Cooperative Agents](https://web.mit.edu/16.412j/www/html/Advanced%20lectures/2004/Multi-AgentReinforcementLearningIndependentVersusCooperativeAgents.pdf)**: Ming Tan compares independent learners with agents sharing sensations, episodes, or learned policies and examines learning gains and communication costs (ICML, 1993).
- **[LLawCo: Learning Laws of Cooperation for Modeling Embodied Multi-Agent Behavior](https://proceedings.mlr.press/v306/zhou26i.html)**: Zhou, Gan, and Cherian derive cooperation rules from failed interactions and incorporate them through supervised fine-tuning. Evaluation uses simulated communicative tasks in PARTNR-Dialog and TDW-MAT (ICML, 2026).

- **[Hierarchical Planning in a Distributed Environment](https://ijcai.org/proceedings/1979/41)**: Daniel D. Corkill distributes NOAH’s hierarchical planning, conflict criticism, and world-model mechanisms across planning processors, illustrated with small planning examples (IJCAI, 1979).
- **[Partial-Order Planning with Concurrent Interacting Actions](https://www.cs.cmu.edu/afs/cs/project/jair/pub/volume14/boutilier01a.pdf)**: Boutilier and Brafman introduce POMP, a sound and complete partial-order planner for concurrent interacting actions under their STRIPS-style model. Planning is centralized for cooperative agent teams (JAIR, 2001).
- **[The Decrypto Benchmark for Multi-Agent Reasoning and Theory of Mind](https://proceedings.mlr.press/v306/lupu26a.html)**: Lupu, Willi, and Foerster evaluate interactive multi-agent reasoning through a cooperative–competitive word game, including human–AI cross-play and targeted theory-of-mind tasks (ICML, 2026).

- **[ALLIANCE: An Architecture for Fault Tolerant Multi-Robot Cooperation](https://web.eecs.utk.edu/~leparker/publications/TRA.pdf)**: Lynne E. Parker introduces distributed, behavior-based action selection for heterogeneous robot teams performing loosely coupled subtasks. A physical-robot laboratory cleanup demonstration evaluates adaptive cooperation (IEEE Transactions on Robotics and Automation, 1998).
- **[Task Decomposition, Dynamic Role Assignment, and Low-Bandwidth Communication for Real-Time Strategic Teamwork](https://publications.ri.cmu.edu/storage/publications/pub_files/pub2/stone_peter_1999_1/stone_peter_1999_1.pdf)**: Stone and Veloso combine formations, dynamic role assignment, and low-bandwidth communication for teams with periodic full-communication opportunities. Evaluation uses homogeneous agents in simulated robotic soccer (Artificial Intelligence, 1999).

- **[CAST: Collaborative Agents for Simulating Teamwork](https://ijcai.org/proceedings/2001/151)**: Yen et al. represent shared team processes with Petri nets and anticipate teammates’ information needs for proactive communication. Evaluation uses synthetic software-agent teams (IJCAI, 2001).
- **[The RETSINA MAS Infrastructure](https://www.ri.cmu.edu/pub_files/2003/7/art-1024172719965.pdf)**: Sycara, Paolucci, Van Velsen, and Giampapa describe reusable services, communication conventions, and agent requirements for heterogeneous multi-agent systems (Autonomous Agents and Multi-Agent Systems, 2003).
- **[AgentArch: A Benchmark for Evaluating Agent Architectures in Enterprise Workflows](https://aclanthology.org/2026.aacl-long.44/)**: Bogavelli, Subramani, and Sharma compare 18 agent configurations across orchestration, prompting style, memory, and thinking tools on two enterprise workflows (AACL-IJCNLP, 2026).

- **[On social laws for artificial agent societies: off-line design](https://cris.technion.ac.il/en/publications/on-social-laws-for-artificial-agent-societies-off-line-design/)**: Shoham and Tennenholtz formalize coordination through constraints selected before execution and analyze the synthesis of useful social laws, including traffic rules for idealized mobile robots (Artificial Intelligence, 1995).
- **[ProtocolBench: Which LLM MultiAgent Protocol to Choose?](https://proceedings.mlr.press/v306/du26l.html)**: Du et al. compare agent communication protocols on task success, latency, message overhead, and recovery from injected failures in tested scenarios (ICML, 2026).
- **[Rethinking the Evaluation of Efficiency Methods for Multi-Agent Systems](https://aclanthology.org/2026.emnlp-main.798/)**: Zhang et al. evaluate representative multi-agent efficiency methods under shared models, agent definitions, and runtime. They test whether structural changes explain reported gains across controlled configurations (EMNLP, 2026).

- **[Reaching a Consensus](https://www.cse.cuhk.edu.hk/~cslui/CMSC5734/DeGroot-Reaching_a_concensus.pdf)**: Morris H. DeGroot models repeated linear pooling of subjective probability distributions and gives conditions for consensus, with explicit weights for the resulting common distribution (Journal of the American Statistical Association, 1974).
- **[From Debate to Decision: Conformal Social Choice for Safe Multi-Agent Deliberation](https://aclanthology.org/2026.emnlp-main.830/)**: Wang et al. calibrate aggregated agent probabilities into answer sets for action or escalation in multiple-choice reasoning tasks. Their marginal coverage guarantee assumes exchangeable calibration and test examples at a preselected round; it does not cover adaptive stopping (EMNLP, 2026).

- **[Pooling of Unshared Information in Group Decision Making: Biased Information Sampling During Discussion](https://www.uni-muenster.de/imperia/md/content/psyifp/aeechterhoff/vorlesungkommunikation/stasser_titus_unsharedinfogroupdisc_jpsp1985.pdf)**: Garold Stasser and William Titus study biased information sampling in human group discussions through a simulated political caucus. Shared information and existing preferences dominate discussion in the studied setting (Journal of Personality and Social Psychology, 1985).
- **[Aggregating Sets of Judgments: An Impossibility Result](https://ppettit.scholar.princeton.edu/sites/g/files/toruqf7426/files/documents/Aggregating_EconomicsandPhilosophy_2002.pdf)**: Christian List and Philip Pettit establish an impossibility result for aggregating logically connected judgments under specified rationality, domain, anonymity, and systematicity conditions (Economics and Philosophy, 2002).
- **[Debate or Vote: Which Yields Better Decisions in Multi-Agent Large Language Models?](https://proceedings.neurips.cc/paper_files/paper/2025/hash/934252acd87f254d5d4672fbde283bd2-Abstract-Conference.html)**: Choi, Zhu, and Li separate voting from inter-agent discussion across seven NLP benchmarks and examine their respective contributions to debate performance (NeurIPS, 2025).

- **[Cooperate to Compete: Strategic Coordination in Multi-Agent Conquest](https://aclanthology.org/2026.emnlp-main.609/)**: O’Neill et al. evaluate negotiation and shifting alliances in a conquest game with secret objectives, partial observability, and nonbinding agreements, including human–AI games (EMNLP, 2026).
- **[ProMediate: A Simulation Testbed for Evaluating Proactive Mediation in Multi-Party Negotiation](https://aclanthology.org/2026.findings-acl.1479/)**: Liu et al. evaluate when and how mediator agents intervene in simulated negotiations involving several parties and topics. Metrics include consensus changes and intervention latency (Findings of ACL, 2026).

- **[Counterspeculation, Auctions, and Competitive Sealed Tenders](https://cramton.umd.edu/market-design-papers/vickrey-counterspeculation-auctions-and-competitive-sealed-tenders.pdf)**: William Vickrey analyzes auction rules, including incentives to bid private values when the highest bidder pays the second-highest bid, assuming no bidder collusion (The Journal of Finance, 1961).
- **[Perfect Equilibrium in a Bargaining Model](https://arielrubinstein.org/papers/11.pdf)**: Ariel Rubinstein studies perfect equilibrium in two-player alternating-offer bargaining with costs of delay (Econometrica, 1982).

- **[Time, Clocks, and the Ordering of Events in a Distributed System](https://lamport.azurewebsites.net/pubs/time-clocks.pdf)**: Leslie Lamport defines causal event ordering and logical clocks for coordinating message-passing processes (Communications of the ACM, 1978).
- **[Impossibility of Distributed Consensus with One Faulty Process](https://groups.csail.mit.edu/tds/papers/Lynch/jacm85.pdf)**: Fischer, Lynch, and Paterson prove that deterministic consensus cannot guarantee termination in a fully asynchronous system with reliable messages and even one possible process crash (JACM, 1985).
- **[Designing a Family of Coordination Algorithms](https://cdn.aaai.org/ICMAS/1995/ICMAS95-010.pdf)**: Decker and Lesser introduce Generalized Partial Global Planning, modular mechanisms that coordinate cooperative agents by constraining their local schedules through exchanged task information and commitments (ICMAS, 1995).
- **[Systematic Failures in Collective Reasoning under Distributed Information in Multi-Agent LLMs](https://proceedings.mlr.press/v306/li26ej.html)**: Li, Naito, and Shirado introduce HiddenBench, using 65 hidden-profile tasks to study whether agent groups discover and combine separately held information (ICML, 2026).

- **[TarMAC: Targeted Multi-Agent Communication](https://proceedings.mlr.press/v97/das19a.html)**: Das et al. learn message contents and recipients from task rewards, with multiple communication rounds before actions in partially observable multi-agent tasks (ICML, 2019).
- **[Learning when to Communicate at Scale in Multiagent Cooperative and Competitive Tasks](https://arxiv.org/abs/1812.09755)**: Singh, Jain, and Sukhbaatar introduce IC3Net, which learns communication timing through a gating mechanism and uses individualized rewards across cooperative, competitive, and mixed tasks (ICLR, 2019).
- **[Async-RBench: Benchmarking Asynchronous Task Execution in LLM Agents](https://arxiv.org/abs/2610.32429)**: Zeng et al. evaluate responses to asynchronous subagent results through 200 executable tasks with controlled delivery and explicit response contracts (2026 preprint).

- **[Grounding in Communication](https://web.stanford.edu/~clark/1990s/Clark%2C%20H.H.%20_%20Brennan%2C%20S.E.%20_Grounding%20in%20communication_%201991.pdf)**: Herbert H. Clark and Susan E. Brennan describe how human participants establish sufficient evidence of understanding, with grounding shaped by purpose and communication medium (1991).
- **[How a Cockpit Remembers Its Speeds](https://pages.ucsd.edu/~ehutchins/documents/CockpitSpeeds.pdf)**: Edwin Hutchins analyzes cockpit memory as information represented and propagated across pilots and instruments (Cognitive Science, 1995).
- **[Learning to Share: Selective Memory for Efficient Parallel Agentic Systems](https://proceedings.mlr.press/v306/fioresi26a.html)**: Fioresi et al. learn which intermediate results parallel agent teams should add to shared memory. They evaluate information reuse and runtime on AssistantBench and GAIA (ICML, 2026).
- **[Dialogue is the Plan: From Interface to Joint Action in Agentic AI](https://aclanthology.org/2026.acl-short.63/)**: Inan, Alikhani, and Sicilia connect dialogue theory with agent architectures and propose explicit shared commitments, clarification actions, and measures of grounding and repair (ACL, 2026; conceptual paper).

- **[A Counterexample in Stochastic Optimum Control](https://mcrotk.github.io/courses/references/counterexample.pdf)**: Hans S. Witsenhausen constructs a decentralized control problem where nonlinear policies outperform linear policies despite linear dynamics, Gaussian uncertainty, and quadratic costs (1968).
- **[Multi-Agent Reinforcement Learning with Communication-Constrained Priors](https://proceedings.neurips.cc/paper_files/paper/2025/hash/e26502ce357ce3015e8778f0e85d4b39-Abstract-Conference.html)**: Yang et al. model communication constraints and distinguish lossy from lossless messages when training cooperative multi-agent policies (NeurIPS, 2025).
- **[Unifying Partner and Environment Diversity to Improve Human-AI Coordination](https://arxiv.org/abs/2611.32031)**: Zhang et al. combine partner-population and environment diversity during training. They evaluate coordination with held-out partners and environments in foraging and Overcooked tasks (2026 preprint).

- **[Cooperative Pathfinding](https://cdn.aaai.org/AIIDE/2005/AIIDE05-020.pdf)**: David Silver introduces Cooperative A*, Hierarchical Cooperative A*, and Windowed Hierarchical Cooperative A* for non-colliding routes, assuming access to other agents’ planned routes (AIIDE, 2005).
- **[AI, Take the Wheel: What Drives Delegation and Trust in Human–Computer Cooperative Question Answering?](https://aclanthology.org/2026.findings-acl.422/)**: Gor et al. study delegation and answer adoption in mixed human–AI trivia teams across 24 tournament matches (Findings of ACL, 2026).

- **[The Dynamics of Reinforcement Learning in Cooperative Multiagent Systems](https://cdn.aaai.org/AAAI/1998/AAAI98-106.pdf)**: Claus and Boutilier compare independent and joint-action learners and study how game structure and exploration affect equilibrium selection in cooperative repeated games (AAAI, 1998).
- **[Demystifying Multi-Agent Debate: The Role of Confidence and Diversity](https://aclanthology.org/2026.findings-acl.1694/)**: Zhu et al. analyze initial-answer diversity and calibrated confidence in debate. They compare interventions with vanilla debate and majority voting across six reasoning benchmarks (Findings of ACL, 2026).

- **[The Byzantine Generals Problem](https://lamport.azurewebsites.net/pubs/byz.pdf)**: Lamport, Shostak, and Pease establish agreement protocols and fault-tolerance limits when participants may send conflicting information, under specified communication and authentication assumptions (1982).
- **[Efficiency of Experimental Security Markets with Insider Information: An Application of Rational-Expectations Models](https://www.journals.uchicago.edu/doi/10.1086/261084)**: Plott and Sunder test information revelation in laboratory security markets containing informed insiders under repeated market conditions (Journal of Political Economy, 1982).

- **[Learning Decentralized LLM Collaboration with Multi-Agent Actor Critic](https://proceedings.mlr.press/v306/liu26k.html)**: Liu et al. compare centralized and decentralized critics for training decentralized LLM teams across writing, coding, and game-playing tasks (ICML, 2026).
- **[Advancing Language Multi-Agent Learning with Credit Re-Assignment for Interactive Environment Generalization](https://proceedings.colm.cc/paper_files/paper/2025/hash/80e354fdac2c7fbf439a51f4853edbac-Abstract-Conference.html)**: He et al. train role-free language agents using reassigned process rewards and synthesized preferences. They evaluate collaboration across interactive environments (COLM, 2025 pre-proceedings).

- **[Particle Swarm Optimization](https://faculty.washington.edu/paymana/swarm/kennedy95-ijcnn.pdf)**: Kennedy and Eberhart introduce a population-based method for nonlinear function optimization, an adjacent foundation for collective search (ICNN, 1995).
- **[Human-level performance in 3D multiplayer games with population-based reinforcement learning](https://discovery.ucl.ac.uk/id/eprint/10076318/)**: Jaderberg et al. train populations for Capture the Flag and evaluate agents with unfamiliar teammates and opponents, including human players (Science, 2019).
- **[The Hanabi Challenge: A New Frontier for AI Research](https://research.google/pubs/the-hanabi-challenge-a-new-frontier-for-ai-research/)**: Bard et al. establish Hanabi as an imperfect-information cooperation challenge, release its learning environment, and propose evaluation protocols for agent teams (Artificial Intelligence, 2020).

- **[Multiagent Planning with Factored MDPs](https://proceedings.neurips.cc/paper_files/paper/2001/file/7af6266cc52234b5aa339b16695f7fc4-Paper.pdf)**: Guestrin, Koller, and Parr use factored value functions and coordination-graph message passing to select cooperative joint actions under an approximate value function (NeurIPS, 2001).
- **[Dynamic Programming for Partially Observable Stochastic Games](https://cdn.aaai.org/AAAI/2004/AAAI04-112.pdf)**: Hansen, Bernstein, and Zilberstein combine dynamic programming with elimination of dominated strategies for finite-horizon partially observable games, including optimal solution computation for the common-payoff case (AAAI, 2004).

- **[Sharp Transition towards Shared Vocabularies in Multi-Agent Systems](https://www.codebiology.org/pdf/%5B3%5D%20Baronchelli%20et%20al%20%282006%29.pdf)**: Baronchelli, Felici, Loreto, Caglioti, and Steels study shared naming conventions produced by local language games without central control in a simplified agent model (2006).
- **[Towards Open Ad Hoc Teamwork Using Graph-based Policy Learning](https://proceedings.mlr.press/v139/rahman21a.html)**: Rahman et al. learn teammate and joint-action value models for collaboration when agents with fixed policies enter and leave without advance notice (ICML, 2021).
- **[N-agent Ad Hoc Teamwork](https://proceedings.neurips.cc/paper_files/paper/2024/hash/cabf611498431ad89a85ace75f790d93-Abstract-Conference.html)**: Wang et al. formalize ad hoc teamwork with multiple controlled agents and varying teammates, then evaluate policy optimization with learned teammate representations (NeurIPS, 2024).

- **[Social Influence as Intrinsic Motivation for Multi-Agent Deep Reinforcement Learning](https://proceedings.mlr.press/v97/jaques19a.html)**: Jaques et al. reward agents for counterfactually estimated influence on other agents’ actions and evaluate coordination and learned communication in social dilemmas (ICML, 2019).
- **[Learning to Incentivize Other Learning Agents](https://proceedings.neurips.cc/paper/2020/hash/ad7ed5d47b9baceb12045a929e7e2f66-Abstract.html)**: Yang et al. learn incentive functions that transfer rewards between agents and account for their effects on recipients’ learning in general-sum Markov games (NeurIPS, 2020).

- **[AgentAsk: Multi-Agent Systems Need to Ask](https://aclanthology.org/2026.acl-long.1294/)**: Lin et al. classify errors at inter-agent handoffs and train clarification interventions that balance accuracy, communication cost, and latency (ACL, 2026).

- **[How Social Influence Can Undermine the Wisdom of Crowd Effect](https://pmc.ncbi.nlm.nih.gov/articles/PMC3107299/)**: Lorenz, Rauhut, Schweitzer, and Helbing find that exposure to others’ estimates reduces diversity without improving collective error in their human estimation experiment (PNAS, 2011).
- **[Network Dynamics of Social Influence in the Wisdom of Crowds](https://ndg.asc.upenn.edu/wp-content/uploads/2017/06/PNAS-2017-1615978114-Collective-Intelligence.pdf)**: Becker, Brackbill, and Centola compare centralized and decentralized influence networks in human estimation tasks. They find improved accuracy in decentralized networks under the studied conditions (PNAS, 2017).
- **[Dota 2 with Large Scale Deep Reinforcement Learning](https://arxiv.org/abs/1912.06680)**: OpenAI describes the distributed self-play system and continual-training methods used to train OpenAI Five for team-based Dota 2 (2019).
- **[α-Rank: Multi-Agent Evaluation by Evolution](https://arxiv.org/abs/1903.01373)**: Omidshafiei et al. introduce α-Rank, an evolutionary game-theoretic method for evaluating and ranking interacting agent policies (Scientific Reports, 2019).

- **[Nash Q-Learning for General-Sum Stochastic Games](https://www.jmlr.org/papers/v4/hu03a.html)**: Hu and Wellman extend Q-learning through joint-action values and Nash-equilibrium updates, with convergence guarantees restricted to specified stage games (JMLR, 2003).
- **[Multiagent Learning Using a Variable Learning Rate](https://publications.ri.cmu.edu/multiagent-learning-using-a-variable-learning-rate)**: Bowling and Veloso introduce the WoLF principle for varying learning rates against adapting opponents. Their theoretical self-play convergence result concerns a restricted class of iterated matrix games (2002).
- **[Multi-agent Reinforcement Learning in Sequential Social Dilemmas](https://www.ifaamas.org/Proceedings/aamas2017/pdfs/p464.pdf)**: Leibo et al. introduce sequential social dilemmas and study how learned cooperation changes with environmental conditions in Gathering and Wolfpack games (AAMAS, 2017).
- **[Inequity aversion improves cooperation in intertemporal social dilemmas](https://proceedings.neurips.cc/paper_files/paper/2018/hash/7fea637fd6d02b8f0adf6f7dc36aed93-Abstract.html)**: Hughes et al. incorporate inequity-averse preferences into Markov-game agents and examine their effects on cooperation and temporal credit assignment (NeurIPS, 2018).

- **[Coordination of Groups of Mobile Autonomous Agents Using Nearest Neighbor Rules](https://www.mit.edu/~jadbabai/papers/JadLiMorseTAC_June03.pdf)**: Jadbabaie, Lin, and Morse prove heading convergence under local averaging and sufficiently frequent joint connectivity in noise-free agent models (2003).
- **[Consensus Problems in Networks of Agents with Switching Topology and Time-Delays](https://www.cds.caltech.edu/~murray/papers/2003f_om04-tac.html)**: Olfati-Saber and Murray develop consensus protocols and convergence analysis for switching networks and communication delays under separate graph and timing assumptions (2004).
- **[A Unified Game-Theoretic Approach to Multiagent Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2017/hash/3323fe11e9595c09af38fe67567a9394-Abstract.html)**: Lanctot et al. introduce policy-space response oracles, combining learned responses to policy mixtures with empirical game-theoretic strategy selection (NeurIPS, 2017).
- **[Emergent Tool Use From Multi-Agent Autocurricula](https://arxiv.org/abs/1909.07528)**: Baker et al. study how competing hide-and-seek teams develop successive strategies involving tools and coordination in a physics simulator (ICLR, 2020).

- **[Novel Type of Phase Transition in a System of Self-Driven Particles](https://www.uio.no/studier/emner/matnat/fys/FYS4715/h25/ch3-5_motion/src/vicsek1995.pdf)**: Vicsek et al. model collective motion through constant-speed particles that align with neighboring directions under noise (Physical Review Letters, 1995).
- **[Effective Leadership and Decision-Making in Animal Groups on the Move](https://pdodds.w3.uvm.edu/teaching/courses/2009-08UVM-300/docs/others/everything/couzin2005a.pdf)**: Couzin, Krause, Franks, and Levin model how informed minorities can guide group movement without explicit signaling or identification of informed individuals (Nature, 2005).
- **[MALT: Improving Reasoning with Multi-Agent LLM Training](https://arxiv.org/abs/2412.01928)**: Motwani et al. train role-specialized generation, verification, and refinement agents using rewards propagated through sampled reasoning trees. They evaluate the method on MATH, GSM8K, and CSQA (COLM, 2025).
- **[Emergent social conventions and collective bias in LLM populations](https://www.lajello.com/papers/sciadv25emergent.pdf)**: Ashery, Aiello, and Baronchelli study shared naming conventions, collective bias, and convention changes driven by committed minorities in interacting LLM populations (Science Advances, 2025).

- **[A Market-Oriented Programming Environment and its Application to Distributed Multicommodity Flow Problems](https://arxiv.org/abs/cs/9308102)**: Michael P. Wellman introduces WALRAS, a computational market environment for resource allocation through competitive price equilibria under specified economic assumptions (JAIR, 1993).
- **[Sold!: Auction Methods for Multirobot Coordination](https://ai.stanford.edu/~gerkey/research/final_papers/tra01.pdf)**: Gerkey and Matarić implement MURDOCH’s dynamic auction-based task allocation and evaluate coordination among physical robots (2002).
- **[Don’t lie to your friends: Learning what you know from collaborative self-play](https://proceedings.colm.cc/paper_files/paper/2025/hash/2ea07a4acbf7e38913062fd69a70805f-Abstract-Conference.html)**: Eisenstein et al. train small agent groups with shared rewards and different retrieval tools. They study transfer to single-agent tool use and selective answering (COLM, 2025 pre-proceedings).

- **[An Analysis of Formal Inter-Agent Dialogues](https://www.sci.brooklyn.cuny.edu/~parsons/publications/conferences/aamas02c.pdf)**: Parsons, Wooldridge, and Amgoud define argument-exchange protocols and analyze how agent attitudes affect termination and complexity in formal-language dialogues (AAMAS, 2002).
- **[Why Do Humans Reason? Arguments for an Argumentative Theory](https://www.dan.sperber.fr/wp-content/uploads/2011_mercier_why-do-humans-reason.pdf)**: Mercier and Sperber propose that producing and evaluating arguments is a central function of human reasoning. Transfer of this cognitive theory to AI teams is unverified (2011).
- **[Should we be going MAD? A Look at Multi-Agent Debate Strategies for LLMs](https://proceedings.mlr.press/v235/smit24a.html)**: Smit et al. compare debate and prompting strategies through accuracy, cost, and time. They examine sensitivity to protocol settings and agent agreement (ICML, 2024).
- **[Multi-Agent Verification: Scaling Test-Time Compute with Multiple Verifiers](https://arxiv.org/abs/2502.20379)**: Lifshitz, McIlraith, and Du combine best-of-n sampling with multiple aspect-specific verifiers to evaluate candidate answers at inference time (COLM, 2025).

- **[Agent-Oriented Programming](https://cse-robotics.engr.tamu.edu/dshell/cs631/papers/shoham93agent.pdf)**: Yoav Shoham defines agent programs through formally represented beliefs, decisions, capabilities, obligations, and typed communication, with an implemented interpreter (1993).
- **[The Gaia Methodology for Agent-Oriented Analysis and Design](https://www.cs.ox.ac.uk/people/michael.wooldridge/pubs/jaamas2000b.pdf)**: Wooldridge, Jennings, and Kinny model multiagent organizations through roles, responsibilities, permissions, and interaction protocols. This version assumes static relationships and capabilities and excludes true conflicts between component goals (2000).
- **[Post-training for Efficient Communication via Convention Formation](https://arxiv.org/abs/2508.06482)**: Hua, Wang, and Artzi study post-training for communication conventions through reference-game and document-grounded interaction benchmarks (COLM, 2025).

- **[Labeling Images with a Computer Game](https://www.cs.cmu.edu/~biglou/ESP.pdf)**: Luis von Ahn and Laura Dabbish introduce the ESP Game, in which paired human players’ matching descriptions produce image labels (CHI, 2004).
- **[reCAPTCHA: Human-Based Character Recognition via Web Security Measures](https://www.cs.cmu.edu/~biglou/reCAPTCHA_Science.pdf)**: Von Ahn, Maurer, McMillen, Abraham, and Blum combine control questions, repeated human responses, and OCR outputs to transcribe scanned words during security checks (Science, 2008).
- **[Mean Field Multi-Agent Reinforcement Learning](https://proceedings.mlr.press/v80/yang18d.html)**: Yang et al. approximate population interactions through average neighboring behavior and develop mean-field Q-learning and actor-critic algorithms (ICML, 2018).
- **[Learning with Opponent-Learning Awareness](https://ifaamas.org/Proceedings/aamas2018/pdfs/p122.pdf)**: Foerster et al. introduce LOLA, which accounts for how an agent’s policy influences other agents’ learning updates, with experiments on repeated games and a gridworld social dilemma (AAMAS, 2018).

- **[Bagging Predictors](https://link.springer.com/article/10.1007/BF00058655)**: Leo Breiman combines predictors trained on bootstrap samples through averaging or plurality voting, an adjacent foundation for aggregation of multiple predictions (1996).
- **[A Decision-Theoretic Generalization of On-Line Learning and an Application to Boosting](https://www.schapire.net/papers/FreundSc95.pdf)**: Freund and Schapire develop multiplicative-weight allocation under bounded losses and AdaBoost for combining weak learners, an adjacent ensemble-learning foundation (1997).
- **[From One to Many: Planning for Loosely Coupled Multi-Agent Systems](https://cdn.aaai.org/ICAPS/2008/ICAPS08-004.pdf)**: Brafman and Domshlak formalize how agent coupling affects cooperative planning complexity and develop planning methods that exploit limited interactions under their STRIPS-based model (ICAPS, 2008).

- **[Knowledge and Common Knowledge in a Distributed Environment](https://groups.csail.mit.edu/tds/papers/Halpern/JACM90.pdf)**: Halpern and Moses formalize group knowledge and its role in coordinated action, including attainable weaker forms of common knowledge under specified communication and timing models (JACM, 1990).
- **[Agreeing to Disagree](https://www.haverford.edu/sites/default/files/Aumann1976.pdf)**: Robert J. Aumann proves that two agents with a common prior and common knowledge of their posterior probabilities for the same event must assign it equal probabilities (1976).

- **[The Distributed Constraint Satisfaction Problem: Formalization and Algorithms](https://jmvidal.cse.sc.edu/library/yokoo98a.pdf)**: Yokoo, Durfee, Ishida, and Kuwabara formalize distributed constraint satisfaction and develop asynchronous backtracking and weak-commitment search for coordinating consistent agent decisions (1998).
- **[Adopt: Asynchronous Distributed Constraint Optimization with Quality Guarantees](https://robots.isi.edu/prl/modi2005adopt-asynchronous-distributed-constraint.pdf)**: Modi, Shen, Tambe, and Yokoo introduce asynchronous optimization with optimality and bounded-error guarantees under their distributed constraint optimization model (2005).
- **[A Scalable Method for Multiagent Constraint Optimization](https://ijcai.org/proceedings/2005/21)**: Petcu and Faltings introduce DPOP’s pseudotree-based utility propagation. Message count is linear, and maximum message size depends on induced width (IJCAI, 2005).
- **[“Other-Play” for Zero-Shot Coordination](https://proceedings.mlr.press/v119/hu20a.html)**: Hu et al. introduce other-play to reduce dependence on arbitrary self-play conventions and evaluate coordination with unfamiliar agents and humans in Hanabi (ICML, 2020).
- **[Off-Belief Learning](https://proceedings.mlr.press/v139/hu21c.html)**: Hu et al. train cooperative policies using a fixed policy for interpreting past actions, with controlled reasoning levels and zero-shot coordination experiments in Hanabi (ICML, 2021).
- **[Collaborating with Humans without Human Data](https://proceedings.neurips.cc/paper/2021/hash/797134c3e42371bb4979a462eb2f042a-Abstract.html)**: Strouse et al. introduce Fictitious Co-Play. Policies train against diverse self-play partners and historical checkpoints, then are evaluated with unfamiliar agents and humans in a collaborative cooking simulator (NeurIPS, 2021).

- **[Towards Flexible Teamwork](https://arxiv.org/abs/cs/9709101)**: Milind Tambe introduces STEAM, an implemented teamwork model with team monitoring, reorganization, and selective communication (JAIR, 1997).
- **[A Formal Analysis and Taxonomy of Task Allocation in Multi-Robot Systems](https://ai.stanford.edu/~gerkey/research/final_papers/mrta-taxonomy.pdf)**: Gerkey and Matarić classify multi-robot task-allocation problems and relate them to optimization methods. The analysis assumes independently assignable tasks (2004).
- **[Cross-environment Cooperation Enables Zero-shot Multi-agent Coordination](https://proceedings.mlr.press/v267/jha25b.html)**: Jha et al. train cooperation across procedurally generated environments and evaluate coordination with unfamiliar partners, including humans (ICML, 2025).

- **[Learning Multiagent Communication with Backpropagation](https://papers.neurips.cc/paper/2016/hash/55b1927fdafef39c48e5b73b5d61ea60-Abstract.html)**: Sukhbaatar, Szlam, and Fergus introduce CommNet, which jointly learns continuous communication and agent policies for fully cooperative tasks (NeurIPS, 2016).
- **[Multi-Agent Cooperation and the Emergence of (Natural) Language](https://arxiv.org/abs/1612.07182)**: Lazaridou, Peysakhovich, and Baroni study learned communication in image referential games and methods for grounding the resulting symbols in natural language (2017).
- **[Emergence of Grounded Compositional Language in Multi-Agent Populations](https://cdn.aaai.org/ojs/11492/11492-13-15020-1-2-20201228.pdf)**: Mordatch and Abbeel study discrete compositional communication and nonverbal coordination in a physically situated cooperative environment (AAAI, 2018).
- **[GPTSwarm: Language Agents as Optimizable Graphs](https://proceedings.mlr.press/v235/zhuge24a.html)**: Zhuge et al. represent language agents as composable computational graphs and optimize prompts and inter-agent connections (ICML, 2024).
- **[A Dynamic LLM-Powered Agent Network for Task-Oriented Agent Collaboration](https://arxiv.org/abs/2310.02170)**: Liu et al. introduce DyLAN, which selects agent teams through preliminary trials and adjusts communication during task solving (2024).
- **[AgentDropout: Dynamic Agent Elimination for Token-Efficient and High-Performance LLM-Based Multi-Agent Collaboration](https://aclanthology.org/2025.acl-long.1170/)**: Wang et al. learn round-specific collaboration graphs that remove redundant agents and messages. They evaluate task performance and token use (ACL, 2025).

- **[Maximum Likelihood Estimation of Observer Error-Rates Using the EM Algorithm](https://crowdsourcing-class.org/readings/downloads/ml/EM.pdf)**: Dawid and Skene estimate observer-specific errors without known true labels, providing a statistical model for aggregating fallible judgments (1979).
- **[Strategy-Proofness and Arrow’s Conditions: Existence and Correspondence Theorems for Voting Procedures and Social Welfare Functions](https://www.kellogg.northwestern.edu/~/media/Files/Faculty/Research/ArticlesBookChaptersWorkingPapers/Strategy%20Proofness.ashx)**: Mark Allen Satterthwaite establishes limits on truthful preference aggregation under formal voting assumptions (1975).

- **[A Universal Modular ACTOR Formalism for Artificial Intelligence](https://ijcai.org/proceedings/1973/31)**: Hewitt, Bishop, and Steiger introduce computational actors that interact through messages (IJCAI, 1973).
- **[Social Interaction Breaks Replicate Independence in Controlled-Clone LLM Agents](https://arxiv.org/abs/2611.29581)**: Zheng, Luo, and Luu use matched controlled-clone experiments to study how interaction changes response profiles and affects independence assumptions in multi-agent evaluation (2026 preprint).
- **[From Local Errors to System Failures: Modeling and Benchmarking Error Propagation in Multi-Agent LLM Systems](https://arxiv.org/abs/2611.31063)**: Yu et al. introduce REPA and ErrPropBench-10 to model error propagation through agent workflows and evaluate targeted recovery (2026 preprint).

- **[Intention Is Choice with Commitment](https://cs.stanford.edu/~epacuit/classes/lori-spr09/cohenlevesque-intention-aij90.pdf)**: Cohen and Levesque formalize relationships among beliefs, goals, actions, and persistent commitments, including conditions for abandoning intentions (1990).
- **[Commitments and conventions: The foundation of coordination in multi-agent systems](https://maxapress.com/data/article/ker/preview/pdf/S0269888900000205.pdf)**: Nick R. Jennings models coordination through commitments and conventions for reassessing them as circumstances change (1993).

- **[SOTOPIA-π: Interactive Learning of Socially Intelligent Language Agents](https://aclanthology.org/2024.acl-long.698/)**: Wang et al. train language agents through behavior cloning and self-reinforcement on filtered social interactions, with human and model-based evaluation (ACL, 2024).

- **[Stay Focused: Problem Drift in Multi-Agent Debate](https://aclanthology.org/2026.findings-eacl.268/)**: Becker et al. study how debates depart from the initial problem and evaluate methods to detect and mitigate that drift (Findings of EACL, 2026).

- **[The Complexity of Decentralized Control of Markov Decision Processes](https://people.cs.umass.edu/~immerman/pub/bgiz.pdf)**: Bernstein, Givan, Immerman, and Zilberstein establish computational complexity limits for decentralized multi-agent decision-making under partial information (2002).
- **[Using Partial Global Plans to Coordinate Distributed Problem Solvers](https://ijcai.org/proceedings/1987/183)**: Durfee and Lesser coordinate distributed problem solvers through selectively exchanged local-plan summaries (IJCAI, 1987).
- **[Stop Overvaluing Multi-Agent Debate -- We Must Rethink Evaluation and Embrace Model Heterogeneity](https://arxiv.org/abs/2502.08788)**: Zhang et al. compare multi-agent debate methods with single-agent baselines and examine the role of model heterogeneity (2025).

- **[Flocks, Herds, and Schools: A Distributed Behavioral Model](https://www.red3d.com/cwr/papers/1987/boids.html)**: Craig W. Reynolds demonstrates coordinated group motion from independent actors with local perception and simple behavioral rules (SIGGRAPH, 1987).
- **[Ant System: Optimization by a Colony of Cooperating Agents](https://difusion.ulb.ac.be/vufind/Record/ULB-DIPOT:oai:dipot.ulb.ac.be:2013/74581/Details)**: Dorigo, Maniezzo, and Colorni introduce an optimization method in which simple agents coordinate indirectly through pheromone-like shared information (1996).

- **[Adaptive Mixtures of Local Experts](https://www.cs.toronto.edu/~hinton/absps/jjnh91.pdf)**: Jacobs, Jordan, Nowlan, and Hinton introduce learned routing among specialist networks, an architectural foundation for specialization and aggregation (1991).
- **[On the acceptability of arguments and its fundamental role in nonmonotonic reasoning, logic programming and n-person games](https://cse-robotics.engr.tamu.edu/dshell/cs631/papers/dung95acceptability.pdf)**: Phan Minh Dung introduces abstract argumentation frameworks for reasoning about attacks between arguments and the acceptability of sets of arguments (1995).

- **[Markov games as a framework for multi-agent reinforcement learning](https://aima.eecs.berkeley.edu/~russell/classes/cs294/f21/papers/Littman_ICML94_Markov_Games.pdf)**: Michael L. Littman formulates multi-agent reinforcement learning through Markov games and presents minimax-Q for two-player zero-sum settings (ICML, 1994).
- **[Counterfactual Multi-Agent Policy Gradients](https://arxiv.org/abs/1705.08926)**: Foerster et al. introduce COMA, which uses a centralized critic and a counterfactual baseline for credit assignment among cooperative agents (2017 preprint; AAAI, 2018).
- **[Value-Decomposition Networks For Cooperative Multi-Agent Learning Based On Team Reward](https://www.ifaamas.org/Proceedings/aamas2018/pdfs/p2085.pdf)**: Sunehag et al. learn an additive decomposition of a shared team value function into agent-wise values for decentralized policies (AAMAS, 2018).

- **[The Contract Net Protocol: High-Level Communication and Control in a Distributed Problem Solver](https://reidgsmith.com/The_Contract_Net_Protocol_Dec-1980.pdf)**: Reid G. Smith describes task allocation through announcements, bids, and awards among distributed problem solvers (1980).
- **[The Hearsay-II Speech-Understanding System: Integrating Knowledge to Resolve Uncertainty](https://mas.cs.umass.edu/Documents/Erman_Hearsay80.pdf)**: Erman, Hayes-Roth, Lesser, and Reddy describe a blackboard architecture for coordinating independent knowledge sources through shared intermediate results (1980).
- **[BDI Agents: From Theory to Practice](https://cdn.aaai.org/ICMAS/1995/ICMAS95-042.pdf)**: Rao and Georgeff connect belief–desire–intention theory with practical agent implementations and an air-traffic-management application (ICMAS, 1995).
- **[Cut the Crap: An Economical Communication Pipeline for LLM-based Multi-Agent Systems](https://arxiv.org/abs/2410.02506)**: Zhang et al. introduce AgentPrune, which prunes message-passing graphs to reduce communication overhead in multi-agent systems (2024 preprint; ICLR, 2025).

- **[AgentWorld: Benchmarking Long-Horizon Collaboration of Multi-agent LLMs](https://arxiv.org/abs/2609.31590)**: Shu et al. evaluate long-horizon collaboration among agents with asymmetric roles and abilities (2026).
- **[Architectural Design, Not Only Model Intelligence, Governs Multi-Agent LLM Performance](https://arxiv.org/abs/2602.03128)**: Orogat, Rostam, and Mansour introduce MAFBench and compare multi-agent frameworks with the underlying language model held fixed (2026).
- **[Multi-Agent Actor-Critic for Mixed Cooperative-Competitive Environments](https://arxiv.org/abs/1706.02275)**: Lowe et al. introduce MADDPG, an actor-critic approach to centralized training and decentralized execution in cooperative and competitive environments (NeurIPS, 2017).
- **[The Surprising Effectiveness of PPO in Cooperative, Multi-Agent Games](https://arxiv.org/abs/2103.01955)**: Yu et al. evaluate PPO-based methods as baselines for cooperative multi-agent reinforcement learning (2021 preprint; NeurIPS, 2022).

- **[Learning to Communicate with Deep Multi-Agent Reinforcement Learning](https://arxiv.org/abs/1605.06676)**: Foerster et al. introduce two methods for learning communication protocols among agents (2016).
- **[QMIX: Monotonic Value Function Factorisation for Deep Multi-Agent Reinforcement Learning](https://arxiv.org/abs/1803.11485)**: Rashid et al. train decentralized policies with a centralized value function (2018).
- **[Melting Pot](https://arxiv.org/abs/2107.06857)**: Leibo et al. introduce a multi-agent reinforcement learning evaluation suite of test scenarios measuring generalization to novel social situations (2021).
- **[CICERO: Human-level play in the game of Diplomacy](https://www.science.org/doi/10.1126/science.ade9097)**: Meta's FAIR team report an agent combining a language model with planning and reasoning that reached human-level play in Diplomacy (Science, 2022).
- **[Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/abs/2304.03442)**: Park et al. populate a sandbox town with LLM agents that remember, reflect, and plan to produce believable individual and emergent social behavior (2023).
- **[SOTOPIA: Interactive Evaluation for Social Intelligence in Language Agents](https://arxiv.org/abs/2310.11667)**: Zhou et al. introduce an environment for evaluating social interactions among language agents (2023).
- **[CAMEL: Communicative Agents for "Mind" Exploration of Large Language Model Society](https://arxiv.org/abs/2303.17760)**: Li et al. propose a role-playing framework using inception prompting to drive autonomous cooperation between two LLM agents (2023).
- **[Improving Factuality and Reasoning in Language Models through Multiagent Debate](https://proceedings.mlr.press/v235/du24e.html)**: Du et al. evaluate multiple LLM instances debating over several rounds on factuality and reasoning tasks (ICML, 2024).
- **[Debating with More Persuasive LLMs Leads to More Truthful Answers](https://arxiv.org/abs/2402.06782)**: Khan et al. study multi-agent debate between LLMs as a method for scalable oversight and for eliciting more truthful answers from non-expert judges (ICML 2024).
- **[ChatDev: Communicative Agents for Software Development](https://arxiv.org/abs/2307.07924)**: Qian et al. organize LLM agents into a virtual software company with chat-driven design, coding, testing, and documentation stages (2023).
- **[MetaGPT: Meta Programming for a Multi-Agent Collaborative Framework](https://arxiv.org/abs/2308.00352)**: Hong et al. encode standardized operating procedures into an assembly-line multi-agent framework for software tasks (2023).
- **[AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation](https://arxiv.org/abs/2308.08155)**: Wu et al. present an open-source framework for building applications from customizable, conversable LLM agents (2023).
- **[AgentVerse: Facilitating Multi-Agent Collaboration and Exploring Emergent Behaviors](https://arxiv.org/abs/2308.10848)**: Chen et al. propose a framework that dynamically adjusts agent group composition and studies emergent social behaviors during collaboration (2023).
- **[Concordia: Generative Agent-Based Modeling](https://arxiv.org/abs/2312.03664)**: Vezhnevets et al. release a library using a Game Master pattern to simulate generative agents grounded in physical, social, or digital space (2023).
- **[Agent-as-a-Judge: Evaluate Agents with Agents](https://arxiv.org/abs/2410.10934)**: Zhao et al. extend LLM-as-a-judge to agentic evaluators that give intermediate feedback across a task, with a code-generation benchmark (2024).
- **[Magentic-One: A Generalist Multi-Agent System for Solving Complex Tasks](https://arxiv.org/abs/2411.04468)**: Fourney et al. present a modular orchestrator-led multi-agent system for open-ended web and file-based tasks (2024).
- **[Generative Agent Simulations of 1,000 People](https://arxiv.org/abs/2411.10109)**: Park et al. build agents from qualitative interviews with 1,052 real individuals and measure how accurately they reproduce survey responses and behaviors (2024).
- **[MultiAgentBench: Evaluating the Collaboration and Competition of LLM Agents](https://arxiv.org/abs/2503.01935)**: Zhu et al. introduce a benchmark with milestone-based metrics across collaborative and competitive scenarios and coordination topologies (2025).
- **[Evaluating Generalization Capabilities of LLM-Based Agents in Mixed-Motive Scenarios Using Concordia](https://arxiv.org/abs/2512.03318)**: Smith et al. evaluate cooperation across unfamiliar partners and scenarios in the Concordia Contest (2025).
- **[Which Agent Causes Task Failures and When? On Automated Failure Attribution of LLM Multi-Agent Systems](https://arxiv.org/abs/2505.00212)**: Zhang et al. introduce the Who&When dataset and evaluate methods for identifying the agents and steps responsible for failures (2025).
- **[Capable language models can outgrow the benefits of collaboration](https://doi.org/10.1038/s42256-026-01268-y)**: Kim et al. compare single-agent and multi-agent architectures under controlled prompts, tools, and compute budgets across six benchmarks. They examine when coordination improves performance or adds overhead (Nature Machine Intelligence, 2026; [preprint](https://arxiv.org/abs/2512.08296)).
- **[How we built our multi-agent research system](https://www.anthropic.com/engineering/multi-agent-research-system)**: Anthropic's engineering write-up describes an orchestrator-worker architecture in which a lead agent spawns subagents for parallel research (2025).

## Researchers & labs

*Generative social simulation & cooperative AI*
- **[Joel Z. Leibo](https://www.jzleibo.com/)**: Google DeepMind; creator of Melting Pot and Concordia, and a cultural-evolution framing of multi-agent cooperation.
- **[Alexander Vezhnevets](https://www.vezhnick.com/)**: Google DeepMind; lead of Concordia and generative agent-based modeling.
- **[Allan Dafoe](https://www.allandafoe.com/)**: Google DeepMind; founder of the Centre for the Governance of AI and the Cooperative AI Foundation.
- **[Edgar A. Duéñez-Guzmán](https://scholar.google.com/citations?user=Hl5wdRMAAAAJ&hl=en)**: Game theory and multi-agent reinforcement learning; contributor to Melting Pot and Concordia.

*Cooperative AI & game theory*
- **[Lewis Hammond](https://lewishammond.com/)**: Cooperative AI Foundation; multi-agent risk and safety.
- **[Jesse Clifton](https://longtermrisk.org/author/jesse-clifton/)**: Cooperative AI Foundation / Center on Long-Term Risk; bargaining and conflict.
- **[Vincent Conitzer](https://www.cs.cmu.edu/~conitzer/)**: Carnegie Mellon University; directs FOCAL, on game-theoretic foundations of cooperative AI.
- **[Michael P. Wellman](https://strategicreasoning.org/michael-p-wellman/)**: University of Michigan; empirical game-theoretic analysis and market games.
- **[David C. Parkes](https://parkes.seas.harvard.edu/)**: Harvard University; mechanism design and economics-and-computation.

*Multi-agent reinforcement learning*
- **[Jakob Foerster](https://www.jakobfoerster.com/)**: University of Oxford (FLAIR) and Meta FAIR; deep multi-agent reinforcement learning.
- **[Christian Schroeder de Witt](https://wittlab.ai/)**: University of Oxford; multi-agent security and covert communication.
- **[Natasha Jaques](https://natashajaques.ai/)**: University of Washington / Google DeepMind; social reinforcement learning.
- **[Max Kleiman-Weiner](http://faculty.washington.edu/maxkw/)**: University of Washington; computational models of cooperation and social learning.
- **[Eugene Vinitsky](https://www.eugenevinitsky.com/)**: New York University; multi-agent reinforcement learning at scale.
- **[Dylan Hadfield-Menell](https://people.csail.mit.edu/dhm/)**: MIT CSAIL; cooperative inverse reinforcement learning and alignment.
- **[Stuart Russell](https://people.eecs.berkeley.edu/~russell/)**: UC Berkeley; directs CHAI, on assistance games and provably beneficial AI.

*Self-play & negotiation*
- **[Noam Brown](https://noambrown.com/)**: OpenAI; self-play, search, and strategic reasoning (CICERO).
- **[Tim Baarslag](https://homepages.cwi.nl/~baarslag/)**: CWI and Utrecht University; automated negotiation and the ANAC competition.

*Failure modes, collusion & social intelligence*
- **[Mert Cemri](https://people.eecs.berkeley.edu/~mert_cemri/)**: UC Berkeley; multi-agent failure taxonomy (MAST).
- **[Maarten Sap](https://maartensap.com/)**: Carnegie Mellon University / Allen Institute for AI; social intelligence in language agents (SOTOPIA).
- **[Sara Fish](https://sara-fish.github.io/)**: Harvard University; algorithmic collusion among LLM agents.
- **[Emilio Calvano](https://emiliocalvano.wixsite.com/emiliocalvano)**: LUISS / Toulouse School of Economics; algorithmic pricing and collusion.

*Computational social science of agents*
- **[Iyad Rahwan](https://www.rahwan.me/)**: Max Planck Institute for Human Development; machine behavior and cooperative AI.
- **[Andrea Baronchelli](https://www.andreabaronchelli.com/)**: City St George's, University of London; emergence of social conventions in human and LLM populations.

*Cooperative agents & robustness (adjacent)*
- **[Sheila McIlraith](https://www.cs.toronto.edu/~sheila/)**: University of Toronto; theory of mind for cooperative agents.
- **[Adam Gleave](https://www.gleave.me/)**: FAR AI; multi-agent robustness and adversarial policies.
- **[Susmit Jha](https://susmitjha.github.io/)**: SRI International; assured autonomy and trustworthy AI.

## Funders, programs & RFPs

- **[Cooperative AI Foundation](https://www.cooperativeai.com/foundation)**: A charitable foundation, backed by a philanthropic commitment from Macroscopic Ventures, that funds research aimed at improving the cooperative intelligence of advanced AI systems.
- **[Cooperative AI Foundation: Research Grants 2025](https://www.cooperativeai.com/grants/2025)**: A closed call for research proposals on cooperation-relevant capabilities and propensities in AI systems.
- **[Schmidt Sciences: Science of Trustworthy AI](https://www.schmidtsciences.org/trustworthy-ai/)**: A Schmidt Sciences program funding technical research to understand, predict, and control risks from frontier AI systems, including a research aim on multi-agent risks.
- **[Schmidt Sciences: AI Agents](https://www.schmidtsciences.org/ai-agents/)**: A pilot program supporting academic and nonprofit researchers studying how multiple AI agents communicate and coordinate with one another.
- **[Macroscopic Ventures](https://macroscopic.org/grants)**: A nonprofit grantmaker whose focus areas include cooperative AI and reducing risks from advanced AI, and which funds the Cooperative AI Foundation.
- **[Coefficient Giving: Navigating Transformative AI](https://coefficientgiving.org/funds/navigating-transformative-ai/)**: The fund (from the grantmaker formerly named Open Philanthropy) supporting technical safety, governance, and field-building work on risks from transformative AI.
- **[ARIA: Safeguarded AI](https://aria.org.uk/opportunity-spaces/mathematics-for-safe-ai/safeguarded-ai/)**: A UK Advanced Research and Invention Agency programme developing methods for fleets of AI agents to produce formally verified, quantitatively safe artefacts.
- **[Foresight Institute: AI for Science & Safety Nodes](https://foresight.org/grants/ai-science-safety-nodes-rfp/)**: A request for proposals on local compute, coordination and accountability, and AI-driven science. The deadline was October 31, 2026.
- **[NSF: Safe Learning-Enabled Systems](https://www.nsf.gov/funding/opportunities/safe-learning-enabled-systems)**: An archived US National Science Foundation funding opportunity for research on the safety of learning-enabled systems, run in partnership with Open Philanthropy and Good Ventures.
- **[DICE: Decentralized Artificial Intelligence through Controlled Emergence (DARPA)](https://www.darpa.mil/research/programs/decentralized-artificial-intelligence-through-controlled-emergence)**: A DARPA program developing theory and algorithms for decentralized coordination and local inference control among collectives of heterogeneous AI agents.
- **[MATHBAC: Mathematics of Boosting Agentic Communication (DARPA)](https://www.darpa.mil/research/programs/mathbac)**: A 2026 DARPA program developing mathematical frameworks to design and provide guarantees for communication protocols among collectives of AI agents.

## Workshops, venues & communities

- **[AAMAS (via IFAAMAS)](https://www.ifaamas.org/)**: The International Foundation for Autonomous Agents and Multiagent Systems, which sponsors the annual AAMAS conference for agents and multi-agent systems research.
- **[AAMAS 2026](https://cyprusconferences.org/aamas2026/)**: The 25th International Conference on Autonomous Agents and Multiagent Systems, held in Paphos, Cyprus, in May 2026.
- **[Cooperative AI Workshop (NeurIPS)](https://www.cooperativeai.com/events)**: The Cooperative AI Foundation's recurring workshops at NeurIPS and other machine learning conferences.
- **[Concordia Contest](https://www.cooperativeai.com/contests/concordia-2024)**: A NeurIPS competition challenging participants to build language-model agents that exhibit cooperative intelligence in text-based mixed-motive scenarios.
- **[Melting Pot Contest](https://www.cooperativeai.com/contests/melting-pot-2023)**: A NeurIPS competition, run with Google DeepMind and MIT, evaluating multi-agent reinforcement learning agents on mixed-motive cooperation problems.
- **[ANAC (Automated Negotiating Agents Competition)](https://ii.tudelft.nl/nego/node/7)**: An annual international competition, held in conjunction with AAMAS or IJCAI since 2010, in which researchers develop and benchmark automated negotiation agents.
- **[Cooperative AI Summer School](https://www.cooperativeai.com/summer-school/summer-school-2025)**: An annual residential program run by the Cooperative AI Foundation for students and early-career researchers entering the field.

## Contributing

Contributions are welcome. Please open a pull request that:

- adds entries in the existing `**[Name](URL)**: one neutral sentence.` format,
- places each entry in the most fitting section, ordered by prominence,
- links the official repo, homepage, or paper (arXiv/DOI), and
- keeps descriptions factual and free of marketing language.

Suggestions, corrections, and dead-link reports via issues are equally valued.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, contributors have waived all copyright and related or neighboring rights to this work.
