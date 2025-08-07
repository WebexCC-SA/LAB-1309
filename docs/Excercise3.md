# Lab 3 - Voice flow configuration for AI Agent


Please use the following credentials to connect to Control Hub and configure Webex Contact Center:

| <!-- -->         | <!-- -->         |
| ---------------- | ---------------- |
| `Control Hub URL`            | <a href="https://admin.webex.com" target="_blank">https://admin.webex.com</a> |
| `Username`       | wxccemealabs+admin**ID**@gmail.com  _(where **ID** is your assigned pod number; this ID will be provided by your proctor)_ |
| `Password`       | ciscoliveAMER25! |


**Objective**

This lab exercise aims to guide participants in creating and configuring a voice flow for an Autonomous Webex AI Agent that was set up in a previous exercise. Participants will then interact with the AI Agent via a phone call to test the voice flow. 

This exercise will also provide an opportunity to experience the AI Assistant feature of the contact center by highlighting the virtual agent's conversation summary when the call is escalated to a live agent

## **Section 1 - Voice flow configuration**

- Navigate to the Control Hub and log in using the credentials provided above.
- After logging in to the Control Hub, navigate to the **'Flows'** menu on the-left hand side.
- Click **'Manage Flows'** and select **'Create Flows'**.

![Nav](./assets/t4s1p2.png){ width="1000" }

- When prompted to **'Choose a method'**, select **'Flow Templates'**.

![Nav](./assets/t4s1p3.png){ width="800" }

- Choose **'AI Agent Autonomous (Package Tracking)'**, click **'Next'**, provide a flow name (e.g., '_ai_agent_autonomous_andy_'), and click **'Create Flow'**.

![Nav](./assets/t4s1p4.png){ width="500" }
![Nav](./assets/t4s1p5.png){ width="500" }

- Once the flow loads, click on the **'VirtualAgentV2'** node and select the Webex AI Agent (created in **Task 1**) under **'Virtual Agent'**.

![Nav](./assets/t4s1p6.png){ width="1000" }

- Click on the **'QueueContact'** node and select **'AIQueueN'** (_where **'N'** is your lab user number, e.g., labuser**7**@wxccciscolive.wbx.ai_).

![Nav](./assets/t4s1p7.png){ width="1000" }

- Click on an empty space in the flow, then on the right-hand side, navigate to **'Global Variables'**. Click on **'Global_VoiceName'**, select edit option (pencil icon), use 'en-US-Jess' for **'Default Value'**, and click **'Save'**.

![Nav](./assets/t4s1p8.png){ width="1000" }

- Turn Flow Validation **'On'** by clicking the **'Validation'** button at the bottom of the page to publish the flow. Once validation is complete, click **'Publish Flow'** and then **'Publish Flow'** again in the next dialog box (**Latest** version label is selected automatically).

![Nav](./assets/t4s1p9.png){ width="400" }

- Navigate to **'Channels'** menu in the Webex Contact Center configuration.
- Open **'AIChannelN'** (_where **'N'** is your lab user number, e.g., labuser**7**@wxccciscolive.wbx.ai_), associate your created flow under **'Routing Flow'** (note down the **'Support Number'** associated with this channel - it will be needed later in this lab for testing), and click **'Save'**.

![Nav](./assets/t4s1p10.png){ width="600" }
![Nav](./assets/t4s1p11.png){ width="1000" }


## **Section 2 - Verifying Voice Flow, Agent Handover and AI Assistant Summary**

- Log in to the Webex Contact Center Agent Desktop:
	- For the phone number, select **'Extension'** and enter the extension in the format 100**N** (where **'N'** is your lab user number, e.g., _labuser**7**@wxccciscolive.wbx.ai_)':
	- For the team use **AITeamN** (where **'N'** is your lab user number, e.g., _labuser**7**@wxccciscolive.wbx.ai_)'.

![Nav](./assets/t4s2p1.png){ width="400" }

- Call the channel number (from the steps above), interact with the Webex AI Agent, and request a transfer to a human at the end.
- Switch to the **'Available'** state on the Webex Contact Center Agent Desktop and accept the call.
- Observe the AI Assistant summary of your conversation with the agent.

![Nav](./assets/t4s2p2.png){ width="600" }
![Nav](./assets/t4s2p3.png){ width="1200" }

- End the call.
- Congratulations! You have completed this task and the lab!
