# 🏗️ AI Solution Architect - Intelligent Enterprise Architecture Recommendation System

An AI-powered Solution Architect platform designed to analyze software project requirements and recommend comprehensive, enterprise-grade software architectures, technology stacks, sprint plans, cloud cost estimates, and technical risk mitigations.

---

## 📌 Problem Statement & Background
When starting a software project, choosing the right technology stack, database, architecture pattern, authentication method, and deployment strategy is one of the biggest challenges developers and tech leaders face. Wrong technology choices lead to increased cost, development delays, technical debt, and scalability bottlenecks.

**ArchitectAI** solves this by leveraging Generative AI (Google Gemini API) paired with a deterministic expert system to synthesize tailored, production-ready solution architecture blueprints with deep technical justifications before writing a single line of code.

---

## ✨ Key Features

- **⚡ AI Requirement Analysis**: Evaluates project domain, expected DAU, concurrency requirements, budget tier, team size, launch deadlines, compliance constraints (GDPR, PCI-DSS, HIPAA, SOC2), and feature requirements.
- **🎨 Interactive Visual Topology Diagram**: Renders dynamic, animated SVG request flow diagrams across Presentation, Edge/WAF, Compute Services, and Data/Caching layers with clickable component inspection cards.
- **🛠️ Deep Technology Stack Justifications**: Detailed recommendations for Frontend, Backend, Database, Auth, Cloud, and Queue services detailing *"Why This Technology?"* and *"Why Not Alternative Technologies?"*.
- **📊 Multi-Option Architecture Comparison Matrix**: Side-by-side comparative scoring of Recommended Architecture vs Structural Alternatives across Complexity, Cost, Time-to-Market, Scalability, and Maintenance.
- **📅 Agile Sprint Plan & Roadmap**: 16-Week execution schedule broken down into bi-weekly sprints with task backlogs, story point allocations, team velocity metrics, and visual Gantt phase bars.
- **💰 Dynamic Cloud Cost Estimator**: Itemized monthly cloud hosting expenses with an interactive DAU scale slider (1,000 to 500,000 users) and cost optimization strategies.
- **🛡️ Technical Risk Analysis & Mitigation Matrix**: Severity-graded audit of Technical Debt, Security Risks, SPOF (Single Point of Failure), and Compliance Gaps with actionable mitigations.
- **📄 Executive PDF Report Export**: 1-click multi-page executive PDF report generation ready for client presentations and technical stakeholders.
- **🔐 JWT Authentication & User Session**: Simulated JWT authentication with role-based access (`Principal Architect`, `CTO`, `Senior Engineer`, `Student`).
- **📚 Blueprint History Workbench**: LocalStorage persistence to save, load, export raw JSON, or manage past architectural reports.

---

## 📐 Technology Stack

| Layer | Technology |
| :--- | :--- |
| **Frontend** | React.js 18, Vite, Tailwind CSS |
| **UI Components & Icons** | Lucide React, Custom Glassmorphism CSS |
| **AI Recommendation Model** | Google Gemini API (Gemini 1.5/2.0 Flash) + Expert Rule Engine |
| **PDF Generation** | jsPDF, html2canvas |
| **Authentication** | JWT (JSON Web Tokens) Simulation (RSA-256) |
| **State & Persistence** | React Hooks, LocalStorage Blueprint Workbench |

---

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (v18.0.0 or higher)
- [npm](https://www.npmjs.com/) (v9.0.0 or higher)

### Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/AI-Solution-Architect.git
   cd AI-Solution-Architect
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```

3. **Start the Development Server**
   ```bash
   npm run dev
   ```

4. **Access the Application**
   Open your browser and navigate to `http://localhost:5173/`.

---

## 🔑 Configuring Google Gemini API (Optional)

1. Get a free API Key from [Google AI Studio](https://aistudio.google.com/app/apikey).
2. Open the application, click **"Configure Gemini AI"** in the top navigation bar.
3. Paste your Gemini API Key and click **Save API Key**.
> *Note: If no API key is provided, the platform seamlessly uses its built-in enterprise expert reasoning engine to generate architectural blueprints.*

---

## 📁 Project Structure

```
Project_1/
├── src/
│   ├── components/
│   │   ├── Analysis/
│   │   │   ├── ArchitectureComparison.jsx   # Side-by-side trade-off matrix
│   │   │   └── TechStackView.jsx            # Deep tech stack justifications
│   │   ├── Cost/
│   │   │   └── CostEstimator.jsx            # Interactive DAU slider & cost breakdown
│   │   ├── Diagrams/
│   │   │   └── ArchitectureDiagram.jsx        # SVG visual request flow diagram
│   │   ├── History/
│   │   │   └── ProjectHistory.jsx           # Saved blueprints drawer
│   │   ├── ProjectForm/
│   │   │   └── ProjectWizard.jsx            # 4-step intake wizard & presets
│   │   ├── Report/
│   │   │   └── ExecutiveReport.jsx          # Executive report dashboard view
│   │   ├── Risks/
│   │   │   └── RiskAnalysis.jsx             # Technical risk & mitigation matrix
│   │   ├── Timeline/
│   │   │   └── SprintPlan.jsx               # Agile sprint roadmap & Gantt chart
│   │   ├── ApiKeyModal.jsx                  # Gemini API Key configuration
│   │   ├── AuthModal.jsx                    # JWT authentication & profile modal
│   │   └── Navbar.jsx                       # Sticky header navigation
│   ├── data/
│   │   └── knowledgeBase.js                 # Presets & architectural catalogs
│   ├── services/
│   │   ├── aiEngine.js                      # Gemini API integration & fallback engine
│   │   └── pdfGenerator.js                  # PDF exporter utility
│   ├── App.jsx                              # Main app state & routing
│   └── index.css                            # Modern glassmorphism design tokens
├── package.json
└── README.md
```

---

## 🎯 Use Cases

- **Software Developers & Tech Leads**: Make confident technical choices before starting greenfield development.
- **Enterprise Architects & Consultants**: Rapidly produce comprehensive architectural proposals and PDF reports for clients.
- **Students & Researchers**: Learn enterprise architecture patterns, trade-off analysis, and cloud cost estimation.

---

## 📜 License
Distributed under the MIT License. See `LICENSE` for more information.
