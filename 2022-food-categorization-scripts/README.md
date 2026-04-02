# [2022] Food Categorization & Body Image Study 

**Research Objective:** This project investigates the facilitatory effect of context on food categorization and its correlation with body image dissatisfaction and BMI.

---

## Experimental Design & Modules

The study is structured into two main technical modules implemented via **PsyToolkit**:

### 1. Assessment & Psychometrics (`assessment_and_surveys.psy`)
* **Biometrics & BMI:** Automated collection of height and weight for real-time **Body Mass Index (BMI)** calculation.
* **Lifestyle Analytics:** Scripted assessment of dietary habits (e.g., omnivorous, ketogenic, Mediterranean), food intolerances, and physical activity levels (amateur vs. competitive).
* **Body Dissatisfaction Scale (BDS):** Implementation of the silhouette-based test (Mutale et al., 2016).
    * **Logic:** Participants select their "Real Self" vs. "Ideal Self" among 9 figures (ranging from extremely thin to extremely obese) to quantify body dissatisfaction.

### 2. Interactive "Scaffale" Task & Post-Task Evaluation (`food_categorization_task.psy`)
* **Task Mechanics:** A drag-and-drop paradigm where participants categorize 20 food stimuli (10 healthy, 10 unhealthy) onto a 5-shelf unit.
* **Stimuli Management:** Randomization of images selected from the **Food-475** and **Food101** databases, matched for shape and size.
* **Food Preference & Healthiness Assessment:** Following the shelf task, participants evaluated all 20 food stimuli using two 5-point Likert scales:
    * **Preference Rating:** *"How much do you like the food shown in the photo?"* (1 = "Not at all" / 5 = "Very much").
    * **Healthiness Rating:** *"How healthy do you consider the food shown in the photo?"* (1 = "Not at all healthy" / 5 = "Very healthy").
* **Logic:** Images (328x268px) were re-presented in a randomized order to eliminate order bias and analyze the consistency between behavioral categorization and explicit judgment.

---

## Visual Implementation
The following images provide a preview of the experimental interface designed for this study:

### The "Scaffale" (Shelf) Task
![Shelf Task Preview](images/shelf_task_preview.png)
*Participants categorize food items by dragging them into the appropriate shelf level.*

### Food Rating Interface
![Food Rating Preview](images/food_rating_preview.png)
*Evaluation interface for subjective food preference and healthiness ratings.*

### Body Dissatisfaction Silhouette Test
![Silhouette Test](images/body_dissatisfaction_test.png)
*The 9-figure scale used to calculate the gap between perceived and ideal body image.*

---

## Technical Logic
* **Modularity:** Separate scripts for the survey and the interactive experiment to optimize data flow.
* **Data Logging:** Automated recording of selection accuracy, Reaction Times (RT), and qualitative ratings.
* **GDPR Compliance:** Full anonymization of participant data through custom-coded IDs.

---

## References
* **Mutale, C., et al. (2016).** Body Dissatisfaction Scale Assessment.
* **Bar, M. (2004).** Visual objects in context.
* **Stoet, G. (2010, 2017).** PsyToolkit software package.
---

##  References
* **Mutale, C., et al. (2016).** Body Dissatisfaction Scale Assessment.
* **Bar, M. (2004).** Visual objects in context.
* **Stoet, G. (2010, 2017).** PsyToolkit software package.
