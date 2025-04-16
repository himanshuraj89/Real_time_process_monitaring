# Real-Time Process Monitoring Dashboard

A responsive, real-time dashboard that monitors CPU and memory usage using Python, Dash, and Plotly. This project is ideal for understanding system performance and building a customizable system monitoring tool using web technologies.

---

## 🧠 Project Overview

This dashboard provides real-time system performance insights with:

- CPU usage graph updating every 2 seconds
- Memory usage graph with real-time statistics
- Beautiful dark-themed UI with card-style components
- Asynchronous system data fetching using background threading
- Modular structure allowing for further expansion (e.g., process table, disk stats)

---

## 🚀 Features

- 📊 **Live CPU and Memory Graphs**  
  Visually track system performance metrics over time.

- 🎨 **Responsive & Stylish Layout**  
  Custom styling using a modern card layout and dark background.

- ⚙️ **Efficient Data Updates**  
  Uses threading for collecting system data without blocking the UI.

- 📦 **Expandable Architecture**  
  Designed to add more performance metrics (e.g., processes, I/O, network).

---

## 🛠️ Technologies Used

| Tool         | Purpose                             |
|--------------|-------------------------------------|
| Python       | Programming language                |
| Dash         | Web framework for dashboards        |
| Plotly       | Graphing and charting library       |
| psutil       | Access system resource information  |
| Threading    | Background data collection          |

---

## 📁 Project Structure

os_project/
├── assets/
│   └── style.css              # Custom styling (optional/expandable)
├── data_collection (1).py     # Main dashboard script
└── requirements.txt           # Required dependencies


---

## 📦 Installation

Follow the steps below to set up the project:

1. **Clone or download** the repository and navigate to the directory.

2. **Install required libraries**:

   ```bash
   pip install -r requirements.txt


### 🧪 How It Works

- The dashboard layout is built using Dash components (`html.Div`, `dcc.Graph`, `dcc.Interval`).
- The script uses a background thread (`Thread`) to fetch CPU and memory data every 2 seconds using `psutil`.
- Data is stored in `deque` containers for a rolling window of 10 seconds.
- Graphs auto-update via Dash’s `dcc.Interval` and callback mechanism.


### 🔮 Future Improvements

- Add process table with sorting and filtering
- Monitor disk and network I/O statistics
- Export performance metrics to CSV or a database
- Add real-time alert notifications (e.g., high CPU usage)
- Add authentication and multi-user access control (optional)

