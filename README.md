# Covid-19-detection-using-X-ray

## Background

In the context of a COVID-19 pandemic, we want to improve prognostic predictions to triage and manage patient care. Data is the first step to developing any diagnostic/prognostic tool. While there exist large public datasets of more typical chest X-rays from the NIH [Wang 2017], Spain [Bustos 2019], Stanford [Irvin 2019], MIT [Johnson 2019] and Indiana University [Demner-Fushman 2016], there is no collection of COVID-19 chest X-rays or CT scans designed to be used for computational analysis.

The 2019 novel coronavirus (COVID-19) presents several unique features Fang, 2020 and Ai 2020. While the diagnosis is confirmed using polymerase chain reaction (PCR), infected patients with pneumonia may present on chest X-ray and computed tomography (CT) images with a pattern that is only moderately characteristic for the human eye Ng, 2020. In late January, a Chinese team published a paper detailing the clinical and paraclinical features of COVID-19. They reported that patients present abnormalities in chest CT images with most having bilateral involvement Huang 2020. Bilateral multiple lobular and subsegmental areas of consolidation constitute the typical findings in chest CT images of intensive care unit (ICU) patients on admission Huang 2020. In comparison, non-ICU patients show bilateral ground-glass opacity and subsegmental areas of consolidation in their chest CT images Huang 2020. In these patients, later chest CT images display bilateral ground-glass opacity with resolved consolidation Huang 2020.

## Goal

Our goal is to use these images to develop AI based approaches to predict and understand the infection. Our group will work to release these models using our open source Chester AI Radiology Assistant platform.

The tasks are as follows using chest X-ray or CT (preference for X-ray) as input to predict these tasks:

1 Healthy vs Pneumonia (prototype already implemented Chester with ~74% AUC, validation study here)

2 Bacterial vs Viral vs COVID-19 Pneumonia (not relevant enough for the clinical workflows)

3 Prognostic/severity predictions (survival, need for intubation, need for supplemental oxygen)

## Expected outcomes

Tool impact: This would give physicians an edge and allow them to act with more confidence while they wait for the analysis of a radiologist by having a digital second opinion confirm their assessment of a patient's condition. Also, these tools can provide quantitative scores to consider and use in studies.

Data impact: Image data linked with clinically relevant attributes in a public dataset that is designed for ML will enable parallel development of these tools and rapid local validation of models. Furthermore, this data can be used for completely different tasks.

## Required Librarries
1 import streamlit as st

2 import os

3 from PIL import Image

4 from tensorflow.keras.preprocessing import image

5 import numpy as np

6 from tensorflow.keras.models import load_model

## Web App Demo

## Homepage
![1](https://user-images.githubusercontent.com/84785447/146323474-b39aef71-b3bb-4b6e-b002-a1bf8226faad.png)

## Uploading the covid-19 Positive X-ray image
![1](https://user-images.githubusercontent.com/84785447/146323773-0da1ad77-26c3-40c8-a896-199ad6e13a94.png)

## Uploading the normal patient X-ray(covid-19 negative)
![1](https://user-images.githubusercontent.com/84785447/146324069-e2b6e727-e3f1-428e-8e9f-a746c2168053.png)

## To run the app follow the below commands:
1 Please install all the required libraries
2 streamlit run app.py in cmd prompt



