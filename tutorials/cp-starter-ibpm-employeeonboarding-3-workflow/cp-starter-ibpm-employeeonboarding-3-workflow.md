---
title: Set Up a Workflow With Extended Employee Onboarding
description: Set up the Employee Onboarding sample workflow application and integrate with business rules service.
auto_validation: true
time: 10
tags: [ tutorial>beginner, products>sap-web-ide]
primary_tag: products>sap-cloud-platform
---

## Details
### You will learn
  - How to set up a sample workflow application in SAP Web IDE

---

[ACCORDION-BEGIN [Step 1: ](Download a sample application)]

Download **cf-onboarding-sample.zip**  project from [GitHub](https://github.com/SAP-samples/cloud-workflow-samples/blob/master/cf-onboarding-sample/resources/cf-onboarding-sample.zip) in your local file system and extract the files.

!![Download Sample Workflow](downloadsample.png)

[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 2: ](Import sample application)]

1. Choose **SAP Business Application Studio**.

    !![Launch Studio](launchbas.png)

2. Click on the **Dev Space** to go into the workspace and from **File** menu choose **Open Workspace**

    >If the dev-space status is STOPPED then click on the run button to start the space
    !![Start Workspace](startspace.png)

    !![Open Workspace](openworkspace.png)

3. Drag and drop the extracted **cf-onboarding-sample** project in the dialog and click **Open**.

    !![Import Sample MTA 1](dragDropProject.png)

    !![Import Sample MTA 2](opensamplemta.png)

5. You will see that the sample **cf-onboarding-sample** project is imported into your workspace.

    ![Workflow Added](sampleworkflowadded.png)

    > This sample workflow has:

    > - **Business Rules** integrated into it. You can find the integration as part of service task with name `Determine Equipment`.

    > - **User Tasks** for confirmation of the equipment selected via business rules and for the approval of equipment. You can find these user tasks with the names `Confirm and Change Equipment` and `Approve Equipment` respectively.  The user interface associated with these user tasks have been built as SAPUI component and you can find these modules bundled under `confirmEquip` and `approveEquip` respectively in the same multi target application.



[DONE]
[ACCORDION-END]

[ACCORDION-BEGIN [Step 3: ](Build and deploy sample application)]

1. Right-click the **mta.yml** file inside the **cf-onboarding-sample** project, and choose the **Build MTA** option.

    ![Build mta File](build-wf-mta.png)


2. Once the build is completed successfully, right-click on the **`mta_archives` | `sample-onboarding.mta_0.0.1.mtar`** file and choose **Deploy MTA Archives**.

    ![Deploy Workflow](deployworkflow.png)

    >A successful deployment message will be shown in the terminal once the deployment has completed successfully.
    ![View Success Messages](success-message.png)

[VALIDATE_1]
[ACCORDION-END]



---
