# In this exercise we will be connecting an AWS Lambda to an Amazon SQS service
---

We will achieve this by doing the following tasks:
- Make an SQS instance
- Make a Lambda instance
- Add code to Lambda
- Provide SQS access to Lambda service
- Configure the SQS to send message to Lambda service

Part 1: Make an SQS instance

1. In the top search bar, search for **SQS** and select **"Simple Queue Service"**.
2. The Simple Queue Service blade will open up where you have to click the **Create queue** button.
3. On the following page you will be asked to provide a unique queue name, leave rest options as it is and proceed to click **Create queue** at the very bottom.

![create SQS](./images/createQueue.png)

Observe the highlighted ARN in the image below, copy it and store it some place safe.

> Headsup: Access privilege is required for SQS to let it access Lambda, so we have copied the ARN which will provide access to SQS to send messages to Lambda 

![ARN](./images/copyARN.png)


Part 2: Make a Lambda instance

1. In the top search bar, search for **Lambda** and select **"Lambda"**.
2. The Lambda blade will open up where you have to click the **Create function** button.
3. On the following page, these options are important:
   - Select Author from scratch.
   - Give a unique function name.
   - I have selected Python 3.9 as the runtime for the function
   - Scroll down to the bottom and click on **Create function**.

![create Lambda function](./images/createLambda.png)

