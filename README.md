# automatic-language-detection-redirect.js
automatic-language-detection-redirect.js

```javascript
//automatic-language-detection-redirect.js

//original code: https://gist.github.com/fv0/f8acf201faee95cf02e9365dcd0d46a0

// Set of supported languages
var supportedLanguages = { en: "en", en: "en-US", es: "es", es: "es-ES", es: "es-MX", es: "es-CL", jp: "jp", fr: "fr", de: "de", it: "it", pt: "pt", ru: "ru", zh: "zh", tr: "tr" };
var fallbackLanguage = "en";

// Check if the users browser language is a supported language of the website. Otherwise go to fallback.
var language = supportedLanguages[(navigator.language || navigator.userLanguage).substring(0,2)] || fallbackLanguage;

// Go to the language version of your website. Example: https://domain.com/en/

// Place the "." by your web domain, since the point is to test it in a local file

location.replace("." +  "/" + language + "/" + "index.html");

```

--- 

## Special Thanks To

![Visual Studio Code logo](https://raw.githubusercontent.com/HappyRogelio7/automatic-language-detection-redirect.js/master/vscode.png?size=100x100)

[Visual Studio Code](https://www.jetbrains.com/idea/), Code editor for Java and other programming languages and programs.
