# flask_5_tailwind

### Assignment
- Course: HHA 504
- Homework assignment #5: Gain hands-on experience in video hosting, creating a Flask app styled with Tailwind CSS, and deploying it to a cloud platform. Leverage CDN services in Google Cloud or Azure.

### Video Procurement 
- **Video Link:** https://beckie-endpoint.azureedge.net/beckie-container/dogs-life-shorts-dogs-funny-sleepingdogs-labrador-1280-ytshorts.savetube.me.mp4 

### Video Hosting using Cloud CDN
- Login to your Microsoft Azure account.
- Type in `storage accounts` in the search bar.
- Click `create`.
- Create or select a name for your resource group and storage account name.
- Click `create`.
- Go back to the home page and click on the new storage account.
- Under the nagivation bar, click `overview`. Scroll down and click `security`. Then, click the `enable` option for `make sure secure transfer required`, `allow blob anonymous access`, and `allow storage account key access`. Lastly, click `save`.
- Under the nagivation bar and go to `containers`. Then, click `+ containers`, Next, create a name and change the anonymous access level to `container(anonymous read access for containers and blob`. Lastly, click `+ create`.
- Under the nagivation bar, click `security + networking`. Then, click `front door and CDN`. Under service type, click the `Azure CDN` option. Next, create a profile name and endpoint name. Lastly, change the query string caching behavior to `ignore query string` and click `create`.
- Go back to the home page and click on the new storage account. Then, click `upload`. Upload a video that is less than 60 seconds and select a and existing container. Lastly, click `upload`.
- Go back to the home page and click on the new storage account. Under the navigation bar, click `containers`. Then, click on your new container. Next, click on the content. Lastly, copy the URL link.
- Go back to the home page and click on the Front Door and CDN profle. Click on the hostname. Click on the endpoint hostname. For the URL link, copy everything after .net and combine it with your new hostname. Now, keep the new link.

### Flask App With Tailwind CSS
- 

### Cloud Deployment
-

