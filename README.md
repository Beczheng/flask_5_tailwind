# flask_5_tailwind

### Assignment
- Course: HHA 504
- Homework assignment #5: Gain hands-on experience in video hosting, creating a Flask app styled with Tailwind CSS, and deploying it to a cloud platform. Leverage CDN services in Google Cloud or Azure.

### Video Procurement
- Downloaded a dog video from YouTube.

### Video Hosting using Cloud CDN
- Login to your Microsoft Azure account.
- Type in `storage accounts` in the search bar.
- Click `create`.
- Create or select a name for your resource group and storage account name.
- Click `create`.
- Go back to the home page and click on the your storage account.
- Under the nagivation bar, go to overview. Scroll down and click `security`. Then, click the `enable` option for `make sure secure transfer required`, `allow blob anonymous access`, and `allow storage account key access`. Lastly, click `save`.
- Under the nagivation bar and go to containers. Then, click `+ containers`, Next, create a name and change the anonymous access level to `container(anonymous read access for containers and blob`. Lastly, click `+ create`.
- Under the nagivation bar, go to security + networking. Then, click `front door and CDN`. Under service type, click the `Azure CDN` option. Next, create a profile name and endpoint name. Lastly, change the query string caching behavior to `ignore query string` and click `create`.
- Go back to the home page and click on your new storage account. Then, click `upload`. Upload a video that is less than 60 seconds and select an existing container. Lastly, click `upload`.
- Go back to the home page and click on your new storage account. Under the navigation bar, click `containers`. Then, click on your new container. Lastly, copy the URL link.
- Go back to the home page and go to Front Door and CDN profle. Then, click on the hostname. Next, click on the endpoint hostname. Lastly, combine the hostname with the URL link (only combine everything after .net) from the container.

### Flask App With Tailwind CSS
- For more information about my flask application, click [here.](https://github.com/Beczheng/flask_5_tailwind/tree/main/templates)

### Deploy Flask App on Azure
- In your Cloud Shell terminal, type `curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash`. This will install the Azure CLI.
- Type `az` to check if Azure CLI is installed.
- Type `az login --use-device-code`. A link with a code will appear. Click on the link and enter the code. Then, login to your Microsoft Azure account. This will give Cloud Shell permission to access your Azure account.
- Type `az account list --output table`. This will provide you a table of your subscriptions. Make sure that you are using the correct subscription. If not, type `az account set --subscription <SubscriptionId>` to change it.
- Type `az group list` to double check everything.
- Type `az webapp up --name <appname> --runtime PYTHON:3.9 --sku B1`. This will create a webapp for your Flask app.
- To find your Flask app in your Microsoft Azure account, go to "App Services". Then, click on the name of your webapp. Lastly, click on the link to your webapp under "default domain".


