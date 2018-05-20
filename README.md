

multi-language-translator
======

multi-language-translator is a android application with gradle plugin that allows your app to translate multiple languages, without the hassle of working with multiple resources, using the translation editor or ordering an expensive translation from AS/IDEA

It leverages the Yandex API in order to translate your string/voice resources into all the languages specified in the configuration.

Installation
------------

- Clone this repository.

- Open project by Android Studio/JetBrain™ IntelliJ Idea.

You can see the full list of languages here: https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes

ProTips
-------

If you think the translation that was auto generated is not accurate enough you can just override it, by setting the resources in the correct language folder. For example if you are translating to Spanish just create the file: `values-es/strings.xml` and add the resource. Parrot will skip that resource and not perform the translation.
```
<resources>
    <string name="app_name">Mi Aplicación es la mejor</string>
</resources>
````

You can also view the translated resources before they are merged by looking in your build folder.
`{appModule}/build/generated/res/rs/{flavor}/{buildType}/values-{lang}/translated-strings.xml`

Finally
-------
Keep in mind that you have to comply with Yandex Attributtion Requirements. More here: https://tech.yandex.com/translate/doc/dg/concepts/design-requirements-docpage/


License
--------
MIT