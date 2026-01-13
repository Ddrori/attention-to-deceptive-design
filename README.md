# attention-to-deceptive-design
Analysis code and data for two experiments testing educational and visual‑cue interventions on user attention and consent in deceptive cookie banner designs.


Attention to Deceptive Design: Analysis of User Attention and Consent Behavior

This repository contains the analysis code and data for two experimental studies investigating how users attend to and respond to deceptive design patterns in cookie consent banners. 
The research evaluates the effectiveness of two interventions: educational videos on deceptive design patterns and real‑time visual cues, in helping users recognize and resist manipulative interface designs.
All analyses were conducted in Python using Jupyter notebooks.
Eye‑tracking data for both experiments were collected using a Tobii Fusion Pro (120 Hz) eye‑tracker.
The analyses includes behavioral consent decisions with eye‑tracking metrics and use Generalized Linear Mixed Models (GLMMs) to examine how deceptive patterns influence cognitive load, attention allocation, and user autonomy.


Research Overview
Deceptive Pattern: Interface Interference

Both experiments focus on cookie consent banners that use unequal paths, a deceptive design pattern where the “Accept All” option is visually emphasized while alternatives like “Reject All” or “Settings” are less prominent. 
This pattern is common, and can influence user decisions by increasing cognitive load and reducing the visibility of privacy‑protective choices.


Experiment 1: Educational Intervention

Participants (n = 39) were randomly assigned to watch either: an educational video explaining deceptive patterns, how they operate, and their potential negative consequences, or a neutral control video about online search strategies.
After the video, participants completed realistic search tasks across 20 websites. Each website began with a cookie banner (deceptive vs. non‑deceptive).
Eye‑tracking captured: fixation durations on Areas of Interest (AOIs), fixation counts on the cookie consent banner, decision times, gaze allocation across interface elements.
At the end of the study, participants completed a Qualtrics questionnaire.
GLMMs were used to analyze how education influenced attention and consent decisions.

The Experiment 1 Notebook, experiment1_GLMM.ipynd ,includes: GLMM models for acceptance decisions, GLMM models for eye‑tracking features (fixation duration, fixation count, decision time, AOI‑based attention).


Experiment 2: Visual Cue Intervention

In this study, participants viewed cookie banners framed with color‑coded borders indicating whether the design was manipulative or not. These subtle cues were designed to raise awareness.
Participants (n = 19) completed realistic search tasks across 20 websites with eye-tracking. Each website began with a cookie banner (deceptive vs. non‑deceptive).
Eye‑tracking captured: fixation durations on Areas of Interest (AOIs), fixation counts on the cookie consent banner, decision times, gaze allocation across interface elements.
At the end of the study, participants completed a Qualtrics questionnaire.
GLMMs were used to analyze how visual cues affected attention and consent decisions.

The Experiment 2 Notebook, experiment2_GLMM.ipynd, includes: GLMM models for acceptance decisions, GLMM models for eye‑tracking features (fixation duration, fixation count, decision time, AOI‑based attention).


Key Findings

Deceptive designs increased cognitive load, reflected in longer fixations, more fixations, and longer decision times.
Education increased visual scrutiny (more attention to less prominent options) but did not significantly reduce acceptance rates.
Visual cues significantly reduced acceptance of deceptive designs compare to non-deceptive designs and increased attention to interface elements.
Eye‑tracking metrics strongly predicted consent behavior, highlighting the role of attention in resisting manipulation.

These findings contribute to research on deceptive design by showing how interventions can support user autonomy through awareness and attention‑based mechanisms.


Not Included in This Repository

The following materials are intentionally excluded:
Qualtrics questionnaire
Questionnaire responses
Predictive modeling notebook (eye‑tracking → consent prediction)
Raw eye‑tracking files
Additional exploratory models and intermediate data‑processing steps developed during the research
Only the finalized GLMM analyses and cleaned datasets used in the thesis are included.





