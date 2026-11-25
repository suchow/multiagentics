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

- **[An Introduction to MultiAgent Systems (2nd ed.)](https://www.wiley.com/en-us/An+Introduction+to+MultiAgent+Systems,+2nd+Edition-p-9780470519462)**: Michael Wooldridge's standard textbook on classical multi-agent systems, covering agent architectures, interaction, and game-theoretic foundations (Wiley, 2009).
- **[Multiagent Systems: Algorithmic, Game-Theoretic, and Logical Foundations](https://www.masfoundations.org/)**: Shoham and Leyton-Brown's graduate textbook on the formal foundations of multi-agent systems, available as a free PDF (Cambridge University Press, 2009).
- **[Open Problems in Cooperative AI](https://arxiv.org/abs/2012.08630)**: Dafoe et al. set out a research agenda for building AI that can cooperate with humans and other agents (2020).
- **[Large Language Model based Multi-Agents: A Survey of Progress and Challenges](https://arxiv.org/abs/2402.01680)**: Guo et al. survey LLM-based multi-agent systems across agent profiling, communication, and capability growth (2024).
- **[LLM Multi-Agent Systems: Challenges and Open Problems](https://arxiv.org/abs/2402.03578)**: Han et al. catalog open problems in LLM multi-agent systems, including task allocation, reasoning, context, and memory (2024).
- **[Multi-Agent Collaboration Mechanisms: A Survey of LLMs](https://arxiv.org/abs/2501.06322)**: Tran et al. propose a framework characterizing LLM multi-agent collaboration by actors, types, structures, strategies, and coordination protocols (2025).

## Orchestration frameworks

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

- **[Model Context Protocol (MCP)](https://modelcontextprotocol.io/)**: An open standard, originally from Anthropic and now contributed to the Linux Foundation's Agentic AI Foundation, that connects AI applications to external data sources, tools, and prompts.
- **[Agent2Agent (A2A)](https://a2a-protocol.org/)**: An open protocol, originally developed by Google and now hosted by the Linux Foundation, that lets independent AI agents discover one another and exchange tasks and messages across vendors and frameworks.
- **[AGNTCY / Internet of Agents](https://docs.agntcy.org/)**: A Linux Foundation project, initially open-sourced by Cisco, providing infrastructure for agent discovery, identity, messaging, and observability across multi-agent systems.
- **[Agent Communication Protocol (ACP)](https://agentcommunicationprotocol.dev/)**: An open, REST-based protocol introduced by IBM's BeeAI for agent interoperability, now developed as part of A2A under the Linux Foundation.
- **[Agent Network Protocol (ANP)](https://github.com/agent-network-protocol/AgentNetworkProtocol)**: An open-source protocol using W3C Decentralized Identifiers to provide identity, encrypted communication, and capability discovery for agent-to-agent collaboration.
- **[FIPA ACL Message Structure Specification](http://www.fipa.org/specs/fipa00061/SC00061G.html)**: The 2002 FIPA standard defining the message structure of the Agent Communication Language, a historical reference for interoperable multi-agent communication.
- **[KQML](https://research.cs.umbc.edu/kqml/)**: The UMBC resource hub for the Knowledge Query and Manipulation Language, an early-1990s DARPA-sponsored language and protocol for knowledge exchange among software agents.

## Environments & simulation

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
- **[Improving Factuality and Reasoning via Multiagent Debate](https://arxiv.org/abs/2305.14325)**: Du et al. show that having multiple LLM instances debate over several rounds improves factuality and reasoning (2023).
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
- **[Towards a Science of Scaling Agent Systems](https://arxiv.org/abs/2512.08296)**: Kim et al. compare single-agent and multi-agent architectures across tasks. They find that coordination can improve or degrade performance depending on task structure (2025).
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
