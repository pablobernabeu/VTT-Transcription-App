<img align="left" width="50" height="50" src="https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/Royalty-free%20from%20needpix.com.png">

# VTT Transcription App

**VTT Transcription App** is an open-source, R-based web application that allows the conversion of [Web Video Text Tracks Format (WebVTT) files](https://developer.mozilla.org/en-US/docs/Web/API/WebVTT_API) into plain text documents. The VTT files can be uploaded one by one, either in `txt` or `vtt` format. The application quickly removes metadata such as timestamps, and structures the text. Files can be successively uploaded, processed and downloaded (`docx` and `txt`).

Since this application has not been exhaustively tested yet, you may wish to revise the result of the transcription, displayed on the website.

## :globe_with_meridians:&nbsp; The web application can be [launched here](https://pablo-bernabeu.shinyapps.io/VTT-Transcription-App/)

The data is only visible to the person who uploads it.

Questions and suggestions can be submitted as [issues](https://github.com/pablobernabeu/VTT-transcription/issues) or by emailing the developer (p.bernabeu@lancaster.ac.uk). The app can be extended via pull requests.

Developer: Pablo Bernabeu (Dept. Psychology, Lancaster University). Licence: [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/).

## Code details

The core of the application is in the [index.Rmd](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/index.Rmd) script. That script draws on [another script](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/VTT-Transcription-App_doc_renderer.Rmd) to allow the download of `docx` documents. The latter script in turn uses a [Word template](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/VTT-Transcription-App-format-template.docx) to format the `docx` documents.
