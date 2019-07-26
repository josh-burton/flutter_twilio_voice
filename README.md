# flutter_twilio_voice

Provides an interface to Twilio&#x27;s Programmable Voice SDK to allows adding voice-over-IP (VoIP) calling into your Flutter applications.

## Getting Started

This project is a starting point for a Flutter
[plug-in package](https://flutter.dev/developing-packages/),
a specialized package that includes platform-specific implementation code for
Android and/or iOS.

For help getting started with Flutter, view our 
[online documentation](https://flutter.dev/docs), which offers tutorials, 
samples, guidance on mobile development, and a full API reference.

## Configure Server to Generate Access Token

View Twilio Documentation on Access Token Generation: https://www.twilio.com/docs/iam/access-tokens

## Make a Call

```
 await FlutterTwilioVoice.makeCall(
                   accessTokenUrl: "https://${YOUR-SERVER-URL}/accesstoken",
                   to: "$client_identifier_or_number_to_call");

```


## Mute a Call

```
 await FlutterTwilioVoice.muteCall(isMuted: true);

```

## Toggle Speaker

```
 await FlutterTwilioVoice.toggleSpeaker(speakerIsOn: true);

```

## Hang Up

```
 await FlutterTwilioVoice.hangUp();

```

## Client Setup to Receive Calls

```
 await FlutterTwilioVoice.receiveCalls(clientIdentifier: 'alice');

```


## TO DO

1. Android Support
2. Propagate Events and Call Status Notifications to Flutter



