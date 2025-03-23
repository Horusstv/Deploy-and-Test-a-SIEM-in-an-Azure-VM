## Creating and deploying Sentinel

Now what we need to do is add Microsoft Sentinel to our machine.

**What is Microsoft Sentinel**

Microsoft Sentinel is a cloud-native Security Information and Event Management (SIEM) and Security Orchestration, Automation, and Response (SOAR) solution that helps organizations collect, analyze, and respond to security threats across their entire digital estate.

- Type Sentinel at the top and select Microsoft Sentinel.

![Sen](https://imgur.com/zwWsj1U.png)

- Create a new workspace

![sen2](https://imgur.com/U4I3GWR.png)

- Add it to the same group of your VM and also the same region, in this case US east and then name your instance.

![sen3](https://imgur.com/7MVpfFk.png)

- When the validation has been completed you can finally click create, wait for the deplopyment of the instance.

![sen3](https://imgur.com/cIGYNeG.png)

![sen4](https://imgur.com/PT5vtqx.png)

- Once the deployment is complete click on go to resource and then select "Add Microsoft Sentinel to a workspace.

- Select the workspace you just created and click add at the bottom.

![Sen5](https://imgur.com/FCxEGWe.png)

![sen6](https://imgur.com/BdRy2Rj.png)

- When that is complete click on overview.

![sen7](https://imgur.com/7lm0KRT.png)

- Sentinel is ready by now buy it is still not connected to anything.

- To connect it click on Data connectors.

  ![sen8](https://imgur.com/du50hea.png)

- Then click on Content hub.

![sen9](https://imgur.com/EfVlRlA.png)

- Type Windows at the top and select Windows Security Events and then click install.

![sen10](https://imgur.com/WhZjJXU.png)

![sen11](https://imgur.com/cys92dL.png)

- As you can see it is now installed.

![sen12](https://imgur.com/GDFf53O.png)

- Go back to the data connectors page and select the "Windows Security Events Via AMA"

![sen13](https://imgur.com/3YOCf42.png)

- Select Open connectors page.

![sen14](https://imgur.com/KgOmKEK.png)

- Create a new data colletion rule.
- Chose the name you want for it.

![sen15](https://imgur.com/psHfniD.png)

![sen16](https://imgur.com/rB5X00K.png)

- In the resources page select your previously created VM

![sen17](https://imgur.com/FvAXxcQ.png)

- Click on collect all security events.

![sen18](https://imgur.com/P26jgZZ.png)

- Finally create the data collection rule.

![sen19](https://imgur.com/QVp7EKu.png)

- After all this go to Microsoft Sentinel logs and we are going to create a new rule.

![sen20](https://imgur.com/6EC87Au.png)

- Click on create new rule "Microsoft Sentinel Alert"

![sen21](https://imgur.com/GX01iJf.png)

- Set the name to any name, severity to anything you want and set the MITRE ATTACK to Innitial access.

![sen22](https://imgur.com/JVEXDGg.png)

- Click next and set the Rule query to SecurityEvent as in the picture below.

![sen23](https://imgur.com/E4zc33U.png)

![sen24](https://imgur.com/g8ZGtIV.png)

- After successfully created the rule go to your analytics page and you will be able to see the new rule created there.

![sen25](https://imgur.com/NNblLw0.png)

## Final Thoughts

After doing this excercise we were able to see the importance of a SIEM and also the importance of having good detection rules in place that allow you to see the information you need in real time in order to effectively defend an organization or a system from attackers.
