# **AC²: Understanding Architectural Changes in Python Projects**

✅ **Published in:**  
📚 [**29th ACM Joint Meeting on European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2021)**](https://2021.esec-fse.org)  

---

### 📄 **Abstract**
As open-source projects adopt **faster release cycles**, it becomes challenging for developers to **maintain architectural consistency** while incorporating new changes.  

💡 **The Challenge:**
- Keeping software architecture in-check across multiple releases.
- Tracking evolving complexity in Python projects over time.

🔍 **Our Solution:**
We introduce **AC²**, a visualization tool that helps users analyze **architectural changes** at multiple levels of abstraction. AC² uses:
- 📊 **Call Graphs** and **Collaboration Graphs** to depict interactions between architectural components.
- 🔎 **Four interactive views** to visualize architectural changes between two project releases.
- 📈 Insights into **increasing complexity** of project architecture, empowering maintainers and developers to make informed decisions.

---

### 🚀 **Key Features**
-  **Compare Two Releases:** Compare and visualize architectural changes between two project releases.
-  **Examine Architectural Alterations:** Analyze differences at both higher and lower abstraction levels.
-  **Identify Complexity Trends:** Monitor growing complexity over multiple releases.

---

### 🎥 **Demo & Download**
👉 **Demo:** [Watch the Demo](https://www.youtube.com/watch?v=GNrJfZ0RCVI)  
📥 **Download:** [AC² GitHub Repository](https://github.com/rishalab/AC2)

---

### 📂 **Directory Structure**
```
AC2/
├── file_map_engine/             # Engine for mapping files and generating call/collaboration graphs
│   ├── ast_engine.py            # Parses and analyzes AST for Python files
│   ├── ast_helper.py            # Provides utility functions for AST analysis
│   ├── call_dir.py              # Processes and maps call graphs
│   └── engine.py                # Main engine to process repositories
├── static/                      # Contains cohesion data for the target repository
├── target_repo_dir/             # Stores tags of the target repository
├── templates/                   # HTML templates for web interface
│   ├── home.html
│   └── index.html
├── main.py                      # Main application script
└── requirements.txt             # List of required Python packages
```

---

### 🧠 **Cohesion Value Interpretation (Using LCOM)**

- 🎯 `== 1` – Highly cohesive class (✅ Good class)
- ⚠️ `>= 2` – Low cohesion, class should be split into smaller classes
- ❌ `== 0` – No methods in class (Bad class)

---

## 🛠️ **Installation**

1. **Clone or download** the GitHub repository:
```bash
git clone https://github.com/eashaan-rao/AC2.git
```

2. **Navigate to the main directory:**
```bash
cd AC2/src/main
```

3. **Install required dependencies:**
```bash
pip install -r requirements.txt
```

---

## 🚀 **Usage**

1. **Run the application:**
```bash
python main.py
```

2. Open your browser and go to:
```
http://localhost:5000/
```

3. **Analyze a GitHub repository:**  
- Enter a Python GitHub Repository link and press **Enter** to generate annotated graphs.
![](demo_image_1.png)

4. **Compare two releases:**  
- Compare annotated **call graphs** and **collaboration graphs** for different versions of a repository.
![](demo_image_2.png)

---

### 📢 **Citation**
If you find this work useful, please cite:

```bibtex
@inproceedings{10.1145/3468264.3473120,
  author    = {Rao, A. Eashaan and Vagavolu, Dheeraj and Chimalakonda, Sridhar},
  title     = {AC²: towards understanding architectural changes in Python projects},
  booktitle = {Proceedings of the 29th ACM Joint Meeting on European Software Engineering Conference and Symposium on the Foundations of Software Engineering},
  year      = {2021},
  pages     = {1555–1559},
  doi       = {10.1145/3468264.3473120},
  location  = {Athens, Greece},
  series    = {ESEC/FSE 2021}
}
```

---

## 👥 **Team**
- **Dheeraj Vagavolu**
- **A. Eashaan Rao**
- **Sridhar Chimalakonda**  
  [**RISHA Lab**](https://rishalab.in) – Research in Intelligent Software and Human Analytics Lab, IIT Tirupati

---

## 🎯 **Future Work**
- 🔍 Incorporate support for additional languages beyond Python.
- 📈 Extend visualizations to depict architectural drift over time.
- 🧩 Improve handling of larger repositories to enhance performance.

---

### 🤝 **Contributing**
We welcome contributions! If you’d like to improve **AC²** or add new features:
- Submit a pull request 🚀
- Open an issue with suggestions 💡

