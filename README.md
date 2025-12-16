📱 TrialForge - Mobile Command Center

TrialForge Mobile is a responsive executive dashboard designed for Clinical Operations leaders on the move. It consolidates three critical pillars of trial management—Patient Retention, Recruitment Velocity, and Staff Stability—into a single, touch-optimized interface.

Shutterstock

It demonstrates how "Forge Theory" (Signal Decay Modeling) can be operationalized into a real-time monitoring tool, predicting risks like patient dropout or staff burnout before they become critical failures.
✨ Key Features

    Multi-Modal Context: Instantly switch between three operational views:

        Retention: Monitor active patient engagement and dropout risks.

        Recruitment: Track lead conversion velocity and "ghosting" risks.

        Staff: Analyze site workload and predict CRA burnout.

    Mobile-First UX: Features a responsive layout that adapts from a desktop sidebar to a touch-friendly mobile navigation bar.

    Dynamic Theming: The interface color psychology shifts with the context (Clinical Blue, Recruitment Purple, Alert Orange) to reduce cognitive load.

    Decay Forecasting: Visualizes the "Natural Decay" of metrics (interest, motivation, energy) against the "Stabilized Path" created by interventions.

🚀 Quick Start

    Run: Open index.html in any browser.

    Mobile View: For the best experience, open Developer Tools (F12) and toggle "Device Toolbar" (Ctrl+Shift+M) to simulate a mobile phone or tablet.

    Navigate: Tap the icons in the sidebar/top-nav to switch contexts.

    Simulate: Notice how the KPIs, Risk Lists, and Charts update instantly to reflect the selected operational domain.

🧮 The Logic: Signal Decay

This dashboard visualizes Behavioral Decay over time using pre-computed trend lines.
The Concept
Signalt​=Signalinitial​×e−k⋅t

    Patient Mode: k represents the loss of motivation to adhere to protocol.

    Recruitment Mode: k represents the rapid loss of lead interest (Lead Cooling).

    Staff Mode: k represents the depletion of resilience (Burnout Curve).

⚙️ Configuration

The dashboard content is driven by the CONFIG object. You can easily "White Label" this tool for different industries (e.g., changing "Patients" to "Customers") by editing the data structure:
JavaScript

const CONFIG = {
    patient: {
        title: 'Customer Retention', // Changed from Patient
        theme: '#2980b9',
        kpis: [ ... ],
        items: [
            { name: 'Client A (At Risk)', risk: 'High' }
        ]
    },
    // ... other modes
};

🛠️ Tech Stack

    Core: HTML5, CSS3 (Mobile-First Media Queries).

    Logic: Vanilla JavaScript (ES6+).

    Charting: Plotly.js.

    Icons: FontAwesome.

⚠️ Concept Note

Frontend Demonstration. This is a UI/UX concept for a Clinical Trial Management System (CTMS) mobile companion. It does not connect to a live backend database. The metrics shown are static examples designed to illustrate the "Command Center" workflow.
📄 License

Open Source. Ideal for prototyping operational dashboards and mobile web apps.
