# AI-assisted Qualitative Analysis of Reddit Mental Health Reports

## Overview

This project demonstrates an LLM-based agentic workflow for analysing first-person mental health narratives.

The aim is to extract:
- psychological themes
- behavioural mechanisms
- possible intervention targets
- evidence-supported research hypotheses

## Workflow

<img width="1498" height="891" alt="image" src="https://github.com/user-attachments/assets/54138df3-3a03-4429-b3f1-ce289845d2aa" />


## Technologies

- Python
- Jupyter Notebook
- LangChain
- Groq LLM API
- Pydantic structured outputs

## Example analysis and outputs

Generated hypotheses and selected visual summaries are included in the outputs folder.

To illustrate the practical application of each agentic step, example outputs of each step are shown below.

> **Note:** The analysis is exploratory and intended to support qualitative research. LLM-generated interpretations are not diagnoses or clinical recommendations.

### 1. Narrative Analysis

The first stage extracts descriptive information from the narrative before attempting psychological interpretation.

| Category               | Identified content                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Emotions**           | Anxiety, despair, hopelessness, frustration, helplessness, shame                                                                                             |
| **Challenges**         | Financial instability, limited access to education, alcohol misuse, feeling overwhelmed by anxiety                                                           |
| **Coping strategies**  | Self-medication with alcohol                                                                                                                                 |
| **Protective factors** | None explicitly identified                                                                                                                                   |
| **Therapeutic needs**  | Support for underlying difficulties; development of coping strategies beyond self-medication; exploration of future goals; addressing shame and hopelessness |

### 2. Behavioural Mechanism Analysis

The second stage interprets possible behavioural processes underlying the reported experiences.

**Identified mechanisms**

* Avoidance
* Rumination
* Social withdrawal
* Emotion-regulation difficulties
* Maladaptive coping
* Self-medication

**Explanation**

The individual appears to be using maladaptive coping strategies to manage their anxiety and panic, which may be contributing to their overall distress. They also seem to be experiencing difficulties with emotion regulation, which may be driving their use of substances and maladaptive coping strategies.

**Uncertainty**

It is unclear what the underlying causes of the individual's anxiety and panic are, and whether these are related to their sleep anxiety or other factors. Further assessment would be needed to determine the root causes of their distress.


### 3. Intervention mapping

### 3. Intervention Mapping

Based on the behavioural mechanisms identified in the previous stage, the workflow maps the narrative to potentially relevant psychological intervention approaches.

| Intervention                                  | LLM-generated rationale                                                                                                                                          |
| --------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Cognitive Behavioural Therapy (CBT)**       | CBT has been shown to be effective in addressing anxiety, shame, and hopelessness by teaching individuals to reframe their thoughts and develop more adaptive coping strategies. |
| **Dialectical Behaviour Therapy (DBT)**       | DBT has been effective in reducing self-medication and improving emotional regulation in individuals with anxiety, shame, and hopelessness.                                |
| **Solution-Focused Brief Therapy (SFBT)**     | SFBT has been shown to be effective in improving hope and reducing shame in individuals with complex mental health issues.                                       |
| **Mindfulness-Based Stress Reduction (MBSR)** | MBSR has been effective in reducing anxiety and improving emotional regulation in individuals with anxiety and shame.                                            |
| **Trauma-Informed Care (TIC)**                | Was identified by the model as a potentially relevant approach for experiences involving shame and complex psychological distress.                               |

Below you can see a representation of the overall frequency of suggested interventions.

<img width="2440" height="1468" alt="image" src="https://github.com/user-attachments/assets/f89fff10-77c8-4a57-82b8-54ce9e8f3a49" />


### 4. Evidence Traceability

The workflow then links interpretations back to the original narrative.

| Supporting excerpt                                           | Interpretation                                                                                                 |
| ------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------- |
| *“How … do you get better when you have no future.”*         | Indicates perceived hopelessness and limited future orientation.                                               |
| *“No funds for an education.”*                               | Identifies financial and educational barriers that may contribute to perceived lack of opportunity.            |
| *“I’m also an alcoholic cause that helps me forget about …”* | Suggests alcohol is being used as a strategy for reducing or avoiding emotional distress.                      |
| *“Am I past the point of lost?”*                             | Indicates severe uncertainty about the possibility of improvement and a negative appraisal of the self/future. |

This evidence-tracing stage is included to make LLM-generated interpretations more transparent and easier for a researcher to audit.

### 5. Exploratory Research Hypothesis

**Hypothesis**

Individuals with anxiety and shame tend to engage in maladaptive coping mechanisms, such as substance use and avoidance, which exacerbate their mental health issues.

**Rationale**

This hypothesis emerged from the qualitative data as individuals frequently mentioned using substances to cope with their emotions and avoiding challenges due to feelings of anxiety and hopelessness.

**Supporting patterns**

* Maladaptive coping patterns
* Avoidance behaviour
* Substance use as a coping mechanism

**Example supporting evidence**

> *“I’m also an alcoholic cause that helps me forget about …”*

This quote indicates that the individual is self-medicating with alcohol to cope with their anxiety and other emotions, which is a maladaptive coping mechanism that can exacerbate their mental health issues.

**Research value**

This hypothesis could be scientifically valuable as it highlights the importance of addressing maladaptive coping mechanisms in treatment plans for individuals with anxiety and shame.


## Limitations

This project is an exploratory qualitative analysis tool and does not provide clinical recommendations or diagnostic assessments.
