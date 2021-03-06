# [ARM Template Editor for Azure Sentinel Analytics Rules](https://github.com/nathanjalston/Azure_Sentinel_Hackathon_2021)
**Azure Resource Manager (ARM) Template Editor for Bulk Modification of Azure Sentinel Analytics Rules.**
* Submitted as part of [AzureSentinel Hackathon 2021 - MSSA-PSCA1](https://devpost.com/software/mssa-psca1)
* [MSSA-PSCA1 GitHub](https://github.com/MSSAPSCA1/Azure_Sentinel)
* [Demo Video](https://youtu.be/f0YaSqNwJCM)
___

## [ARM Template Editor](https://github.com/nathanjalston/Azure_Sentinel_Hackathon_2021/blob/main/AZ_Sentinel_Analytics_Rules_Editor.py)

Python script to modify properties of Azure Resource Manager (ARM) templates for bulk modification of Azure Sentinel Analytics Rules. Currently capable of modifying Rule Status (Enabled/Disabled), Rule Frequency, and Rule Period for any number of Azure Sentinel Analytics Rules contained within any number of ARM template files.

### Notes from Azure Sentinel:
* The Rule Frequency (queryFrequency) value must be between 5 minutes and 14 days.
* The Rule Period (queryPeriod) value must be between 5 minutes and 14 days.
* The Rule Frequency must be less than, or equal to, the Rule Period.
* When the Rule Period is greater than, or equal to, 2 days, the Rule Frequency must be greater than, or equal to, 1 hour.

### Operating Instructions:

**Prerequisites:**
* Python 3 Interpreter. (see Microsoft Docs/ Microsoft Learn for [validation](https://docs.microsoft.com/en-us/learn/modules/python-install-vscode/2-python-programming-language?pivots=windows) or [install](https://docs.microsoft.com/en-us/learn/modules/python-install-vscode/3-exercise-install-python3?pivots=windows) instructions)
* Path to ARM template/ ARM template file address in directory.

**Procedure:**
1.  Open the AZ_Sentinel_Analytics_Rules_Editor.py using a Python 3 Interpreter.
2.  Enter the path to the ARM template file(s) (i.e. C:\fakepath\AZ_Sentinel\Vectra_Detect_AZ_Sentinel_Analytics_Rules.json), or drag-and-drop each file, one at a time. Separate each file using a comma (,).
3.  Select options by entering the number associated with the option.
4.  Enter requested data based on constraints specified in the program and in the Notes from Azure Sentinel.
5.  Once the process is completed, a new file or new files will be created at the same address as the original file(s) with the user-specified prefix appended as the prefix of the filename(s). You will now have two files for each ARM template, the orignal and the new file.
___

## [ARM Templates for Default Analytics Rules](https://github.com/nathanjalston/Azure_Sentinel_Hackathon_2021/tree/main/Default_AZ_Sentinel_Rule_Templates)

ARM templates for specific sets of default Azure Sentinel Analytics Rules.
* Rule Frequency = Default
* Rule Period = Default

### Analytics Rules:
*  [0-A](https://github.com/nathanjalston/Azure_Sentinel_Hackathon_2021/blob/main/Default_AZ_Sentinel_Rule_Templates/0-A_Azure_Sentinel_Scheduled_Analytics_Rules.json)
*  [A-F](https://github.com/nathanjalston/Azure_Sentinel_Hackathon_2021/blob/main/Default_AZ_Sentinel_Rule_Templates/A-F_Azure_Sentinel_Scheduled_Analytics_Rules.json)
*  [F-N](https://github.com/nathanjalston/Azure_Sentinel_Hackathon_2021/blob/main/Default_AZ_Sentinel_Rule_Templates/F-N_Azure_Sentinel_Scheduled_Analytics_Rules.json)
*  [N-S](https://github.com/nathanjalston/Azure_Sentinel_Hackathon_2021/blob/main/Default_AZ_Sentinel_Rule_Templates/N-S_Azure_Sentinel_Scheduled_Analytics_Rules.json)
*  [S-Z](https://github.com/nathanjalston/Azure_Sentinel_Hackathon_2021/blob/main/Default_AZ_Sentinel_Rule_Templates/S-Z_Azure_Sentinel_Scheduled_Analytics_Rules.json)
