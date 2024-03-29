<img align="left" width="50" height="50" src="https://github.com/pablobernabeu/VTT-Transcription-App/raw/main/assets/Royalty-free%20from%20needpix.com.png">

# WebVTT caption transcription app

This open-source, R-based web application allows the conversion of video captions (subtitles) from the [Web Video Text Tracks (WebVTT) Format](https://www.w3.org/TR/webvtt1/) into plain texts. For this purpose, users upload a WebVTT file with the extension `.vtt` or `.txt` (examples available [here](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/assets/Example_subtitles_1.vtt) and [here](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/assets/Example_subtitles_2.txt)). Automatically, metadata such as timestamps are removed, and the text is formatted into a paragraph. The result is displayed on the website, and can be downloaded as `.docx` and `.txt` documents. Overall, this application serves to improve the accessibility of video captions.

## The web application can be [launched here](https://pablo-bernabeu.shinyapps.io/VTT-Transcription-App/).

The data is only available to the user, and is deleted when the website is closed.

Questions and suggestions can be submitted as [issues](https://github.com/pablobernabeu/VTT-transcription/issues) or emailed to pcbernabeu@gmail.com. The app can be extended via pull requests.

Developer: Pablo Bernabeu (Dept. Psychology, Lancaster University). Licence: [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/).

## Code details

The core of the application is in the [index.Rmd](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/index.Rmd) script, which uses '[regular expressions](https://stringr.tidyverse.org/articles/regular-expressions.html)' to process the VTT file. In turn, that script draws on [another one](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/assets/VTT-Transcription-App_doc_renderer.Rmd) to enable the download of `.docx` documents. Last, the latter script in turn uses a [Word template](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/assets/VTT-Transcription-App-format-template.docx).
