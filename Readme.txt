README
======

COMP 6910 — Winter 2026
Performance vs. Cost Efficiency in Kubernetes-Based Microservice Autoscaling
Memorial University of Newfoundland

-----------------------------------------------------------------------
Group-3
-----------------------------------------------------------------------
Afiya Farjana       — Student ID: 202486149
Jannatul Ferdous    — Student ID: 202487105
Rumnaz Khan         — Student ID: 202487843

Instructor: Dr. Kaiyang Liu

-----------------------------------------------------------------------
SUBMISSION CONTENTS
-----------------------------------------------------------------------
Cloud_Project_report.pdf            Final project report (LNCS format)
Cloud_Computing_Presentation.pptx   Slides delivered April 7, 2026
README.md                           This file

Data analysis code/
    Minikube_data_analysis.ipynb    Analysis notebook — Minikube
    GKE_data_analysis.ipynb         Analysis notebook — GKE

microservices-demo/hpa-configs/
    frontend-hpa.yaml               HPA configuration files used
    cart-hpa.yaml                   in all 36 experiments
    checkout-hpa.yaml
    recommendation-hpa.yaml

microservices-demo/raw-data/
    minikube/   18 experiment folders with Locust HTML reports
    gke/        18 experiment folders with Locust HTML reports
    HPA_single.txt          Minikube single-service HPA watch logs
    HPA.txt                 Minikube multi-service HPA watch logs
    HPA_Single_gke.txt      GKE single-service HPA watch logs
    HPA_multi_gke.txt       GKE multi-service HPA watch logs

Processed data/
    comp6910_graphs_minikube/   Minikube experiment graphs
    comp6910_graphs_gke/        GKE experiment graphs
    comp6910_graphs_comparison/ Minikube vs GKE comparison graphs

-----------------------------------------------------------------------
EXPERIMENTS
-----------------------------------------------------------------------
36 total (18 Minikube + 18 GKE)
Thresholds : 50%, 70%, 85% CPU utilisation
User loads : 100, 300, 500 concurrent users
Scopes     : Single-service and Multi-service HPA
Tool       : Locust 2.43

-----------------------------------------------------------------------
ANALYSIS NOTEBOOKS
-----------------------------------------------------------------------
Notebooks run on Google Colab.
Upload raw-data contents to Google Drive under MyDrive/comp6910/
then open notebooks in Colab and run all cells.