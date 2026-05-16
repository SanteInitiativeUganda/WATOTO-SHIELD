# Watoto Shield

**Climate-Health Early Action for Children**

Watoto Shield is an open-source AI/data science platform that helps communities predict climate-sensitive child health risks and trigger early action through SMS/USSD alerts for caregivers, Village Health Teams (VHTs), schools, clinics, and local councils.

> **Tagline:** Turning climate, waste, and health data into timely action before children get sick.

---

## Overview

Children in climate-vulnerable communities are increasingly exposed to health risks linked to extreme heat, flooding, air pollution, poor drainage, unsafe waste disposal, malaria, diarrhoeal disease, asthma attacks, respiratory illness, and other climate-sensitive conditions.

In many communities, early warning signs are visible before illness escalates. Heavy rain may be forecast. Drains may already be blocked. Waste may be accumulating near homes or schools. Clinics may begin seeing more cases. Schools may report absenteeism. However, these signals often sit in separate systems and do not reach the people who can act early.

**Watoto Shield** connects climate, environmental, health, and community-reported data into one early action system. It identifies high-risk areas and sends simple, localized alerts to help communities prevent child illness before it becomes a crisis.

---

## Problem

Climate change is increasing children’s exposure to:

- Extreme heat
- Flooding
- Air pollution
- Unsafe water
- Poor drainage
- Open dumping and waste accumulation
- Vector-borne diseases such as malaria
- Diarrhoeal diseases
- Respiratory illness and asthma attacks
- Health facility service disruptions

Many current response systems are reactive. Caregivers, VHTs, schools, clinics, and local leaders often respond after children are already sick.

Watoto Shield addresses this gap by turning fragmented climate, waste, and health data into practical early action.

---

## Solution

Watoto Shield uses a simple early action loop:

**Sense → Predict → Alert → Act → Verify**

### 1. Sense

Collect data from multiple sources, including:

- Weather and rainfall forecasts
- Heat and air quality indicators
- Waste and blocked drainage reports
- Clinic and public health surveillance data
- VHT and caregiver SMS/USSD reports
- School absenteeism signals
- Community observations from local leaders

### 2. Predict

Use lightweight AI/data science and rules-based risk scoring to identify communities where children may be at increased risk of climate-sensitive illness in the coming days.

### 3. Alert

Send simple SMS/USSD alerts to the right actors:

- Caregivers
- VHTs and community health workers
- Schools
- Clinics and health facilities
- Local councils
- Youth cleanup groups
- District health teams

### 4. Act

Trigger practical prevention and preparedness actions, such as:

- VHT household visits
- Safe water and hygiene messaging
- ORS readiness at clinics
- Asthma medication checks
- Drainage clearing
- Waste hotspot cleanup
- School-level monitoring
- Referral support

### 5. Verify

Track whether action happened and whether risk reduced through:

- VHT response reports
- Resolved waste hotspot reports
- Clinic attendance trends
- School absenteeism trends
- Community feedback
- Repeat hotspot tracking

---

## Example Use Case

A parish is expecting heavy rainfall in three days. VHTs and caregivers have reported blocked drains and open waste dumping near a school. A nearby clinic is also seeing an increase in diarrhoeal disease cases.

Watoto Shield identifies the area as high risk and sends:

- **Caregiver alerts:** Treat drinking water, watch for diarrhoea signs, and contact the VHT early.
- **VHT alerts:** Follow up households with young children and advise on safe water practices.
- **Clinic alerts:** Prepare ORS, zinc, and referral support.
- **School alerts:** Monitor absenteeism and reinforce hygiene messages.
- **Local council alerts:** Prioritize drainage clearing and waste removal before rainfall.

---

## Current Prototype Status

Watoto Shield is at **early prototype stage**.

The initial system architecture, user journey, risk-scoring logic, sample data structure, SMS/USSD alert flow, and open-source documentation have been developed. The prototype package demonstrates how climate, waste, drainage, and child health risk indicators can be combined to generate location-based early warning alerts and action prompts for caregivers, VHTs, clinics, schools, and local councils.

Current prototype components include:

- Problem definition
- System architecture
- User journey
- Early action loop
- Initial risk-scoring logic
- Priority use cases
- Sample alert messages
- Synthetic data structure
- Pilot design
- Open-source repository documentation

Next development steps include:

- Building the minimum viable product
- Setting up SMS/USSD flows
- Developing and testing the risk scoring engine
- Creating dashboard mockups
- Testing alerts with frontline users
- Piloting in a selected Ugandan community

---

## Key Features

Planned core features include:

- SMS/USSD-based reporting and alerts
- Climate-health risk scoring
- Waste and drainage hotspot reporting
- Geospatial hotspot mapping
- Child-focused vulnerability indicators
- Clinic and DHIS2-compatible data integration, where approved
- Localized alerts in relevant languages
- District dashboard for planning and accountability
- Action verification and feedback loop
- Open-source documentation and reusable tools

---

## Technology Stack

The proposed low-cost technology stack includes:

