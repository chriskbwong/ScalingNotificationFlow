# ScalingNotificationFlow
SMS to phone call Twilio studio flow. 

You can import the JSON by following this guide:
https://www.twilio.com/docs/studio/user-guide#importing-flow-data

You need to make an API request in order to kick off of this studio flow. Here's a cURL request that details what parameters go need to be passed through.

curl -X POST “https://studio.twilio.com/v1/Flows/YOUR_TWILIO_FLOW_SID/Executions” -d “To=YOUR_TO_NUMBER” -d “From=YOUR_TWILIO_NUMBER” -d “Parameters={\“RestaurantName\“:\“Stein's Fine Dines\“, \“WaitTime\“:\“30 minutes\“, \“CustomerName\“:\“Chris Wong\“, \“OrderInfo\“:\“Fine Wine\“, \“EndUserPhoneNumber\“:\“SOMEONE_ELSE'S_PHONE_NUMBER\“}” -u YOUR_TWILIO_ACCOUNT_SID:YOUR_TWILIO_AUTH_TOKEN
