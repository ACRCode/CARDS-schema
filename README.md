# ACR Assist: Schema Definition

## Introduction

Radiology practice contains a large number of guidelines and algorithms for workup of specific clinical scenarios and findings. In order for these to be delivered within the context of a radiologist’s point-of-care (such as a PACS workstation or a voice recognition/report generation system), guidelines need to be specified in a structured format. The format developed and documented here serves as the interface between the creators of radiology reporting guidelines and the vendors of radiology reporting tools.

## Framework Schema

The schema is defined in [CARDS_Schema_2.0.rnc](https://github.com/acrscm/acr-assist-decision-support-schema/blob/master/CARDS_Schema_2.0.rnc) using the RelaxNG Compact format ([specification](http://relaxng.org/compact-20021121.html); [tutorial](http://relaxng.org/compact-tutorial-20030326.html)).

Briefly, the schema lays out the structure of guideline:
- **Metadata** section contains descriptive information about the guideline
- **Data Elements** section defines the various pieces of data used to characterize the clinical scenario and drive guidance and any logic
- **Rules** section defines the logic which can be run based on the input data elements to specify a guided output
- **End Points** section defines the actions to be taken based on the output of running the defined rules on the inputs given for a case.

For a more general overview of the schema, a white paper overview is in press at [JACR](http://jacr.org) and will soon be available online.

## Sample Guideline

A sample guideline is available at [Sample\Hello_Assist\Hello_Assist.xml](https://github.com/acrscm/acr-assist-decision-support-schema/blob/master/Sample/Hello_Assist/Hello_Assist.xml).

## See Also

- [ACR Assist home page](https://www.acr.org/Practice-Management-Quality-Informatics/Informatics/Structured-Content)
- [Reference implementation for rendering and executing ACR Assist modules](https://github.com/acrscm/acr_assist_simulator_control)
- [Try the simulator](https://assist.acr.org/simulator/)


