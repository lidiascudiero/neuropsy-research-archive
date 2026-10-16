# MSc Thesis (2023): Clinical traits and cognitive processing 

**Research Objective:** investigation into the interaction between clinical traits (Attachment, Anxiety) and cognitive processing (Attention, Memory, Interpretation).

---

##  Ethics and privacy
* **Institutional Approval:** approved by the Ethics Committee of the **University of Campania "Luigi Vanvitelli"**.
* **Informed Consent:** mandatory digital consent block (6 requirements) before participation.
* **Data Privacy:** guaranteed absolute anonymity through custom-generated codes.

---

## Experimental protocol and task sequence
The study was divided into multiple sections, implemented via **PsyToolkit** scripting:

###  Phase 1: Assessment and psychometrics
1. **Demographics:** age, gender, sexual orientation, and relationship status.
2. **ECR-12 (Experience in Close Relationship):** a 12-item self-assessment scale measuring adult attachment styles.
3. **STAI-Y2 (State-Trait Anxiety Inventory):** a 20-item inventory evaluating generic stress and trait anxiety.
4. **LCSQ (Looming Cognitive Style Questionnaire):** evaluation of cognitive reactions to hypothetical threat scenarios.
   * *Technical Note:* implemented using `range` sliders (1-5) for subjective threat probability.
5. **AST (Ambiguous Scenarios Test):** measuring interpretation bias in social stories.
   * *Technical Note:* Implemented using `rank` logic to order possible behavioral responses.

###  Phase 2: Cognitive pradigms
6. **Posner Cueing Task:** spatial attention task.
   * *Procedure:* participants respond to a green "X" appearing on the left or right after a visual cue.
   * *Logic:* Fixation (500ms) → Cue (200ms) → Delay (500ms) → Target.
7. **Recognition Memory task:** encoding and retrieval of emotional stimuli.
   * *Procedure:* presentation of images (emotional/neutral) and subsequent recognition test.
   * *Logic:* 1000ms image presentation followed by an Old/New discrimination phase.

---

###  Experimental Interface preview
Below is a visual representation of the cognitive tasks implemented in Phase 1 (Ambiguous Scenarios Test) and 2 (Posner and Memory Recognition):

![Experimental Tasks](task.png)

*The image shows the visual stimuli and response interface designed via PsyToolkit scripting.*

## Technical scripts (.psy)
The scripts in this folder demonstrate advanced **PsyToolkit** capabilities:
* `assessment_battery.psy`: Handles points 1 to 5, including custom anonymization logic.
* `posner_cueing_task.psy`: Implements the attentional shift paradigm.
* `recognition_memory_task.psy`: Manages the stimuli randomization and memory encoding/retrieval.

---


##  Technical implementation
* **Modular Scripting:** separate files for psychometric batteries and cognitive tasks to optimize data flow.
* **Ethics and GDPR:** mandatory digital consent blocks and custom anonymization algorithms for full data protection.

---

##  Experimental results

The study was implemented via PsyToolkit and analyzed using IBM SPSS v21.0. 

### Assessment and psychometrics
* **ECR-12 & STAI-Y2:** Integrated assessment of adult attachment styles and trait anxiety.
* **Looming Cognitive Style (LCSQ):** anxious individuals perceived physical threats as significantly more imminent and "speeding up" compared to secure and avoidant groups.
* **Ambiguous Scenarios Test (AST):** disorganized attachment styles showed a significant bias toward "Anger" interpretations in social scenarios.
### Cognitive Paradigms & Findings
* **Posner Cueing Task:** * anxious participants showed a trend toward faster overall reaction times.
    * General findings across all groups indicated an initial avoidance of positive stimuli (100ms) followed by difficulty disengaging from both positive and negative cues (500ms).
* **Old-New Recognition Task:** * negative social stimuli were recognized with higher accuracy compared to neutral and positive ones.
    * Positive images were more likely to cause "false alarms," showing a higher response bias (mistaken for already seen).
### Data Logic
* **Data Wrangling**: used Excel for cleaning raw reaction time (RT) data and aggregating psychometric sub-scores from ECR-12, STAI-Y2, LCSQ, and AST.
* **Statistical Modeling**: conducted via **IBM SPSS v21.0** using **ANOVA**, **MANOVA**, and **Pearson correlations** to identify significant interactions between clinical traits and cognitive performance.
* **Assets**: Stimuli selected and validated through a pilot study focusing on valence and arousal to ensure high experimental control.

---

##  References
* **Posner, M. I. (1980).** Orienting of attention.
* **Brennan, K. A., et al. (1998).** ECR scale.
* **Spielberger, C. D. (1983).** STAI inventory.
* **Riskind, J. H., et al. (2000).** LCSQ.
* **Berna, G., et al. (2011).** AST.
