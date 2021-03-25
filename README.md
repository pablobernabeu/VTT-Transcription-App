# VTT Transcription App

**VTT Transcription App** is an open-source, R-based web application that allows the conversion of [Web Video Text Tracks Format (WebVTT) files](https://developer.mozilla.org/en-US/docs/Web/API/WebVTT_API) into plain text documents. The VTT files can be uploaded one by one, either in 'txt' or 'vtt' format. The application removes metadata such as timestamps, and structures the text. Files can be quickly uploaded, processed and downloaded in succession. The result can be downloaded as 'docx' or 'txt' documents.

## :globe_with_meridians:&nbsp; The web application can be [launched here](https://pablo-bernabeu.shinyapps.io/VTT-Transcription-App/)

The data is only visible to the person who uploads it.

Since this application has not been exhaustively tested yet, you may wish to revise the result of the process, which is directly displayed on the website.

Questions and suggestions can be submitted as [issues](https://github.com/pablobernabeu/VTT-transcription/issues), and the app can be extended via pull requests.

Developer: Pablo Bernabeu (Dept. Psychology, Lancaster University). Licence: [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/).

## Code details

The core of the application is in the script [VTT-Transcription-App.Rmd](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/VTT-Transcription-App.Rmd). This file uses [an additional script](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/VTT-Transcription-App_doc_renderer.Rmd)--to the download of `docx` documents. In turn, the latter file uses a [Word template](https://github.com/pablobernabeu/VTT-Transcription-App/blob/main/VTT-Transcription-App-format-template.docx) to format the `docx` documents.
