# Construction Equipment Task Monitoring MCQ Dataset

This repository contains the Multiple Choice Question (MCQ) dataset introduced in the research article: **"Zero-shot framework for construction equipment task monitoring"** (Jeoung, Jung, & Hong, 2025). 

The dataset is specifically designed to evaluate the capability of Multimodal Large Language Models (MLLMs) to understand, reason, and monitor construction equipment tasks through video frame analysis.

## Dataset Overview

The dataset was curated from YouTube videos featuring various construction equipment and complex site operations. 

* **Source Material:** 52 YouTube videos
* **Video Clips:** 216 clips (extracted at intervals under 30 seconds; average length ~28.5s)
* **Total Questions:** 1,207 multiple-choice questions (4 options each)
* **Questions per Clip:** Average of 5.59 (Range: 3 to 9)

### Question Focus Breakdown
* **Activities (65.6%):** 782 questions covering tasks like digging, loading, unloading, lifting, carrying, pushing, leveling, breaking, demolition, and idling.
* **Equipment (17.6%):** 213 questions focused directly on the machinery.
* **General Context (16.7%):** 202 questions covering counts, colors, and the surrounding environment.

---

## Question Types

To comprehensively evaluate MLLMs, the questions are divided into three distinct reasoning categories:

### 1. Spatial Inference (263 questions)
Evaluates the understanding of position, arrangement, and spatial relationships between equipment and other objects (e.g., soils, workers, other equipment). These can typically be answered from a single frame.

**Example:** What is the position of the excavator in relation to the dump truck during the loading process?
(A) Beside the dump truck
(B) Behind the dump truck
(C) In front of the dump truck
(D) Above the dump truck

### 2. Task Inference (331 questions)
Requires reasoning about the activity, task, or purpose of the construction equipment based on the sequence of input frames.

**Example:** What activity does the bulldozer perform after the truck is loaded?
(A) Starts digging
(B) Pushes material
(C) Moves to another location
(D) Loads more material

### 3. Temporal Event (613 questions)
Tests the understanding of timing, sequence, or specific frames where a particular event or action occurs within the operational timeline.

**Example:** In which frame does the excavator idle with no movement?
(A) Frame 00:01–00:10
(B) Frame 00:11–00:20
(C) Frame 00:21–00:30
(D) Excavator is actively working in all frames

---

## Purpose and Usage

This dataset was originally used to benchmark proprietary MLLMs (such as GPT-4o mini and Gemini 1.5 Flash) on their ability to monitor construction sites without domain-specific training data (Zero-Shot Learning). It helps clarify the scope and depth of information MLLMs can extract from video frames regarding equipment location, operational states, and workflow sequences.

---

## Citation

If you use this dataset in your research or project, please cite the original article:

> Jeoung, J., Jung, S., & Hong, T. (2025). Zero-shot framework for construction equipment task monitoring. *Computer-Aided Civil and Infrastructure Engineering*. https://doi.org/10.1111/mice.13506
