---

copyright:
  years: 2015, 2019
lastupdated: "2019-04-08"

subcollection: text-to-speech

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:tip: .tip}
{:important: .important}
{:note: .note}
{:deprecated: .deprecated}
{:pre: .pre}
{:codeblock: .codeblock}
{:screen: .screen}
{:javascript: .ph data-hd-programlang='javascript'}
{:java: .ph data-hd-programlang='java'}
{:python: .ph data-hd-programlang='python'}
{:swift: .ph data-hd-programlang='swift'}

# About
{: #about}

> ** Service update:** *The {{site.data.keyword.texttospeechshort}} service was updated on March 24, 2019. The service now offers Deep Neural Network (DNN) versions of its German voices, and all DNN-based voices now support the `pitch` and `rate` attributes of the SSML `<prosody>` element. For more information, see the [24 March 2019 service update](/docs/services/text-to-speech/release-notes.html#March2019c) in the release notes*.

The {{site.data.keyword.texttospeechfull}} service provides an application programming interface (API) that uses {{site.data.keyword.IBM_notm}}'s speech-synthesis capabilities to convert written text to natural-sounding speech. The service streams the results back to the client with minimal delay. The service offers both [HTTP](/docs/services/text-to-speech/http.html) and [WebSocket](/docs/services/text-to-speech/websockets.html) interfaces.

## Features and capabilities

The {{site.data.keyword.texttospeechshort}} service offers the following features and capabilities:

-   **Audio formats** - Produces audio in Ogg or WebM with the Opus or Vorbis codec, WAV, FLAC, MP3 (MPEG), l16 (PCM), mulaw, or basic format. For more information, see [Audio formats](/docs/services/text-to-speech/audio-formats.html).
-   **Voices** - Synthesizes text to audio in various languages, voices, and dialects. The service offers DNN-based versions of some voices. For more information, see [Languages and voices](/docs/services/text-to-speech/voices.html).
-   **SSML** - Accepts plain text or text that is marked up with the XML-based Speech Synthesis Markup Language (SSML). For more information, see [Using SSML](/docs/services/text-to-speech/SSML.html).
-   **Expressiveness** - Extends SSML with an expressive element that you can use to indicate a speaking style of *GoodNews*, *Apology*, or *Uncertainty*. Available only for the US English Allison voice that is not DNN-based. For more information, see [Expressive SSML](/docs/services/text-to-speech/SSML-expressive.html).
-   **Voice transformation** - Extends SSML by adding a voice transformation element. You can use the element to expand the range of possible voices by controlling aspects such as pitch, rate, and timbre. Also offers two built-in virtual voices, *Young* and *Soft*. Available only for US English voices that are not DNN-based. For more information, see [Voice transformation SSML](/docs/services/text-to-speech/SSML-transformation.html).
-   **Word timings** - With the WebSocket interface, supports the SSML `<mark>` element and optional word timing information for all strings of the input text. Timing information synchronizes the input text and the resulting audio. For more information, see [Obtaining word timings](/docs/services/text-to-speech/word-timing.html).
-   **Customization** - Provides a customization interface that you can use to specify how the service pronounces unusual words that occur in your input. You can define pronunciations with the International Phonetic Alphabet (IPA) or {{site.data.keyword.IBM_notm}} Symbolic Phonetic Representation (SPR). For more information, see [Understanding customization](/docs/services/text-to-speech/custom-intro.html).

For more information about the pricing plans for the service, see the {{site.data.keyword.texttospeechshort}} service in the [{{site.data.keyword.cloud_notm}} Catalog ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://{DomainName}/catalog/services/text-to-speech){: new_window}.

## Language support
{: #languages-index}

The service supports voices in the following languages: Brazilian Portuguese, English (UK and US dialects), French, German, Italian, Japanese, and Spanish (Castilian, Latin American, and North American dialects). The service offers at least one male or female voice, sometimes both, for each language. Each voice uses appropriate cadence and intonation for its dialect. For more information about the voices that are available for each language, see [Languages and voices](/docs/services/text-to-speech/voices.html).

## Use cases
{: #usecases}

The service is appropriate for voice-driven and screenless applications, where audio is the preferred method of output:

-   Interfaces for the disabled, such as assistance tools for the vision-impaired
-   Reading text and email messages aloud to drivers
-   Video-script narration and video voice over
-   Reading-based educational tools
-   Home-automation solutions

## Try out the service

For examples of the service in action, see

-   A [quick demo ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://text-to-speech-demo.ng.bluemix.net/){: new_window} of the {{site.data.keyword.texttospeechshort}} service that accepts text and generates speech with different voices. It offers expressiveness and transformation where supported.
-   Applications in {{site.data.keyword.ibmwatson}} [Starter Kits ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://www.ibm.com/watson/developercloud/starter-kits.html){: new_window} that demonstrate the {{site.data.keyword.texttospeechshort}} service.
