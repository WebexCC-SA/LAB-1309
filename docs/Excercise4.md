# Excercise 4 - Explore Webex AI Assistant Feature 

Please use the following credentials to connect to Control Hub and configure Webex Contact Center:

| <!-- -->         | <!-- -->         |
| ---------------- | ---------------- |
| `Control Hub URL`            | <a href="https://admin.webex.com" target="_blank">https://admin.webex.com</a> |
| `Username`       | wxccemealabs+admin**ID**@gmail.com  _(where **ID** is your assigned pod number; this ID will be provided by your proctor)_ |
| `Password`       | ciscoliveAMER25! |

## **Objective**

This lab's objective is to provide participants with a basic understanding of the AI Assistant feature in the Webex Contact Center and demonstrate how it enhances the live agent experience.

Building on previous labs that showcased how Webex AI Agents assist customers with inquiries and actionable tasks, this lab will focus on the AI Assistant's role when a customer's call is escalated to a live agent. You will explore, configure, and test the following AI capabilities:

- **AI Agent Transfer Summaries** : See how the AI provides a summary of the conversation when a virtual agent transfers a call to a human agent, giving the agent full context.

- **Call Drop Summaries** : Learn how the AI generates a summary for a new agent if a customer's call is disconnected and they call back, ensuring they don't have to repeat themselves.

- **Real-time Transcriptions** : Experience how this feature provides a live, real-time transcription of the conversation for agents , improving clarity and customer satisfaction.

## Section 1: 

- To achieve this objective, we must first ensure that the all the summary and transcripts feature is enabled for the tenant. 

- To check this: Log in to <a href="https://admin.webex.com" target="_blank">https://admin.webex.com</a> with the provided credentials.

- In Control Hub, under Services, click on Contact Center. Then, under Contact Center navigation pane on the left side, scroll down to DESKTOP EXPEREINCE section and click on Cisco AI Assistant.

	![Nav](./assets/Excercise1_1.1.png){ width="500" }

- Ensure that the "Call Drop Summary" toggle is enabled.

	![Nav](./assets/Excercise1_1.2.png){ width="500" }

- The next step is to configure the AI Assistant widget for agent use. 

- To accomplish this, the agent's desktop layout must include the "ai-assistant" JSON string in the Agent Advanced Header section

- You can review this in Control Hub by navigating to "Desktop Layouts" within the "Desktop Experience" section of the Contact Center services.

	![Nav](./assets/Excercise1_2.png){ width="500" }

- Search and Open the layout CL_2025_AI_CallDropSummary and download the file CL_2025_AI_CallDropSummary.json.

  	![Nav](./assets/Excercise1_3.png){ width="600" }
  
- Review the file in a text editor. In the Agent Advanced Header section, you should see the verbiage highlighted in this screenshot

	![Nav](./assets/Excercise1_4.png){ width="400" }

- To simplify the process, the desktop layout has already been mapped to the agents who will test this feature
  
- Now, log in to the Agent Desktop using the provided credentials.
  	- URL: <a href="https://desktop.wxcc-us1.cisco.com/" target="_blank">https://desktop.wxcc-us1.cisco.com/</a>
  	- Username: `Contact the lab proctor if information is unavailable.`  
  	- Password: `Contact the lab proctor if information is unavailable.`
	
- Please select **Extension** as the telephony option. Use the extension provided by the proctor, and set the Team as **MS Dynamic**

	![Nav](./assets/Excercise1_5.png){ width="400" }

- This will load the layout as configured above.

- You will notice the AI Assistant and its capabilities loaded.

	![Nav](./assets/Excercise1_1.png){ width="600" }

- Ensure the agent is set to the "Available" state.

- Place a call from your cell phone to the Dialed Number "+14698578314".

- The call will be auto-accepted, and you will hear a recorded message explaining the call drop summary feature.

!!! Note 
	If you encounter any issues reaching the US number, please contact the instructor. They will be able to make a call on your behalf and demonstrate the Call Drop Summary feature

- Keep the call active with ongoing conversation for approximately 40 seconds, then hang up from your cell phone. 

- Make another call to the same number and observe the experience. You should see a notification that "Cisco AI Assistant: Summary ready."

  	![Nav](./assets/Excercise1_6.png){ width="500" }
  
- Click on the "Cisco AI Assistant" option at the top of the screen.

- This will display a summary of the last dropped call
  
  	![Nav](./assets/Excercise1_7.png){ width="500" }

# Results
Congratulations, you are now familiar with WxCC Call Drop Summaries feature powered by Cisco AI Assistant!
