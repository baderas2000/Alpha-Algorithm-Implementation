# Alpha Miner Implementation - README

## 1. Approach

### 1.1. Language, Tools, and Libraries
- The Alpha Miner algorithm was implemented using **Python**.
- **Google Colab** was selected as the development environment, as it facilitated easy collaboration.
- For reading XES files (process logs), we utilized the `read_xes()` method from the **PM4PY** library.
- For generating a visual representation of the **Petri-Net**, we used the **Snakes** library.

#### General Workflow
1. We begin by reading the log files and identifying the start and end tasks.
2. Temporal dependencies between events were identified.
3. We created sets of four types of dependencies, which formed the base for generating the Petri-Net.
4. The output is a Petri-Net that represents the process model.

### 1.2. Challenges
- The current implementation has some inaccuracies and requires fine-tuning.
- The main issue is using **causal relations** as the base for generating the Petri-Net, which causes problems with differentiating between different kinds of splits.
- Future refinements are planned to address these issues, especially for our own learning purposes.

### 1.3. How to Run
To run the code:
- Open the provided **Google Colab** notebook.
- Press the "Run" button to execute the cells sequentially.
- All required libraries will be automatically installed within the environment, making the process straightforward.

### 1.4. Team Collaboration
- The team worked collectively without strict task separation.
- Meetings were held regularly to learn, brainstorm, and implement the code together.

---

Feel free to reach out for more details or troubleshooting.
