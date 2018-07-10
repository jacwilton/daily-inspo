# daily-inspo
pip install twilio
python setup.py install
from twilio.rest import Client

# Your Account SID from twilio.com/console
account_sid = ""
# Your Auth Token from twilio.com/console
auth_token  = ""

client = Client(account_sid, auth_token)
myTwilioNumber = '+16314029977'
to = ''
message = client.messages.create(body=
