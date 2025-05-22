# 🛰️ AkashTeer AI Agent Simulation

**AkashTeer** is a cutting-edge multi-agent simulation inspired by India's indigenous autonomous defense system — a real-time, satellite-linked, AI-coordinated battle swarm framework. This project replicates core elements of AkashTeer’s intelligence infrastructure using modern Generative AI agent frameworks including **LangChain**, **LangGraph**, and **CrewAI**.

> ⚡️ Simulate a zero-latency combat cloud connecting real-time satellite intelligence, swarm coordination, and AI-powered mission execution.

---

## 🚀 Project Objectives

* Simulate a **multi-layered AI command system** coordinating satellite feeds, autonomous drones, and stealth protocols.
* Integrate **LangGraph** for agentic flow orchestration (e.g. ISR → Targeting → Decision → Deployment).
* Use **CrewAI** for human-in-the-loop role simulation (Tactical Officer, Satellite AI, Drone Commander).
* Prototype **NavIC-like GPS precision guidance**, weather-adaptive mission updates, and real-time anomaly response.
* Enable **plug-and-play agent orchestration** that can scale from battlefield simulation to disaster response or smart defense logistics.

---

## 🧠 Core Technologies

| Layer                 | Tools/Frameworks                                                                       |
| --------------------- | -------------------------------------------------------------------------------------- |
| Agent Orchestration   | [CrewAI](https://docs.crewai.com/), [LangGraph](https://docs.langchain.com/langgraph/) |
| Agent Memory & Chains | [LangChain](https://www.langchain.com/), VectorStore, ReAct                            |
| LLM Backend           | OpenAI GPT-4 / Claude / Ollama-compatible                                              |
| Utilities             | Python 3.11+, bash scripting, dotenv, JSON streaming                                   |
| Optional              | Streamlit / Gradio for visual dashboards                                               |

---

## 📦 Folder Structure

```bash
akashteer_ai_agents/
├── agents/
│   ├── satellite_intel_agent.py
│   ├── swarm_control_agent.py
│   ├── tactical_decision_agent.py
│   ├── drone_execution_agent.py
├── flows/
│   ├── langgraph_combat_loop.py
│   └── mission_reroute_flow.py
├── crews/
│   ├── command_center_crew.py
│   └── field_response_crew.py
├── utils/
│   ├── navic_simulator.py
│   └── satellite_feed_loader.py
├── data/
│   └── mock_satellite_imagery/
├── run_simulation.py
├── requirements.txt
└── README.md
```

---

## 🎯 Use Case Simulations

1. **Target Identification & Interception**

   * Agents analyze synthetic ISRO-style satellite data
   * Predict enemy movement
   * Assign drone payloads and stealth routes

2. **Anomaly Detection & Mission Rerouting**

   * Mid-mission weather disruptions or radar detection
   * Command AI recalculates path using Terrain + NAVIC simulator

3. **Tactical Officer Override**

   * Human agent (simulated) intervenes with alternate logic via CrewAI

---

## 🧪 How to Run

### 1. Clone the repo

```bash
git clone https://github.com/yourusername/akashteer_ai_agents.git
cd akashteer_ai_agents
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Set up `.env`

Create a `.env` file with your LLM API key:

```env
OPENAI_API_KEY=sk-xxxxxxxxxxxx
```

### 4. Run a sample simulation

```bash
python run_simulation.py
```

You can also trigger:

```bash
python flows/langgraph_combat_loop.py
```

---

## 🧬 Agent Roles

| Agent                       | Responsibility                                           |
| --------------------------- | -------------------------------------------------------- |
| 🛰️ `SatelliteIntelAgent`   | Analyzes satellite feeds (mock Cartosat/RISAT data)      |
| 🧠 `TacticalDecisionAgent`  | Chooses targets and assigns priority levels              |
| 🐝 `SwarmControlAgent`      | Coordinates up to 10 simulated drones with stealth logic |
| ⚔️ `DroneExecutionAgent`    | Executes payload delivery or strike missions             |
| 🧑‍✈️ `TacticalOfficerCrew` | Optional human-simulating agent via CrewAI               |

---

## 🔐 Ethical AI, Safety, and Governance

AkashTeer includes modules and stubs for:

* Bias monitoring in target identification
* Command override logs
* Geo-political boundary simulation (avoid civilian zones)
* Faith-based and UN-compatible AI guardrails (for future extensibility)

---

## 🏛️ Inspiration

Inspired by India’s **AkashTeer Defense Program** (DRDO + ISRO + BEL), this project is a tribute to indigenous defense innovation, translated into a multi-agent AI system capable of simulation, training, and research.

---

## 📈 Roadmap

* [ ] Streamlit-based mission control dashboard
* [ ] Add HuggingFace model compatibility
* [ ] Expand to SAR and thermal imaging ingestion
* [ ] Enable drone fleet visualization (via Cesium.js or Deck.gl)
* [ ] Plugin-based threat intelligence integration (cyber/ground)

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first.
Contact: **[sudarshan.shekar@datacaliper.com]
(mailto:omsaisudarshan108@gmail.com)**

---

## 📜 License

MIT License © 2025 AkashTeer AI Initiative
*For educational, research, and ethical simulation purposes only.*
