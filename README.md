# Image-Recognition-SMS


Flask application made in Python with Twilio Message service. Allows the user to send pictures to a given number and get a response with relevant keywords from the picture - using Clarifai's image recognition API. This application was made with the aim of experimenting with the Clarifai API.

### Get Started
1. `pip install flask twilio  clarifai`
2. type `nano .bash_profile` to open `.bash_profile`
3. add: `export CHARIFAI_API_KEY=*your API key*`
4. set up your Twilio account
5. start ngrok by typing `ngrok http 5000`
6. configure your phone number in Twilio to have a webhook connected to the ngrok address like this:
![See image](https://s3.amazonaws.com/com.twilio.prod.twilio-docs/original_images/UpFaHOezK9Ryyytjk-nl2MQHHXAgS9aPF3kBMmws3OKj_BiGmdcGtNX0hvfOYwQXS4_evCeDqF.png)
7. run this command: `python app.py`
8. now send a picture to your Twilio phone number and it should return keywords describing the picture
