# flutter_ameno_ipsum

A Flutter package for generating random sentences and paragraphs based on Ameno song from Era. The output looks similar to the famous "lorum ipsum" placeholder text. Useful when designing user interfaces that require example text:

> Adapare dori imperavi adapare ameno ameno emulari. Reo reo matiremo, dori dori am me. Dimere, latiremo mea,latiremo ameno. Dom omenare dore dori me dori imperavi ameno am. Mea me.
> 
> Omenare dori. Emulari dimere adapare. Latire ameno. Imperavi emulari, mea me ameno, me dore emulari reo. Me ameno dom, dom ameno ameno me. Dore dori latiremo reo matiremo. Me imperavi.

## Usage

Import the package:

```dart
import 'package:flutter_ameno_ipsum/flutter_ameno_ipsum.dart';
```

Call the `ameno` function, specifying the number of paragraphs and words to generate.

```dart
String text = ameno(paragraphs: 2, words: 60);
print(text);
```

The above might print:

> Imperavi matiro dori ameno dimere am, mea dori. Ameno, latire ameno, latiremo omenare omenare dimere. Me, ameno mea matiro, dore imperavi latire ameno dore am. Dori mea reo. Imperavi reo.
> 
> Dore me dimere latiremo mea dori. Mea ameno mea mea reo. Am reo dimere reo latiremo, reo latiremo omenare dori dore. Dore matiro latiremo, omenare me latire, ameno dom me.

## How it works

Sentences are formed from a list of words based on the lyrics of Ameno. Up to two commas are inserted per sentence. Shorter words are favoured 50% of the time, which produces a more natural looking sentence.

Words are selected randomly. The sentences are not valid latin! (just like Ameno's lyrics)

## Thanks you !
Thanks to [dmjones](https://github.com/dmjones) for his package [flutter_lorem](https://github.com/dmjones/flutter_lorem)

## Dorime
![](img/dorime.jpg)
