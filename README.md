RF_Tuning_Tool
==============

A Python program to facilitate GSM/WCDMA/LTE RF tuning and reduce manual operation.


Introduction
------------

RF tuning contains many manual routine operations, including device setup, 
callbox setup and record measurement result. These routines take lots of 
time and distract RF engineer from tuning itself.

This program contains three classes to wrap callbox and phone commands and 
integrated tuning tools in both command-line and GUI.


File Description
----------------

File name				Function
---------				--------
RF_Tuning_Tool_2.pyw	GUI WCDMA/LTE tuning tool
RF_Tuning_Tool.pyw		GUI WCDMA/LTE tuning tool (obsolete)
Agilent8960.py			Wrap of Agilent8960 GPIB commands
Anritsu8820C.py			Wrap of Anritsu8820C GPIB commands
QCOM.py					Wrap of Qualcomm QMSL library
tuning.py				Command-line WCDMA tuning tool
tuning_LTE.py			Command-line LTE tuning tool
WCDMA_attributes.py		Parameters including COM port, path loss, etc.
WCDMA.py				Link mode auto test tool for TxP/sensitivity


Supported Device
----------------

- Qualcomm based phone
- Callbox: Anritsu 8820C and Agilent 8960


Requirement
-----------

Hardware
- Qualcomm based device
- Callbox with GPIB (Agilent 8960/ Anritsu 8820C)
- GPIB (tested with NI USB-GPIB adapter)

Software
- Python (tested with 2.7.5, Win7)
- PyVisa (for callbox control)
- PySide (Python binding for QT)
- Qualcomm Library QMSL_MSVC10R (for phone control)
	:Qualcomm library is not free, you need to get it from Qualcomm directly.


Usage
-----

- Check parameters in WCDMA_attrigutes.py
- Execute RF_Tuning_Tool_2.pyw