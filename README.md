# 🔧 Business Process Mapping & Optimization Case Study

A consulting-style **Business Analyst** case study that maps an organisation's core
operational processes, quantifies **bottlenecks, cost, SLA performance, and rework**, and
recommends a data-backed **To-Be** process design. Delivered as a single, executive-ready
**Excel dashboard** plus a full recommendation report.

---

## 🎯 Objective
Identify inefficiencies across business processes, map the workflow, analyse bottlenecks,
and propose optimisation strategies (automation, standardisation, redesign) that cut cycle
time and cost while lifting SLA achievement.

## 🧩 Business Problem
A mid-sized services organisation runs 110 recurring process activities across six
departments (Finance, HR, Procurement, Customer Service, Operations, Sales). Leadership sees
rising costs, SLA breaches, and customer complaints but lacks visibility into *where* time
and money are lost. This project turns raw process logs into a clear improvement roadmap.

## 🏢 Case Study Background
The dataset ([`data/business_process_data.csv`](data/business_process_data.csv)) captures
each process activity end-to-end: owner, resource, duration, waiting/approval time, task
volume vs completion, errors, rework, cost, SLA target/achievement, complaints, status, and
the identified improvement opportunity — **21 fields, 110 records**.

## 🗺️ Process Mapping Methodology
1. **Stakeholder & SIPOC analysis** — define suppliers, inputs, process, outputs, customers.
2. **As-Is mapping** — document the current workflow and hand-offs per department.
3. **Bottleneck analysis** — rank activities by waiting/approval time and cost.
4. **Root-cause & gap analysis** — why delays, errors, and rework occur.
5. **To-Be design** — automation/standardisation/redesign of the worst offenders.
6. **Impact & cost-benefit analysis** — quantify the before-vs-after opportunity.

## 📊 Analysis Performed
Process Cycle Time, Waiting & Approval Time, Process Cost & Cost-per-Transaction,
SLA Achievement %, Error Rate %, Rework Rate %, Productivity %, and Customer Complaint Rate —
sliced by department, activity, resource, and improvement opportunity.

## ✅ Optimization Recommendations
- Automate the highest-waiting activity (**Data Entry**) and routine approvals/data-entry.
- Redesign cost-heavy processes in **Procurement**; remove non-value-added steps.
- Rebalance resources toward **Customer Service** to recover SLA achievement.
- Standardise rework-prone steps to drive the error rate below current **5.6%**.

## 📈 Dashboard Features (interactive, single landscape page)
An **interactive Excel dashboard** built on native **PivotTables, PivotCharts, and Slicers**, laid out on one landscape page that fits a single screenshot:
- **Slicers (left rail):** **Department, Process Status, Improvement Opportunity** — click any value and **every chart and KPI re-filters instantly** (all four PivotCharts and the KPI cards share one PivotCache).
- **KPI band (top):** Avg Cycle Time, SLA Achievement %, Avg Process Cost, Avg Error Rate, Avg Productivity — live `GETPIVOTDATA` cards that update with the slicers.
- **PivotCharts (2×2):** Avg Cycle Time by Department, Bottleneck — Avg Waiting Time by Activity, Total Process Cost by Department, SLA Achievement % by Department.
- **Recommendations panel** at the bottom; the raw data is a filterable Excel **Table** (`tblProcess`) on the `Data` sheet.

> Built natively in Excel (PivotTables sourced from the named Table), following the method in `Pivot Tables in Excel using claude.docx`.

## 💡 Key Insights
- Bottleneck: **Data Entry** activities have the highest avg waiting time (**67 min**).
- Costliest department: **Procurement** (₹26,470 total process cost).
- Weakest SLA: **Customer Service** at **35%** achievement.
- Overall productivity **90.2%**, error rate **5.6%**, SLA **49.1%**.

## 🗂️ Repository Structure
```
Business Process Mapping & Optimization Case Study/
├─ README.md
├─ Business Process Mapping & Optimization Case Study.docx   # brief
├─ Project Descriptions (Resume + ATS).docx
├─ data/business_process_data.csv
├─ dashboard/Business_Process_Optimization_Dashboard.xlsx
├─ reports/Business Recommendation Report.docx
├─ docs/ (dashboard_image_prompt.md, screenshots/)
└─ Linkedin Post/linkedin_post.docx
```

## 🧾 Conclusion
The case study demonstrates the full Business Analyst toolkit — SIPOC, As-Is/To-Be mapping,
bottleneck and root-cause analysis, and cost-benefit-backed recommendations — packaged as a
recruiter-ready Excel dashboard and report that turn process data into measurable savings.