| Layer | Proposed Tools |
|---|---|
| Data collection | SMS/USSD, mobile forms, clinic data, community reports |
| Climate data | Weather forecasts, rainfall data, heat indicators, air quality sources |
| Health data | Clinic records, disease surveillance, DHIS2-compatible data where approved |
| Processing | Python, lightweight machine learning, rules-based risk scoring |
| Mapping | QGIS, open geospatial data, free satellite imagery where feasible |
| Alerts | SMS/USSD through providers such as Africa’s Talking |
| Dashboard | Open-source web dashboard for district and implementation teams |
| Documentation | GitHub, Markdown, open-source technical guides |

---

## Target Users

Watoto Shield is designed for frontline and local decision-making actors, including:

- Caregivers of children
- Village Health Teams and community health workers
- Schools and teachers
- Health facilities and clinics
- Local councils and municipal leaders
- District health teams
- Youth groups and community cleanup teams
- NGOs and public health partners

---

## Pilot Plan

The initial pilot will focus on a small, practical deployment in Uganda.

### Proposed Pilot Scope

- **Location:** One high-risk urban or peri-urban parish
- **Users:** 20 VHTs, one health facility, selected schools, caregivers, and local council actors
- **Health risks:** Childhood respiratory risk and diarrhoeal disease
- **Climate/environmental risks:** Heat, air pollution, rainfall, flooding, blocked drainage, and waste hotspots

### Pilot Indicators

- Number of alerts sent
- Alert delivery rate
- VHT response rate
- Caregiver actions taken
- Waste hotspots reported
- Waste hotspots resolved
- Clinic visits for target conditions
- School absenteeism trends
- User feedback and usability
- Time from alert to action

---

## Data Privacy and Child Protection

Watoto Shield is designed with privacy, safeguarding, and child protection in mind.

This repository will not contain real personal health data, child names, patient records, or identifiable household information.

For demonstration purposes, the project will use:

- Synthetic data
- Dummy records
- Aggregated indicators
- Privacy-safe mock examples

Any future implementation involving health or child-related data will require appropriate consent, data protection protocols, ethical safeguards, child safeguarding procedures, and compliance with relevant national and institutional requirements.

---

## Open Source Commitment

Watoto Shield is intended to be open-source so that public health teams, local governments, NGOs, researchers, and innovators can adapt and improve the solution for different settings.

Planned open-source components include:

- System architecture
- Risk scoring logic
- SMS/USSD message templates
- Dashboard documentation
- Sample synthetic datasets
- Implementation guides
- Pilot learning tools

---

## Suggested Repository Structure

```text
watoto-shield/
│
├── README.md
├── LICENSE
├── docs/
│   ├── system-architecture.md
│   ├── data-flow.md
│   ├── user-journeys.md
│   ├── sms-alerts.md
│   ├── risk-scoring-logic.md
│   └── pilot-plan.md
│
├── src/
│   └── risk_score.py
│
├── data/
│   ├── sample_inputs.csv
│   └── sample_outputs.csv
│
├── dashboard/
│   └── dashboard-mockup.md
│
└── screenshots/
    └── placeholder.md
```

---

## Roadmap

### Months 1–2

- Finalize repository structure
- Prepare open-source documentation
- Develop SMS/USSD reporting flow
- Prepare data protection and child safeguarding protocols
- Validate pilot indicators with frontline users

### Months 3–4

- Build minimum viable product
- Develop the first risk scoring engine
- Configure dashboard prototype
- Prepare localized alert templates
- Test the alert logic using synthetic and historical sample data

### Months 5–7

- Conduct parish-level pilot
- Train VHTs and local actors
- Test SMS/USSD alerts
- Track early action responses
- Collect user feedback from caregivers, VHTs, schools, clinics, and local councils

### Months 8–9

- Analyze pilot results
- Refine risk model
- Improve user experience
- Document lessons learned

### Months 10–12

- Publish open-source implementation package
- Strengthen dashboard and reporting
- Prepare scale-readiness plan
- Engage district and national stakeholders

---

## Contributing

Contributions are welcome from developers, public health practitioners, climate-health researchers, designers, data scientists, community health experts, and local government innovators.

Possible contribution areas include:

- Risk scoring model development
- SMS/USSD workflow design
- Dashboard development
- Geospatial mapping
- Climate-health research
- Data privacy and protection
- Local language alert design
- Pilot evaluation tools

---

## License

This project is intended for open-source release.

Recommended license options under consideration:

- MIT License
- Apache License 2.0

A final license will be selected before full public release.

---

## Contact

For collaboration, partnership, or technical contribution, please contact:

**Project:** Watoto Shield  
**Focus:** Climate-health early action for children  
**Country:** Uganda  
**Email:** mirene@santeinitiative.org  
**Website:** https://santeinitiative.org/

---

## Final Note

Watoto Shield is being developed to help communities act before children get sick. The project aims to strengthen early warning, early action, healthcare readiness, and community-level climate resilience for children in Uganda.
