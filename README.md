# 🧩 Sudoku Solver using AI (CSP, AC-3, Backtracking)

## 📌 Overview

This project is an intelligent **Sudoku Solver** built using concepts from **Artificial Intelligence** and **Constraint Satisfaction Problems (CSP)**.
It efficiently solves Sudoku puzzles of varying difficulty levels (Easy to Very Hard) by combining multiple optimization techniques.

The solver ensures consistency using **AC-3 (Arc Consistency Algorithm)** and finds solutions using **Backtracking Search** enhanced with heuristics.

---

## 🧠 Techniques Used

This project applies the following AI techniques:

### 🔹 1. Constraint Satisfaction Problem (CSP)

* Each cell is treated as a variable.
* Domain: Values from 1 to 9.
* Constraints:

  * No repetition in rows
  * No repetition in columns
  * No repetition in 3×3 subgrids

---

### 🔹 2. AC-3 Algorithm (Arc Consistency)

* Reduces the domain of variables before search begins.
* Ensures that all variable pairs satisfy constraints.
* Improves efficiency by eliminating invalid values early.

---

### 🔹 3. Backtracking Search

* Recursively assigns values to variables.
* If a conflict occurs, the algorithm backtracks.
* Guarantees a complete and correct solution.

---

### 🔹 4. Forward Checking

* After assigning a value, it removes that value from neighboring domains.
* Detects failure early and reduces unnecessary computation.

---

### 🔹 5. Heuristics (Optimization)

#### ✅ MRV (Minimum Remaining Values)

* Selects the variable with the smallest domain.

#### ✅ Degree Heuristic

* Chooses the variable that affects the most unassigned neighbors.

#### ✅ Least Constraining Value (LCV)

* Selects values that minimize restrictions on other variables.

---

## ⚙️ Features

✔ Solves multiple Sudoku boards automatically
✔ Supports Easy, Medium, Hard, and Very Hard puzzles
✔ Uses advanced AI techniques for efficiency
✔ Displays formatted Sudoku boards
✔ Tracks performance statistics:

* Number of recursive calls
* Number of failures

---

## 📂 Project Structure

```
sudoku-solver/
│
├── sudoku_solver.py   # Main solver code
├── README.md          # Project documentation
```

---

## ▶️ How to Run

### Step 1: Clone or Download

Download the project or clone it using:

```
git clone https://github.com/your-username/sudoku-solver.git
```

### Step 2: Run the Program

Make sure Python is installed, then run:

```
python sudoku_solver.py
```

---

## 📊 Example Output

```
Easy Board

Input:
. . 4 | . 3 . | . 5 .
6 . 9 | 4 . . | . . .
. . 5 | 1 . . | 4 8 9
------+-------+------
. . . | . 6 . | 9 3 .
3 . . | 8 . 7 | . . 2
. 2 6 | . 4 . | . . .
------+-------+------
4 5 3 | . . 9 | 6 . .
. . . | . . 4 | 7 . 5
. 9 . | . 5 . | 2 . .

Solution:
(Generated solved Sudoku will appear here)

Statistics:
BACKTRACK calls   : XXXX
BACKTRACK failures: XXXX
```

---

## 🚀 Performance

The combination of **AC-3 + Backtracking + Heuristics** significantly reduces:

* Search space
* Execution time
* Number of failures

This makes the solver efficient even for very hard puzzles.

---

## 🎯 Learning Outcomes

Through this project, you will understand:

* How CSP works in real-world problems
* Constraint propagation (AC-3)
* Search algorithms and optimization
* AI-based problem solving techniques

---

## 🔮 Future Improvements

* Add GUI (Graphical User Interface)
* Accept user input dynamically
* Visual step-by-step solving
* Web-based Sudoku solver

---

## 👨‍💻 Author

Abdullah Ahmad

---

## ⭐ Support

If you like this project:

* Give it a ⭐ on GitHub
* Share it with others
* Use it in your AI/DSA projects

---

## 📜 License

This project is open-source and free to use for educational purposes.
