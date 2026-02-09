# COIS — Data Architecture

## 1. Objective
Design a simple, reproducible data pipeline for breast cancer survival research.

## 2. Architecture Overview
Source → Bronze → Silver → Gold → Analytics (outside DW)

## 3. Layers
- Source: SEER raw files
- Bronze: Parsed, typed raw tables
- Silver: Cleaned, validated tables
- Gold: Analysis-ready tables (one row per patient)
- Analytics: Survival analysis (KM, cohorts)

## 4. Core Entities
- Patient
- Diagnosis
- Treatment
- Outcome

## 5. Data Flow Rules
- One-way flow only
- No transforms in Source
- Validation required before Silver
- Gold is read-only for analytics

## 6. Non-Goals
- No BI dashboards
- No real-time processing
- No ML prediction services

## 7. Risks & Mitigation
- Data gaps → strict inclusion rules
- Complexity → minimal fields (v1)
