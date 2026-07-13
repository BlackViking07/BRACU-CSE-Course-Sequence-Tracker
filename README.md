# BRACU CSE Course Sequence Tracker

An elegant, high-fidelity, interactive visual curriculum roadmap designed specifically for Computer Science and Engineering (CSE) students. This single-page web dashboard maps out complex course hierarchies across distinct tracking tracks, allowing students to effortlessly visualize, plan, and log their academic progress in real-time.

---

## 🚀 Key Features

*   **Persistent Visual Prerequisite Engine:** Displays full curriculum paths across a multi-column track architecture.
   
    *   🔴 **Solid Crimson Lines:** Hard Prerequisites (HP) that actively lock/unlock advanced course enrollment.
    *   🔵 **Dotted Teal Lines:** Soft Prerequisites (SP) that offer recommended academic pathways without blocking your progress.
      
*   **Path Spotlight / Isolation:** Hovering over any course card dynamically highlights its direct incoming and outgoing prerequisite pathways while beautifully dimming the background lattice for quick scannability.
  
*   **Intelligent Hard Prerequisite Validation:** Prevents accidental tracking. Checking a course box requires all hard prerequisites to be completed first; unchecking a core prerequisite automatically runs a cascading reset on all downstream dependents.
  
*   **Dynamic Foundation Course Mixer:** A customized modal setup for managing non-credit foundation courses (`MAT092` / `ENG091`). Students who place out can instantly waive them, greying out the nodes and directly unlocking advanced tiers (`MAT110` / `ENG101`).
  
*   **Live Credit Analytics:** Dynamically calculates overall program credits completed vs. total remaining, broken down comprehensively by category bars (Program Core, School Core, GenEd, Electives, and Thesis).
  
*   **Local Auto-Save Matrix:** Uses modern browser `localStorage` to save all completed statuses and customized typed names instantly. Your tracker state stays private to you and persists perfectly across page refreshes.

---

## 🛠️ Tech Stack & Architecture

*   **Frontend:** Pure HTML5 & Semantic Content Containers.
*   **Styling Engine:** Custom CSS3 variables, responsive layout grids, flexboxes, and micro-interactions optimized for high scannability.
*   **Graphics Lattice:** Inline Vector SVG (`<svg>`) using dynamically calculated matrix coordinate bindings to map curved paths matching the grid.
*   **Script Logic:** Lightweight, vanilla ES6+ JavaScript handling state cascades, real-time node validation, and event handling. Completely dependency-free.

---

## 📂 Getting Started

Since this project is completely self-contained within a single file, launching it locally is incredibly straightforward:

1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/BlackViking07/BRACU-CSE-Course-Sequence-Tracker.git]
   ```

2. Navigate into the directory:
   ```bash
   cd BRACU-CSE-Course-Sequence-Tracker
   ```

3. Open the ```index.html``` file in any modern web browser (Chrome, Firefox, Edge, or Safari):
   ```bash
   # Or simply double-click the file in your file explorer

   open index.html
   ```


## 📝 Usage Guide

1. Configure Foundation Courses: Upon your first launch, click the Foundation Courses ⚙ button to toggle your placement requirements for ```MAT092``` and ```ENG091```.

2. Log Completed Courses: Click the checkbox on any course card once you have passed it. The dashboard will automatically calculate your earned credits and reveal downstream courses.

3. Customize Flexible Nodes: For Program Electives and GenEd slots, click directly into the integrated text box to type in the exact course code you are registered for.

4. Isolate Pathways: Hover your mouse over any complex node (like ```CSE221``` or ```CSE420```) to map and view its specific requirements clearly.

5. Clear Local Workspace: Use the armed Reset all progress danger button to securely wipe the browser's ```localStorage``` state and start fresh.


## 📄 License

This project is open-source and available under the MIT License. Feel free to fork, customize, and adapt it for your own university curriculum structures!
