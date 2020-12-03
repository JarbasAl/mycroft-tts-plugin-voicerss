## Description
Mycroft TTS plugin for [VoiceRSS](http://www.voicerss.org)

The "plugins" are pip install-able modules that provide new engines for mycroft

more info in the [docs](https://mycroft-ai.gitbook.io/docs/mycroft-technologies/mycroft-core/plugins)

## Install


`mycroft-pip install jarbas-tts-plugin-voicerss`

## Configuration

Get a [api key](http://www.voicerss.org/api/) and modify your [mycroft.conf](https://mycroft-ai.gitbook.io/docs/using-mycroft-ai/customizations/mycroft-conf)

```json
  "tts": {
    "module": "voicerss_tts_plug",
    "voicerss_tts_plug": {
      "key": "YOUR_API_KEY",
      "voice": "John",
      "lang": "en-us",
      "speed": 0
    }
 
```

`key` - the api key

`lang` - optional, by default will use global language configured for mycroft

`speed` - optional, The speech rate. from -10 (slowest speed) up to 10 (fastest speed). Default value: 0 (normal speed).

`voice` - optional, depends on a language. See voice list [here](http://www.voicerss.org/api/)

### Supported Languages


```json
{
"ca-es": ["Catalan"],
"zh-cn": ["Chinese (China)"],
"zh-hk": ["Chinese (Hong Kong)"],
"zh-tw": ["Chinese (Taiwan)"],
"da-dk": ["Danish"],
"nl-nl": ["Dutch"],
"en-au": ["English (Australia)"],
"en-ca": ["English (Canada)"],
"en-gb": ["English (Great Britain)"],
"en-in": ["English (India)"],
"en-us": ["English (United States)"],
"fi-fi": ["Finnish"],
"fr-ca": ["French (Canada)"],
"fr-fr": ["French (France)"],
"de-de": ["German"],
"it-it": ["Italian"],
"ja-jp": ["Japanese"],
"ko-kr": ["Korean"],
"nb-no": ["Norwegian"],
"pl-pl": ["Polish"],
"pt-br": ["Portuguese (Brazil)"],
"pt-pt": ["Portuguese (Portugal)"],
"ru-ru": ["Russian"],
"es-mx": ["Spanish (Mexico)"],
"es-es": ["Spanish (Spain)"],
"sv-se": ["Swedish (Sweden)"],
}
```