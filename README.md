import webbrowser #to open edge
import pywhatkit # to text on whatsabb web
import urllib.parse  # URL encoding
def open_whatsapp_chat(phone_number, message):
    # format URL
    encoded_message = urllib.parse.quote(message)
    whatsapp_url = f"https://web.whatsapp.com/send?phone={phone_number}&text={encoded_message}&time={time_hour, time_minute}"
    # open the URL on whatsapp
    webbrowser.open(whatsapp_url)
phone_number= '#add phone number here'
message= 'Hey, I am texting you using a python code'
time_hour= 16 #specific hour
time_minute= 40

open_whatsapp_chat(phone_number, message)
pywhatkit.sendwhatmsg(phone_number, message, time_hour, time_minute)
