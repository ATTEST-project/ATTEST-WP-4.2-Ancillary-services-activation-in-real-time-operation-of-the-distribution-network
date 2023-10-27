## Description
This tool aims to compute in real-time the optimal flexibility activation for ancillary services procurement by DSO.

## How to run
The tool is run using batch script *run_script.bat*

It requires installation of:
* Julia with packages:
	* PowerModels
	* DataFrames
	* XLSX
* AMPL with Ipopt solver

## Inputs
Inputs are specified in *run_script.bat* script in order:
* MATPOWER network file
* PV production profile
* flexibity devices expected states (output of task 4.1)
* state estimation (output of task 4.3)
* transmission activation from task 4.5
* current time period
* flexibility devices characteristics file (EV-PV file)

## Outputs
Distribution decisions (_dist_decisions.xlsx_) which includes for each device up and down activation. 
