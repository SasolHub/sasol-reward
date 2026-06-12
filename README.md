# 🛢️ Sasol Rewards — Customer Service Live Dashboard

A fully interactive, real-time customer service analytics dashboard built for the Sasol Rewards programme. Upload any ServiceNow Excel export and the entire dashboard auto-refreshes instantly 

🔗 Live Real-Time: https://asanda-khumalo20.github.io/sasol-reward/
📋 Features

📊 KPI Cards


Total Records, Closed, New, Open/Pending, Critical (P1), Agents Active, Resolved, Awaiting Info
All counts update live based on active filters


🔍 Filters & Search


Search by Customer Name, Reference Number, Mobile Number, Agent Name
Filter by Channel, Call Type, State, Priority, Date Range
(Blank) channel option to isolate records with no channel assigned
Reset All clears every filter instantly


⏱️ Case Aging Panel

Real-time breakdown of all Open / Pending cases by how long they have been open:

BandRule🔴 OverdueOlder than 2 months (> 60 days)🟡 AgingBetween 1 and 2 months (30–60 days)🟢 RecentLess than 1 month (< 30 days)


Each band shows count, % of open cases, and top call types within that bucket
Click any band to expand a drilldown table showing every case with days open


📡 Channel Breakdown


Full table: Phone / Email / Mobile App / Blank with state sub-counts (Closed, New, Open, Pending, Awaiting, Resolved, Cancelled)
Total row with grand counts
Mini tiles for quick overview
Click any row or tile to filter the entire dashboard to that channel


📱 Call Type, Service & Summary Panels


State Summary, Priority Summary, Channel Summary
Service Summary, Category Summary
Call Purpose Summary, Call Type Summary
All with progress bars and percentage breakdown


👤 Agent Performance Table


Count per agent: Total, Closed, Open, New, Pending, Awaiting Info, Resolved, Cancelled, % Closed
Sortable by any column
Auto-updates on every filter


📈 3D Agent Charts


3D Bar Chart — total cases per agent with 3D depth effect
3D Line Chart — multi-line trend (Total, Closed, Open, New, Resolved) with glow points
Grouped Bar — side-by-side state breakdown per agent
Stacked Bar — stacked state composition per agent
Controls: Top 10/15/20/30/All agents, sort by Total/Closed/Open/New


📄 Records Table


All records with: Ref #, Channel, Mobile, Customer, Call Type, State (colour-coded badge), Priority (colour-coded badge), Opened date/time, Opened By, Call Purpose, Service
Sortable by any column
Paginated (100 rows per page)



📂 How to Use

Load Your Own Data


Click "Load New Excel" in the top-right header
Select any .xlsx or .xls ServiceNow export
The entire dashboard auto-refreshes — all panels, charts, aging, and filters update instantly
A toast notification confirms the file name and record count loaded


Supported File Formats

The dashboard auto-detects column names and works with multiple ServiceNow export formats:

Column in FileDashboard FieldNumber / RefReference NumberCall Type / Short descriptionCall TypeChannelChannelState / StatusStatePriorityPriorityOpened / Updated / CreatedDate OpenedOpened by / Assigned ToAgentCustomer Name / ContactCustomer First NameCustomer SurnameCustomer SurnameMobile NumberMobileCall Purpose / Action statusCall PurposeService / AccountServiceCategoryCategory


🛠️ Built With

TechnologyPurposeHTML5 / CSS3Structure and stylingVanilla JavaScriptAll logic, filtering, and renderingSheetJS (xlsx.js)Excel file parsingChart.jsAgent performance chartsGoogle Fonts (Inter, Rajdhani)Typography

No frameworks. No backend. No database. Runs entirely in the browser.


📁 Project Structure

sasol-reward-dashboard/
│
└── index.html        # Single-file dashboard — all CSS, JS, and data embedded


🎨 Design


Colour scheme: Sasol Blue (#003087) and White
Theme: Clean, professional, corporate
Responsive: Works on desktop and tablet screens
Live clock in header (South African locale)
Toast notifications for file load events
Colour-coded state badges and priority badges throughout



👤 Author

Asanda Khumalo

Sasol Rewards — Customer Service Analytics

📍 South Africa


📄 Licence

This project is for internal Sasol Rewards reporting purposes.

Data loaded into the dashboard is processed entirely client-side and is never uploaded to any server.
