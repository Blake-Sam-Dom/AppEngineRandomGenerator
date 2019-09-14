# Random Number Generator

## App Engine

App Engine works best on the Google Cloud Platform

First clone the project repository and navigate:
```
git clone https://github.com/Blake-Sam-Dom/AppEngineRandomGenerator.git
cd AppEngineRandomGenerator/
```

### To test locally:

Create an isolated virtual environment and activate it:
```
virtualenv --python python3 envs/random-number
source envs/random-number/bin/activate
```
Navigate to the program directory:
```
cd random-number/
```
Install required dependencies (the only on is Flask):
```
pip install -r requirements.txt
```
And finally, run the app:
```
python main.py
```
You can now view the app through the Web Preview function

Ctrl + C to terminate app

### To deploy application:

Make sure you are in the correct project (any that does not already have an app deployed) in the Google Cloud Platform

Navigate to program directory and create the app:
```
gcloud app create
```
Now deploy:
```
gcloud app deploy app.yaml --project your-project-id
```
Make sure all the displayed information is correct and press go!

The app will deploy and will live at your-project-id.appspot.com by default

If you want to visit mine, it is live at http://cs-4263-252417.appspot.com/
