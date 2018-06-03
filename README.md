# OpenALPR Xamarin
A Open-source Xamarin integration for [OpenALPR](https://github.com/openalpr/openalpr).

## Introduction
Ever wanted to use OpenALPR with Xamarin but never could? Look no further! After tons of research and testing, I've developed a solution that uses the Native JNI Libraries in combination with Android AAR libraries to create a Xamarin Library that can be used to execute OpenALPR recognition.

## Contents of this Repository
- **ALPRCamera.Droid** which is used for real time recognition of license plates with Android Camera2 API. 

- **OpenALPR Xamarin.Android Binding** which is used to bind the .AAR file generated from [SandroMachado's](https://github.com/SandroMachado/openalpr-android) Android Project. This creates a bindable DLL to use in the next bullet.

- **OpenALPR Xamarin.Android Library** which is used to bind the previous Binding into a neat and easy assembly for management and execution.

## Requirements
- Android 4.1+
- Latest version of Xamarin
- Newtonsoft.Json

## How to build
1. Disable 'Use shared runtime' in Android options.
2. Build projects 1 by 1. OpenALPR Binding -> OpenALPR Library -> Camera application.

```
## Credits
- Java code from SandroMachado (https://github.com/SandroMachado/openalpr-android) which was used to create an AAR library
- OpenALPR (for making the core functionality behind the Recognition technology) (https://github.com/openalpr/openalpr)
- Xamarin Monodroid samples (https://github.com/xamarin/monodroid-samples) for example of basic usage of Camara2 API