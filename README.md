# Business Process Modeling Project – Acting School (P54)

This repository contains the deliverables for the Business Process Modeling (BPM) course, part of the MSc in Data Science and Business Informatics at the University of Pisa (UniPi).

**Author:** Lorenzo Lattanzi<br>
**Academic Year:** 2025/2026

## Project Overview

The project models the interaction processes within an acting school involving students, teachers, and the school administration. It covers course selection, teacher assignment, lesson scheduling, lesson execution, payments, and course completion. The processes are represented using BPMN diagrams, transformed into Workflow Nets, and formally analyzed.

## Repository Structure

**BPMN/**
Contains BPMN models of the process:
- Full process model
- School, Student, and Teacher views

**WF NETS/**
Contains Petri net models (.pnml) derived from BPMN diagrams.

**Images and others/**
Contains:
- BPMN diagrams
- Petri net visualizations
- Coverability graphs
- Results of semantic analysis
- Other analysis outputs

## Tools Used

- Camunda Modeler
- WoPeD

## Analysis

The analysis is performed on three Workflow Nets: the Student process, the School process, and the full collaboration net.

**Individual processes (Student & School):**
- BPMN to Workflow Net transformation (via BPMN-to-Petri Net tool)
- Classification as **S-nets** (each transition has exactly one input and one output place)
- **Free-choice property** verification
- **S-component analysis** (single component covering the entire net)
- Boundedness, liveness, safeness, and **soundness** verification (via WoPeD)
- Coverability graph construction (coincides with reachability graph due to boundedness)

**Full collaboration net (manual construction):**
- Integration of Student and School Workflow Nets
- Analysis of **free-choice violations** 
- **PT/TP-handle analysis** 
- S-component analysis
- Boundedness, liveness, and **soundness** verification
