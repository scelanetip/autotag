# Autotagging with Gcloud

## Steps following: [Building App](https://cloud.google.com/appengine/docs/standard/python3/building-app/) 
### 1. Creating your GCP project


To deploy your app to App Engine, you must create a Google Cloud Platform project and your App Engine application 
resources.

#### A - Install and initialize Cloud SDK
gcloud projects create autotag
#### B - Enable App Engine 
gcloud app create

### 2. Writing a Basic Web Service for App Engine

#### A - Use your GCP user credentials to authenticate with the Cloud SDK and enable local testing with Cloud Datastore
gcloud auth application-default login
#### B - Structuring your web service files
As in building-an-app-1/ from 
python-docs-samples-master/appengine/standard_python37/building-an-app/building-an-app-1
#### C - Testing your web service
`virtualenv venv `

`source venv/bin/activate`

`cd autotag`

`pip install -r requirements.txt`

`python main.py`

#### D - Configuring your web service for App Engine

app.yaml

### 3. Deploying your web service to App Engine
#### A - Deploying your service

To deploy your web service, you run the gcloud app deploy command from the root directory of your project,
where your app.yaml file is located:

`gcloud app deploy`

Each time that you deploy your web service, a new version of that app is created in App Engine. During deployment,
a container image is created using the Cloud Build service, and then a copy is uploaded to Google Cloud Storage
before it is run in App Engine.

#### B - Viewing your service

To quickly launch your browser and access your web service at https://GCP_PROJECT_ID.appspot.com,
enter the following command:
`gcloud app browse`

#### C - Managing your service

[Servicios](https://console.cloud.google.com/appengine/services?_ga=2.191318700.-704648248.1557748524&project=axial-sunup-244209&folder&organizationId=127192002317)
[Versiones](https://console.cloud.google.com/appengine/versions?_ga=2.191318700.-704648248.1557748524&project=axial-sunup-244209&folder&organizationId=127192002317&serviceId=default&versionssize=50)

### 4. Running Django on the App Engine standard environment 

[Writing your first Django app](https://docs.djangoproject.com/en/1.11/intro/tutorial01/)



# [Label Detection Tutorial](https://cloud.google.com/video-intelligence/docs/label-tutorial)
[Django File Upload](https://www.youtube.com/watch?v=Zx09vcYq1oc)