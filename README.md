# DOnder's Reaction Time Experiment

This project is a web-based implementation of a classic cognitive psychology experiment designed to measure the duration of specific mental processes. It is based on F.C. Donders' subtraction method, which infers the time taken for a mental operation by subtracting the reaction time of a baseline task from a more complex one.

The experiment consists of three distinct tasks, each building upon the last to isolate different cognitive stages.



---

## 🧪 The Tasks

The experiment guides the user through three sequential tasks:

* **Task A: Simple Reaction Time**
    * **Objective:** Measure the baseline time for stimulus detection and motor response.
    * **Procedure:** A green circle appears on the screen. The participant must press the **SPACEBAR** as quickly as possible.

* **Task B: Categorization (Go/No-Go)**
    * **Objective:** Adds a stimulus identification and categorization stage.
    * **Procedure:** A random number (1-9) appears. The participant must press **'J'** if the number is **EVEN** and **'K'** if it is **ODD**.

* **Task C: Mental Arithmetic (Choice Reaction)**
    * **Objective:** Adds a further cognitive load of evaluation and decision-making.
    * **Procedure:** A simple addition equation appears (e.g., "2 + 4 = 6"). The participant must press **'J'** if the equation is **TRUE** and **'K'** if it is **FALSE**.

---

## 🔬 The Subtraction Method

The results are analyzed using Donders' method:

1.  **Time for Categorization** = (Average RT of Task B) - (Average RT of Task A)
    * This isolates the time it takes to identify a stimulus (as odd/even) and select the correct response.

2.  **Time for Mental Arithmetic** = (Average RT of Task C) - (Average RT of Task B)
    * This isolates the additional time required to perform the mental calculation and verify its truthfulness.

---

## 🚀 Installation & Usage

This experiment is designed to run entirely in a web browser with no complex setup required.

### Running Locally

1.  **Download the Code:** Save the `index.html` file to your computer.
2.  **Open in Browser:** Double-click the `index.html` file. It will open in your default web browser (like Chrome, Firefox, or Edge).
3.  **Run the Experiment:** Follow the on-screen instructions.

**Note:** An internet connection is recommended on the first run to cache the Tailwind CSS and Google Fonts files for proper styling. After that, it should work offline. The Firebase functionality will be ignored when run locally without configuration.

---

## 📊 Data Output

At the end of the experiment, a summary table of your results is displayed.

You also have the option to download your complete raw trial data by clicking the **"Download Raw Data (CSV)"** button. The CSV file includes the following columns for each trial:

* `userId`: A unique identifier for the participant.
* `task`: The task type (A, B, or C).
* `trial`: The trial number within the task.
* `stimulus`: The stimulus that was shown.
* `response`: The key that was pressed.
* `isCorrect`: Whether the response was correct (`true`/`false`).
* `rt`: The reaction time in milliseconds (ms).
