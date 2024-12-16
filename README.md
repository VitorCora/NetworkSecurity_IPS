# NetworkSecurity_IPS

## Creating the Cloud One Account

Go to https://cloudone.trendmicro.com/

And click on Get Started for free

<img width="787" alt="image" src="https://github.com/user-attachments/assets/315deefe-4f68-4cd3-97dc-eb61619f7953" />

Fill the form and create your Account

The user utilized to create the Cloud One account will be the "owner" of the Cloud One Account

* We recommend you to use a group mail for this step.

* After the account is created, we recommend you to create one account per user that needs to have access to Cloud One

* You may create as many user may be needed

<img width="348" alt="image" src="https://github.com/user-attachments/assets/c0f9ef5b-67f2-4f6d-bc60-f291a352b381" />

## Integrating Cloud One with your AWS Accounts

Log into Cloud One

Scroll all the way down

Look for the **Integrations**

<img width="542" alt="image" src="https://github.com/user-attachments/assets/1f6795ff-5041-426a-b009-ae10789c00e6" />

On the **Integrations** Page

Look for **Cloud Accounts**

Under Cloud Accounts,
 Click on  **+ New**

<img width="675" alt="image" src="https://github.com/user-attachments/assets/d0e93c2c-7e41-4c80-bdea-b68de8a739df" />

A pop-up will appear

Under **Step 1. Launch Cloud Formation Template**

  Select the most appropriate region for the creation of the stack
  
  We recommend you chose the region where you regularly deploy your own stacks
  
  On the 3rd item, expand **View Configuration**

  <img width="415" alt="image" src="https://github.com/user-attachments/assets/0448ef61-f9e9-4f6c-a68d-fa04d2d36f7b" />
  
  **Cloud Sentry** will appear as **On**, click twice on it until it turns into a **gray toggle**.
    * On means, resources will be deployed, but will be deactivated
  
  **Network Security** with Hosted Infrastructure will appear as a **gray toggle**, click on it once to turn it unto a **blue toggle**.
    * Gray toggle means feature is deactivated
    * Blue toggle means feature is activated
  
  <img width="382" alt="image" src="https://github.com/user-attachments/assets/c069631d-a57f-4ff8-b9f3-b85d252b25e9" />

Make sure that you are connected to the AWS Account that you will be deploying the **Network Security IPS** to.

Click on **Launch Stack**

In the case that you don't have access to the AWS Account that the Network Security will be deployed, click on **Download Template**

To deploy this template you will need the following information:
  - Trend Cloud One region: **us-1**
  - Trend Cloud One id:
  - Trend Cloud One OIDC Provider URL: cloudaccounts.**us-1**.cloudone.trendmicro.com

  *If your region is different from us-1, just change the boldened area with your Cloud One region

  You may found your Cloud One ID on the top right corner of your Cloud One tenant.

  <img width="858" alt="image" src="https://github.com/user-attachments/assets/62f890f6-ca4b-4de5-a050-245fe36908ce" />

  
After the Stack deployment is done

Go to Cloudformation

Stacks

Look for Cloud-One-Cloud-Account- Management

Under Outputs

Copy the CloudOneRoleArn

<img width="577" alt="image" src="https://github.com/user-attachments/assets/4cde2aa4-5ac5-4cfd-8685-d030a37c6baf" />

Go back to **Cloud One**

On the **Cloud Accounts** Page

On the pop-up

Got to Step 2. Copy stack output,

paste the **ARN**

Step 3, is optional

Trend recommends you to add na **Alias** to the account

This alias should be a name easily understandable to you and your team

<img width="398" alt="image" src="https://github.com/user-attachments/assets/e42a7144-6f93-411d-94c1-0fd2024e523f" />

Click on **Connect **

If you Cloud One looks something like the following you are good to go

<img width="934" alt="image" src="https://github.com/user-attachments/assets/3f16c132-cb57-49aa-b5e7-fc61f40914ff" />






