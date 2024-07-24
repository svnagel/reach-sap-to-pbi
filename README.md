# REACH SAP to PBI (Data-to-Value)

## Table of contents
* [Description](https://github.com/svnagel/sap-reach-pbi?tab=readme-ov-file#description)
* [Use Case Scenario](https://github.com/svnagel/sap-reach-pbi?tab=readme-ov-file#use-case-scenario)
* [Objectives](https://github.com/svnagel/sap-reach-pbi?tab=readme-ov-file#class-diagram)
* [Data Dictionary](https://github.com/svnagel/sap-reach-pbi?tab=readme-ov-file#class-diagram)
* [Class Diagram](https://github.com/svnagel/sap-reach-pbi?tab=readme-ov-file#class-diagram)
* [Prerequisites](https://github.com/svnagel/sap-reach-pbi?tab=readme-ov-file#prerequisites)
* [Sources](https://github.com/svnagel/sap-reach-pbi?tab=readme-ov-file#sources)

## Description
This project was inspired by a HAL thesis (Id: tel-03716180) in the context of the application of EU REACH regulation for French aeronautical equipment manufacturers. It addresses the notions of: data modelling, data pipeline and data visualisation.

## Use Case Scenario
REACH regulation in Europe has banned the use of hexavalent chromium (Chromium-6) compounds since September 21, 2017. The « Sermetel W » paint, currently used by our use case company « SAF » contains this chemical substance. Studies have suggested the paint « Maderbind CF » as a replacement for « Sermetel W ». Our company wishes to monitor the replacements of the « Sermetel W » painting lines. A regular meeting is organised with the environmental health and safety auditors (HSE Audit) to present progress KPIs.

## Objectives
The following KPI(s) will be monitored during HSE meetings:
* Percentage of REACH compliant components

## Data Dictionary
### Paint Table
| **Name**    	| **Type** 	| **Description**                          	| **Example**                      	|
|-------------	|----------	|------------------------------------------	|----------------------------------	|
| id          	| number   	| paint identifier                         	| 01, 02                           	|
| name        	| text     	| name of the painting                     	| Sermetel W, Maderbind CF         	|
| binder type 	| text     	| chemical components of the binder        	| phosphate-chrome, sol-gel        	|
| status      	| text     	| status regarding the replacement project 	| in use, to be replaced, replaced 	|

### Component Table


### Replacement Project Table

## Class Diagram
First, the class diagram will be simplified to build the complete data pipeline (from SAP to PBI). Later, it will be possible to extend the database to add more parameters.

## Prerequisites

## Sources
* [Data Analyst SAP course catalog](https://learning.sap.com/browse/roles/data-analyst?access=free&page=1)
* [SAP S/4HANA Cloud trial](https://www.sap.com/products/erp/s4hana/trial.html)
* [SAP BTP (Business Technology Platform) Data-to-Value Bootcamp](https://github.com/SAP-samples/btp-data-to-value-workshop)
* [REACH Regulation](https://environment.ec.europa.eu/topics/chemicals/reach-regulation_en)
* [HAL thesis (Id: tel-03716180)](https://theses.hal.science/tel-03716180v1/document)
