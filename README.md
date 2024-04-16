# IAM Custom Roles 

# Overview
Cloud IAM provides the right tools to manage resource permissions with minimum fuss and high automation. You don't directly grant users permissions. 
Instead, you grant them roles, which bundle one or more permissions. 
This allows you to map job functions within your company to groups and roles. 
Users get access only to what they need to get the job done, and admins can easily grant default permissions to entire groups of users.

## There are two kinds of roles in Cloud IAM:

- Predefined Roles
- Custom Roles
Predefined roles are created and maintained by Google. Their permissions are automatically updated as necessary, such as when new features or services are added to Google Cloud.

Custom roles are user-defined, and allow you to bundle one or more supported permissions to meet your specific needs. 
Custom roles are not maintained by Google; when new permissions, features, or services are added to Google Cloud, your custom roles will not be updated automatically.
You create a custom role by combining one or more of the available Cloud IAM permissions. Permissions allow users to perform specific actions on Google Cloud resources.

## PROCEDURES
After the Google Cloud console opens in this tab.

![image](https://github.com/gaiyejumo/IAM-custom-Roles-on-Google-Cloud/assets/41402706/883d3aa2-92f6-4286-8a5c-96e95310091e)

Activate Cloud Shell
Cloud Shell is a virtual machine that is loaded with development tools. It offers a persistent 5GB home directory and runs on the Google Cloud. Cloud Shell provides command-line access to your Google Cloud resources.

Click Activate Cloud Shell Activate Cloud Shell icon at the top of the Google Cloud console.
When you are connected, you are already authenticated, and the project is set to your Project_ID, PROJECT_ID. The output contains a line that declares the Project_ID for this session:

Note: Your Cloud Platform project in this session is set to "PROJECT_ID"

gcloud is the command-line tool for Google Cloud. It comes pre-installed on Cloud Shell and supports tab-completion.

(Optional) You can list the active account name with this command:

```
gcloud auth list
```

Click Authorize.
Output:

ACTIVE: *
ACCOUNT: "ACCOUNT"

To set the active account, run:
    $ gcloud config set account `ACCOUNT`


(Optional) You can list the project ID with this command:
```
gcloud config list project
```

Output:

[core]
project = "PROJECT_ID"
Note: For full documentation of gcloud, in Google Cloud, refer to the gcloud CLI overview guide.
