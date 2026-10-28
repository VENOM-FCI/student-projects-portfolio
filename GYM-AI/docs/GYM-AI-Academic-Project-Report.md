# GYM AI System — Academic Project Report

**Project type:** Systems Analysis and Project Management coursework  
**Team size:** 5 students  
**My reported role:** Team Leader and Final Document Designer  
**Public-copy privacy note:** Personal contact details and the named individual’s contact block in the source have been omitted.

## 1. System request

**Business need:** Increase customer satisfaction and retention in gyms through personalized fitness guidance supported by AI.

**Proposed functions**
- Generate personalized workout plans.
- Provide nutrition recommendations.
- Track user progress.
- Give real-time feedback during exercises.

**Expected value**
- Tangible: potential increase in gym membership revenue.
- Intangible: improved user satisfaction and fitness results.

**Constraints recorded in the source**
- Limited budget for AI development.
- User-data privacy must be protected.
- Short expected completion time.

## 2. Feasibility study

### 2.1 Technical feasibility

The report proposes:
- Central servers, user PCs/mobile phones, GPU servers, network devices, backup storage, and data-collection tools.
- Linux or Windows operating systems.
- MySQL or MongoDB for data storage.
- Python or JavaScript for development.
- TensorFlow or PyTorch for AI.
- Web/mobile application access, APIs, security software, HTTPS, stable connectivity, and remote access.
- Specialist roles such as AI engineers, data scientists, web developers, UI/UX designers, QA testers, and network engineers.

These are technologies and resources proposed by the report, not a claim that the student team built all of them.

### 2.2 Economic feasibility — figures as reported

| Item | Reported value |
|---|---:|
| System development | EGP 120,000 |
| AI infrastructure | EGP 80,000 |
| Software licenses | EGP 10,000 |
| Installation | EGP 10,000 |
| Training | EGP 10,000 |
| Annual maintenance | EGP 20,000 |
| Annual technical support | EGP 15,000 |
| Annual hosting and internet | EGP 20,000 |
| Annual electricity | EGP 8,000 |
| Annual software renewal | EGP 7,000 |
| Annual AI subscriptions (benefit) | EGP 100,000 |
| Annual business integrations (benefit) | EGP 60,000 |
| Reduced labour costs (benefit) | EGP 40,000 |
| Increased efficiency (benefit) | EGP 30,000 |

The source reports annual operating costs of EGP 70,000, annual benefits of EGP 230,000, net cash flow of EGP 160,000, payback of 1.47 years, ROI of 96%, and NPV of +EGP 165,000.

**Important source inconsistency:** the initial-cost table prints “2350,000 EGP”; the cash-flow calculation uses EGP 235,000; and the staffing-plan table states EGP 2,350,000. The cumulative cash-flow table also has missing entries. These figures have been preserved here as reported, not silently reconciled, and must be checked before use as validated analysis.

### 2.3 Organizational feasibility

The report expects user adoption to be supported by training and management support. It identifies basic system-use training and an introduction to AI tools as training needs. Expected positive effects include improved productivity, lower operating costs, and better service quality.

### 2.4 Operational feasibility

The report states that the proposed system should fit into daily gym activities, be easy to use, improve workflow efficiency, and reduce human errors. These are expected outcomes, not measured results.

## 3. Work plan

The report includes an example task titled “AI Model Feasibility Analysis”, with a planned period of October 10–25, 2025, a technical/economic feasibility report as the deliverable, high priority, an estimated 40 hours, and an actual 38.5 hours. A second version in the source gives October 10–24, 2025, so the date should be confirmed.

## 4. Work Breakdown Structure (WBS)

| ID | Task | Duration (days) | Dependency/status in source |
|---|---|---:|---|
| 1 | Design Phase | 25 | Open |
| 1.1 | Database Design (Members & Workouts) | 7 | Open |
| 1.1.1 | User Profile & Bio-data Schema | 3 | Open |
| 1.1.2 | AI Training Datasets Schema | 4 | Open |
| 1.2 | AI Model Architecture Design | 10 | Depends on 1.1.2; Open |
| 1.2.1 | Pose Estimation Model Architecture | 5 | Open |
| 1.3 | UI/UX Design (Mobile & Dashboard) | 8 | Open |
| 1.4 | System Integration Plan | 5 | Depends on 1.2 and 1.3; Open |
| 2 | Development Phase | 45 | Depends on 1; Open |
| 2.1 | Frontend Development (React Native) | 20 | Depends on 1.3; Open |
| 2.2 | Backend API Development (Node.js/Python in one version) | 15 | Depends on 1.1; Open |
| 2.3 | AI Integration (Computer Vision Module) | 20 | Depends on 1.2; Open |

These are planning tasks recorded in the assignment, not proof of completed software implementation.

## 5. Staffing plan

The source proposes roles and skills including:
- Feasibility analysis — AI Specialist; Python, TensorFlow, MediaPipe.
- Database design — Database Administrator; MySQL, MongoDB.
- AI modelling — AI Engineer; TensorFlow, PyTorch.
- UI/UX — Designer; Figma, Adobe XD.
- App development — React Native and JavaScript.
- Backend — Node.js and Python.
- Testing — QA Tester and tracking tools.

## 6. Risk assessment

| Risk | Impact described in source | Proposed mitigation |
|---|---|---|
| Technical skill gap with OpenCV/MediaPipe | Development/integration delay; one table estimates a 40% increase | Intensive training, pre-trained models, and consultation with AI specialists |
| Hardware constraints on older phones | Lag and poor user experience | TensorFlow Lite optimization and cloud processing for complex tasks |
| Data privacy | Identified as a medium-likelihood/high-impact risk in one table | Encryption and secure communication protocols |

## 7. Team contribution and learning value

The team consisted of five students. My reported responsibility was leading the team and designing/organizing the final report. The document demonstrates academic practice in system requests, feasibility analysis, work planning, WBS, staffing plans, risk identification, and structured project documentation.

## 8. Limitations

This is a university proposal and project-planning deliverable. It is not evidence that a working AI application was built, deployed, or tested with real gym users. The financial values and inconsistent dates should be verified with the team before being defended as accurate results.
