# Zoom Notification

Sharing this package to have a custom solution when a team wants a constant monitoring on a dedicated meeting id. 

## Web Hooks Only

Webhook-only apps use Event Subscriptions to integrate and connect third-party services to the Zoom platform when an action (event) is triggered. This allows you to automate the task of being notified when a certain event occurs in your Zoom account without making repeated API calls.

Notifications are sent to an endpoint URL in the form of an HTTP POST request with a JSON payload describing the event. This could allow your application could to send data to your server when a new  or  is created, store recorded data when a  has ended, or enable  events to notify your database when a user uninstalls your app.

```bash
For a full look into Webhook-only apps, Read: https://marketplace.zoom.us/docs/guides/build/webhook-only-app
```

## Web Hook Resources

1. https://marketplace.zoom.us/docs/api-reference/webhook-reference/meeting-events/meeting-participant-joined-before-host

2. https://marketplace.zoom.us/docs/api-reference/webhook-reference/meeting-events/participant-joined-meeting


## Zoom API

```python 
Version:       2.0.0
Host:          api.zoom.us/v2
Protocols:     https
Accepts:       application/json, multipart/form-data
Responds With: application/json, application/xml
```

## Custom Notification

1. Notifications when participants joins 

2. Notification when participant is waiting for host to join


## Pre-requisete 

Pro or a higher plan.

"Enable join before host" option should be turned on for the scheduled meeting.

Event Subscriptions must be enabled for your  with the following configurations: 

- A valid Event Notification Endpoint URL.
- "Participant joined meeting before host" subscription enabled under the Meeting event.

## License
[MIT](https://opensource.org/licenses/MIT)
