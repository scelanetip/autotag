# Autotagging with Gcloud

## Steps following [1] 
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


## References
[1] https://cloud.google.com/appengine/docs/standard/python3/building-app/
