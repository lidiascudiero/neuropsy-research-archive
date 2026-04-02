# Neuro-Research Archive: Experimental Design & Behavioral Analytics 

This repository is a professional archive of experimental protocols and behavioral scripting developed between 2022 and 2023. It showcases the implementation of high-precision cognitive tasks and psychometric assessments using **PsyToolkit**.

---

##  Projects Included

###  [2023] Visual Attention & Emotional Memory Protocol
Investigation into the interaction between clinical traits and cognitive processing.
* **Core Paradigms:** Posner Cueing Task and Recognition Memory Task.
* **Psychometrics:** Integrated scoring for ECR-12 (Attachment) and STAI-Y2 (Anxiety), AST, (Ambiguous Scenarios Test), LCSQ (Looming Cognitive Style Questionnaire).
* **Logic:** Advanced flow control with conditional branching and custom anonymization algorithms.

###  [2022] Contextual Categorization Task
Group research project on how environmental consistency biases object classification.
* **Core Paradigm:** Interactive "Scaffale" (Shelf) task.
* **Experimental Logic:** Managing stimuli randomization and response bias in context-dependent environments.

---

##  How to Use the Code

These projects require the **PsyToolkit** software or the **PsyToolkit platform** ([psytoolkit.org](https://www.psytoolkit.org/)).

1. **Create an Account:** Register on [psytoolkit.org](https://www.psytoolkit.org/).
2. **Upload Files:** Create a new experiment/survey and upload the `.psy` scripts found in this repository.
3. **Manage Assets:** Upload the necessary bitmaps/images mentioned in the script tables (e.g., stimuli for the shelf or memory tasks).
4. **Compile & Run:** Use the online platform to compile the code. You can run the experiment online or download the HTML file for offline execution.
5. **Integration:** You can create a survey and include these experiments as part of a larger research battery.

---

## Software Attribution & Mandatory Citations

PsyToolkit is a free-to-use toolkit created by **Prof. Gijsbert Stoet** (Professor in Psychology - Essex University, UK). If you use this code for academic studies or student projects, it is essential to cite the following articles:

* **Stoet, G. (2010).** PsyToolkit - A software package for programming psychological experiments using Linux. *Behavior Research Methods*, 42(4), 1096-1104.
* **Stoet, G. (2017).** PsyToolkit: A novel web-based method for running online questionnaires and reaction-time experiments. *Teaching of Psychology*, 44(1), 24-31.

*If you find this repository helpful, a mention or link to this GitHub page (https://github.com/lidiascudiero) is appreciated.*

---

##  Ethics & Data Handling
All protocols were designed following strict ethical guidelines:
* **GDPR Compliance:** Implemented custom anonymization logic to generate unique, non-identifiable participant codes.
* **Informed Consent:** Mandatory digital consent blocks before any data collection.
* **Scoring:** Automated calculation of clinical thresholds (e.g., STAI-Y2 score $\ge 40$ for anxiety presence).

