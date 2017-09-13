This Node-RED Introduction 101 repository is useful as a pre-hackathon webinar introduction to Bluemix, Watson Cognitive Services and Node-RED.  Many of the projects at your hackathon could use Node-Red on the IBM BlueMix platform to integrate devices, APIs and online services.  It is essential that all participants have foundational knowledge of this technology prior to attending the event.

Webinar Topics:
1. Creating a Bluemix Account
2. Bluemix Overview
3. Watson Cognitive Services Overview
4. Node-Red Overview
- Concept of flows and nodes
- Input & Outputs
- Debug and inject nodes
5. Check out additional Node-RED flows in my [TJBot-Node-RED](https://github.com/johnwalicki/TJBot-Node-RED) repository.

This Node-RED-Introduction101 repository includes a presentation, [Node-RED Flows](NodeRED-examples.flow), Node-RED Flow [screenshots](/Screenshots/) that can be used during a pre-hackathon webinar.

Presenters: John Walicki

## Node-RED flows in this repository:
This flow describes how to create the basic Hello World in a few steps.
1. Drag an Inject node from the palette
2. Drag a Debug node from the palette and wire the two nodes together
3. Double click on the Inject node and change it to inject an A-Z String "Hello World"
4. Press the Red Deploy button in the top Right corner. Press the blue Inject. The Hello World string will appear in the Debug area.
![Hello World](/Screenshots/HelloWorld-Inject-annotated.png?raw=true "Hello World")
This flow describes how to use the language translation node:
5. Drag a Language Translation node from the palette.
6. Double click on the Language Translation node and select German
7. Press the Red Deploy button in the top Right corner. Press the blue Inject. The I am a Berliner string will appear in the Debug area.
![Language Translation](/Screenshots/IchbineinBerliner-Translate-annotated.png?raw=true "Ich bin ein Berliner")
This flow speaks the Berlin weather forecast in German
* Call the Weather Insights for the forecast in Berlin.
* Builds a sentence
* Call language translation to convert to German
* Call Text to Speech to generate a WAV file
* Plays the weather forecast in a German voice
![Weather Forecast](/Screenshots/WeatherForecastinGerman.png?raw=true "Speak the Berlin weather forecast in German")
This flow analyzes incoming Tweets
* Configure the Twitter node for a hashtag
* Convert Tweets to speech and speak them
* Call Tone Analysis node
* Find the highest tone score
* TXT Joyful tweets to a phone number
![Tone Analyzer](/Screenshots/ToneAnalyzer.png?raw=true "Twitter Analyzer flow")
