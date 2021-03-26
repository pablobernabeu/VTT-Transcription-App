<img align="left" width="50" height="50" src="https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/Royalty-free%20from%20needpix.com.png">

# VTT Transcription App

**VTT Transcription App** is an open-source, R-based web application that allows the conversion of subtitle files from [Web Video Text Tracks (WebVTT) Format](https://www.w3.org/TR/webvtt1/) (example files available [here](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/Example_subtitles_1.vtt) and [here](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/Example_subtitles_2.txt)) into plain texts. For this purpose, users upload a VTT file with extension `.vtt` or `.txt`. Automatically, metadata such as timestamps are removed, and the text is formatted into a paragraph. The result is displayed on the website, and can be downloaded as `.docx` and `.txt` documents. Overall, this application serves to improve the accessibility of subtitles.

## :globe_with_meridians:&nbsp; The web application can be [launched here](https://pablo-bernabeu.shinyapps.io/VTT-Transcription-App/) or [here](https://mybinder.org/v2/gh/pablobernabeu/VTT-Transcription-App/HEAD?urlpath=shiny)

The data is only available to the user, and is deleted when the website is closed.

Questions and suggestions can be submitted as [issues](https://github.com/pablobernabeu/VTT-transcription/issues) or emailed to p.bernabeu@lancaster.ac.uk. The app can be extended via pull requests.

Developer: Pablo Bernabeu (Dept. Psychology, Lancaster University). Licence: [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/).

## Code details

The core of the application is in the [index.Rmd](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/index.Rmd) script, which uses '[regular expressions](https://stringr.tidyverse.org/articles/regular-expressions.html)' to process the VTT file. In turn, that script draws on [another one](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/VTT-Transcription-App_doc_renderer.Rmd) to enable the download of `.docx` documents. Last, the latter script in turn uses a [Word template](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/VTT-Transcription-App-format-template.docx).
