# Key Learnings from CS221 Lecture 1: Introduction to AI

The lecture covers AI history, challenges, paradigms, and course overview, emphasizing foundational concepts likely testable on exams like winters, key figures, model types, and optimization basics.[file:18]

## Key Learnings

1. **Dartmouth Workshop (1956)**: Organized by John McCarthy (founded Stanford AI Lab), with Marvin Minsky, Claude Shannon; aimed to simulate every aspect of learning/intelligence precisely.[file:18]

2. **John McCarthy**: Organized 1956 Dartmouth workshop; founded Stanford AI Lab; symbolic/logical AI tradition.[file:18]

3. **Marvin Minsky**: Participant in Dartmouth; co-author of *Perceptrons* (1969) with Seymour Papert, showed linear classifiers fail XOR; shifted AI to symbolic/logic.[file:18]

4. **Claude Shannon**: Dartmouth participant; information theory pioneer.[file:18]

5. **First AI Winter**: Caused by machine translation failure (e.g., "The spirit is willing but the flesh is weak" → Russian → "The vodka is good but the meat is rotten"); government funding cut; issues: insufficient compute, exponential search, lack of language experience.[file:18]

6. **Contributions from early AI**: Lisp (high-level languages, garbage collection), time-sharing, modeling/inference separation.[file:18]

7. **Second AI Wave (1970s-80s): Knowledge/Expert Systems**: Encoded rules for narrow tasks (e.g., disease diagnosis, parts orders); first industrial impact; failed due to brittle rules, manual maintenance, over-promising.[file:18]

8. **Second AI Winter**: Collapse from knowledge limitations.[file:18]

9. **McCulloch & Pitts (1943)**: Neuroscientist/logician; theory of artificial neural networks linking neurons to logic; roots of deep learning.[file:18]

10. **Backpropagation (1980s rediscovery)**: Generic algorithm for training multilayer neural networks.[file:18]

11. **Yann LeCun (1989)**: Applied convolutional neural networks (CNNs) for handwritten digit recognition; deployed by USPS for ZIP codes.[file:18]

12. **AlexNet (2012)**: Transformed computer vision via ImageNet gains.[file:18]

13. **AlphaGo**: Neural networks mastered Go (logic puzzle); bridges symbolic/logical and neural traditions.[file:18]

14. **AI Draws From**: Statistics (maximum likelihood), economics (games), optimization (gradient descent).[file:18]

15. **AI as Agents vs. Tools**: Agents recreate intelligence (perception, motor, language, knowledge, reasoning, learning); tools augment humans (e.g., satellite GDP prediction, datacenter cooling).[file:18]

16. **Human vs. Machine Learning**: Humans learn diverse tasks from few examples; machines excel narrowly with massive data/compute.[file:18]

17. **Deployment Challenges**:
    - Adversarial examples (e.g., glasses fool face recognition; stickers fool stop signs).[file:18]
    - Biases (e.g., Google Translate: Malay "she nurse/he programmer"; COMPAS recidivism tool biased by race).[file:18]
    - Fairness conflicts (e.g., equal false positives vs. equal reoffense rates mathematically incompatible).[file:18]

18. **Modeling-Inference-Learning Paradigm**:
    - **Modeling**: Simplify real world mathematically (e.g., city as graph).[file:18]
    - **Inference**: Ask questions (e.g., shortest path).[file:18]
    - **Learning**: Fit parameters from data (e.g., graph edge costs).[file:18]

19. **Model Hierarchy (Low to High Intelligence)**:
    - **Reflex Models**: Fixed computations, no feedback (linear classifiers, DNNs).[file:18]
    - **State-Based Models**: States/actions (search, MDPs/randomness, games/adversarial; e.g., Pac-Man, robotics).[file:18]
    - **Variable-Based Models**: Assignments under constraints (CSPs hard constraints; Bayesian networks soft; e.g., Sudoku, car tracking).[file:18]
    - **Logic**: Heterogeneous info, deep reasoning (e.g., Prolog-like demo: Alice student/person/hot Phoenix/snowing/unhappy).[file:18]

20. **Course Topics**: ML (generalization), reflex/state/variable/logic models; optimization (DP discrete, gradient descent continuous).[file:18]

21. **Discrete Optimization Example: Edit Distance**: Min inserts/deletes/substitutions (S to T); DP recurrence on prefixes (match: recurse(m-1,n-1); mismatch: min(sub+recurse(m-1,n-1), del+recurse(m-1,n), ins+recurse(m,n-1)); memoize to avoid exponential redundancy.[file:18]

22. **Continuous Optimization Example: Regression**: Least squares min ∑(w*x_i - y_i)^2; gradient descent: w -= η * ∑2*x_i*(w*x_i - y_i).[file:18]

## Historical Names & Achievements Summary

| Name              | Key Achievement(s)                          |
|-------------------|---------------------------------------------|
| John McCarthy    | Dartmouth 1956; Stanford AI Lab; symbolic AI [file:18] |
| Marvin Minsky    | Dartmouth; *Perceptrons* (1969) killed single-layer NNs [file:18] |
| Claude Shannon   | Dartmouth; info theory [file:18]            |
| McCulloch & Pitts| 1943 neural networks (neurons=logic) [file:18] |
| Seymour Papert   | *Perceptrons* with Minsky [file:18]         |
| Yann LeCun       | 1989 CNN digits/USPS ZIP [file:18]          |

No explicit "four components of AI" list, but human capabilities: perception, motor control, language, knowledge (declarative/procedural), reasoning, learning.[file:18]