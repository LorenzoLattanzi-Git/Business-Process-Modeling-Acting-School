# Business Process Modeling Project – Acting School (P54)

This repository contains the deliverables for the Business Process Modeling (BPM) course, part of the MSc in Data Science and Business Informatics at the University of Pisa (UniPi).

Author: Lorenzo Lattanzi
Academic Year: 2025/2026

## Project Overview

The project models the interaction processes within an acting school involving students, teachers, and the school administration. It covers course selection, teacher assignment, lesson scheduling, lesson execution, payments, and course completion. The processes are represented using BPMN diagrams, transformed into Workflow Nets, and formally analyzed.

## Repository Structure

BPMN/
Contains BPMN models of the process:
- Full process model
- School, Student, and Teacher views

WF NETS/
Contains Petri net models (.pnml) derived from BPMN diagrams.

Images and others/
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

The project includes:
- BPMN to Workflow Net transformation
- Structural analysis of Petri nets
- Soundness verification
- Analysis of free-choice, safeness, and boundedness
- Reachability graph estimation
- Discussion of relaxed and weak soundness when applicable