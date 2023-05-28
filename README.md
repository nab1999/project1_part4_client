# Part 4: Setting up CI/CD Pipelines
## 1.0 Creating GitHub repository (containing client application & workflow files) for part 4 of the project1:

![image](https://github.com/nab1999/project1_part4_client/assets/126570628/69180f71-dd3e-43cc-8d97-8e0d2cdb73f5)

## 1.1 Creating “Client-CI.yml” file & its contents for GitHub actions:

![image](https://github.com/nab1999/project1_part4_client/assets/126570628/1587151d-a40b-4fb0-b826-ee5263b90aab)

## 1.2 Creating Actions secrets:

![image](https://github.com/nab1999/project1_part4_client/assets/126570628/1e661406-f2ea-424e-8624-129cccf2f792)

## 1.3 Pushing changes (committing) to run the GitHub workflow (Client-CI):

![image](https://github.com/nab1999/project1_part4_client/assets/126570628/64cc5192-6758-47a3-8fbb-66afb9008ab9)

The “build” job basically builds the Docker image for client and then pushes it to the Docker Hub repository called “nab99/client-repo”.

### 1.3.1 Latest image pushed successfully to Docker Hub repository via GitHub actions:

![image](https://github.com/nab1999/project1_part4_client/assets/126570628/16ff1a83-b709-46f3-9fa1-628df840c3cf)

## 1.4 Creating “Client-CD.yml” file & its contents for GitHub actions:

![image](https://github.com/nab1999/project1_part4_client/assets/126570628/5f4f3f5e-8da6-442d-8898-47b89843d7ee)

This CD workflow will update the Docker Compose file, pull the new image, and deploy the updated services. Then the Slack notifications will be sent to the specified webhook URL to keep us informed about the deployments.

## 1.5 Configuring Slack webhook for deployment notifications:

![image](https://github.com/nab1999/project1_part4_client/assets/126570628/9a2d8503-1e28-4dcb-9925-37d6e4f2bb7f)

## 1.6 Creating Actions secret for Slack Webhook URL:

![image](https://github.com/nab1999/project1_part4_client/assets/126570628/4d617d3e-ab8f-4e42-bb5a-2cd479b1a7dd)

## 1.7 Pushing changes (committing) to run the GitHub workflow (Client-CD):

![image](https://github.com/nab1999/project1_part4_client/assets/126570628/f0dbb2a6-18c1-42cf-b302-a3644960bf03)

## 1.8 Slack notifications successfully received:

![image](https://github.com/nab1999/project1_part4_client/assets/126570628/7c4c4d54-81b3-4a19-b419-a6a7c89e4bb7)

