***********************
Mobile FL Documentation
***********************

.. image:: https://travis-ci.org/readthedocs/sphinx_rtd_theme.svg?branch=master
   :target: https://travis-ci.org/readthedocs/sphinx_rtd_theme
   :alt: Build Status
.. image:: https://img.shields.io/pypi/l/sphinx_rtd_theme.svg
   :target: https://pypi.python.org/pypi/sphinx_rtd_theme/
   :alt: License
.. image:: https://readthedocs.org/projects/sphinx-rtd-theme/badge/?version=latest
  :target: http://sphinx-rtd-theme.readthedocs.io/en/latest/?badge=latest
  :alt: Documentation Status


The document for the ongoing project MFL (Mobile Federated Learning).

---------

Overview
========

The project targets to develop a framework for federated learning framework with mobile IoT devices.

Goal
----

The motivation is to ease the burden on the light weight IoT devices while providing iteratively
updated service models. To achieve the goal, the project targets at the "fog" nodes such
as smartphones to collect service data from the IoT devices for training and feedback updated models 
iteratively to improve the user experience.  

User Demands
------------

User require long battery life and good service experience. Since IoT devices by nature have limited power and computation capacities, 
efficient utilisation of computation capacity, communication capacity and storage capacity are all important to avoid too much battery consumption. 
As such, low frequency of model updates and low data volume of communication is critical. Meanwhile, the model 
updates require to satisfy user experience. 

Required Functionalities
------------------------

In the rest of the document, we classify the devices in the framework into three categories, e.g., UE (IoT device), 
trainer (the device that runs the training algorithm), and cloud (a remote data backup store).
Based on the user demands, the framework requires the following functionalities.


* UE:

  * Accurate sensor data.
  * Summarised measurement report with dedicated data abstraction.
  * Efficient and reliable communication with training device (trainer).
  * Efficient and robust database maintenance.

|
* Trainer:

  * Power-aware training trigger.
  * Fast and light weight reinforcement learning.
  * Efficient and reliable communication with the UE.
  * Efficient and robust abstractive model update report.
  * Efficient communication with the cloud.

| 
* Cloud:

  * Accurate and fast centralised training.
  * Anomaly detection.
  * Robust communications with the trainers.


