<div align="center">

# 🛡️ SecOpsOps

### Teaching Ai To Think Like A Security Analyst

![Ai](https://img.shields.io/badge/Ai-Reinforcement_Learning-purple?style=flat-square)
![Security](https://img.shields.io/badge/Domain-Cybersecurity-blue?style=flat-square)
![Status](https://img.shields.io/badge/Status-Live-success?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-HuggingFace-orange?style=flat-square)

---

### ⚡ Train Ai Agents To Detect, Investigate, And Respond To Real Security Threats

</div>

---

## 🔗 Links

- 🧠 **HuggingFace Space** → https://huggingface.co/spaces/itzrealmee/secopsops  
- 🎮 **Live Demo** → https://itzrealmee-secopsops.hf.space/play  
- 💻 **GitHub** → https://github.com/gggsiw/secopsops  
- 📓 **Colab Notebook** → https://colab.research.google.com/github/gggsiw/secopsops/blob/main/secopsops_training.ipynb  
- 📖 **Blog** → https://huggingface.co/spaces/itzrealmee/secopsops/blob/main/Blog.MD  

---

## 🧠 The Problem

Every 39 Seconds, A Company Gets Attacked.

SOC Analysts Face Thousands Of Alerts Daily — Most Are Noise.  
But Hidden Inside That Noise Is The One Attack That Matters.

- Ransomware  
- Data Exfiltration  
- Active Intrusions  

The Challenge Isn’t Detection — It’s **Decision Making Under Noise**.

---

## 🚀 What Is SecOpsOps?

**SecOpsOps** Is A Reinforcement Learning Environment Where Ai Learns To Act Like A SOC Analyst.

It:
- Reads Security Alerts  
- Uses Enterprise Tools  
- Takes Actions  
- Learns From Rewards & Mistakes  

Not A Toy. Not A Simulation.  
👉 A **Realistic Multi-App Security Workflow Environment**

---

## ⚡ Agent Action Space

| Action | Description |
|--------|------------|
| `investigate` | Analyze Suspicious Alerts |
| `query_logs` | Pull Supporting Log Data |
| `query_siem` | Correlate Events Across Systems |
| `block_ip` | Stop Malicious Actors Instantly |
| `escalate` | Hand Off To Incident Response |
| `close` | Mark False Positives |
| `report` | Generate Incident Reports |
| `create_ticket` | Track Issues In Ticketing System |

---

## 🎯 Scenarios

### 🟢 Easy — Malware Triage
- Identify Real Threats  
- Ignore False Positives  
- Establish Baseline Intelligence  

---

### 🟡 Medium — Brute Force Attack
- Requires Log Investigation  
- Punishes Blind Actions  
- Tests Decision Order  

---

### 🔴 Hard — APT Kill Chain
- Multi-Step Attack Simulation  
- Phishing → Lateral Movement → Exfiltration  
- Includes False Positives  
- Requires Context Awareness  

---

## 🧮 Reward System

```text
final_score = base_score + speed_bonus + chain_bonus + fp_penalty
```

- **Base Score** → Correctness Of Action  
- **Speed Bonus** → Faster Response To Critical Threats  
- **Chain Bonus** → Reward Correct Action Sequences  
- **FP Penalty** → Heavy Punishment For False Positives  

> ⚡ Teaches The Agent *How To Think*, Not Just *What To Do*

---

## 📊 Results

| Task | Score | Insight |
|------|------|--------|
| Easy | 0.82 | Strong On Obvious Threats |
| Medium | 0.67 | Weak Without Investigation |
| Hard | 0.72 | Misses Context Chains |
| **Overall** | **0.74** | Strong Baseline |

---

## 🎮 Try It Live

👉 https://itzrealmee-secopsops.hf.space/play

---

## ⚙️ API Usage

```bash
# Start Episode
curl -X POST https://itzrealmee-secopsops.hf.space/reset \
  -H "Content-Type: application/json" \
  -d '{"task_name": "hard"}'

# Query SIEM
curl -X POST https://itzrealmee-secopsops.hf.space/siem/query \
  -H "Content-Type: application/json" \
  -d '{"task_name": "hard", "query": "203.0.113.5"}'

# Take Action
curl -X POST https://itzrealmee-secopsops.hf.space/step \
  -H "Content-Type: application/json" \
  -d '{"task_name": "hard", "action": {"action_type": "block_ip", "query": "198.51.100.7"}}'
```

📄 Docs → https://itzrealmee-secopsops.hf.space/docs

---

## 🧠 Training Pipeline

1. Generate Optimal Action Chains  
2. Fine-Tune Qwen2.5 Model (SFT)  
3. Evaluate Across Scenarios  
4. Track Reward Improvements  

---

## 🛠 Run Locally

```bash
git clone https://github.com/gggsiw/secopsops.git
cd secopsops
pip install -r requirements.txt
python app.py
```

Open → `http://localhost:7860/play`

---

## 📈 Training Visuals

### Loss Curve
<img src="https://github.com/user-attachments/assets/747e2013-9a3a-478d-bcc0-19cbc8938cde" />

### Reward Curve
<img src="https://github.com/user-attachments/assets/7c7a61eb-1cc1-40f5-8bbd-e68bbee92b1a" />

### Before vs After
<img src="https://github.com/user-attachments/assets/855c3b02-2416-4633-ae74-2411ec1de669" />

---

<div align="center">

## 🧑‍💻 Team

**Krishna Sharma**  
**Arjun Bohara**

---

## ⭐ Support

Star ⭐ • Fork 🍴 • Contribute 🧠

---

### 🛡️ SecOpsOps — Train Ai. Defend Reality.

</div>
