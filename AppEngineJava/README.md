# Random Number Generator

Live Implementation: https://random-number-gcp.appspot.com/

## App Engine

This implementation of the web server was created in Google App Engine using Java. It can be compiled using the same platform.

First, open the Google Cloud Repository, and clone  the project, then navigate to correct repository:

```
git clone https://github.com/Blake-Sam-Dom/AppEngineRandomGenerator.git
cd AppEngineRandomGenerator/
```

## Local Testing

Once inside the correct repository, we can use the Cloud Shell to test it locally and ensure its function. This can be done with the following command:

```
mvn appengine:run
```

You are now able to see what the app will look like from the "Web Preview" mode, that Cloud Shell has.

## App Deployment

To deploy the app, we will use different Cloud Shell commands. First, an app and region needs to be created:

```
gcloud app create
gcloud config set project \[Project-ID]
```

Where "Project Name" is the name of the project you are using.

Finally, simply run the following command:

```
mvn appengine:deploy
```

This will result in the deployment of your web app. The url will be [Project-ID].appspot.com, and should now be accessible.