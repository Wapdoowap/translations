# Help make FetLife multilingual

This repository stores the raw translation files we use to make [Fetlife](https://fetlife.com/) available in different languages! We're actively looking for people to help us add new translations and make the ones we have better.

To translate FetLife, you’ll need a good knowledge of a language other than English ([CEFR][] B2 or above), an understanding of [YAML][] syntax and a way of editing YAML files, and the ability to use Git.

[CEFR]: https://en.wikipedia.org/wiki/Common_European_Framework_of_Reference_for_Languages#Common_reference_levels
[YAML]: http://yaml.org/
[Git]: https://git-scm.com/

## Process

The software which runs FetLife is still in the process of being localized (a fancy word for ‘having all the bits where there’s a fixed English string replaced with something that can support multiple languages’). Over the next month or two the whole website will slowly become available in German and French; after that we’ll start paying more attention to other languages.

### Contributing to an existing language

In general, if `translations/en.yml` is newer than your language’s own `.yml` file ... you’ve got work to do! You can use `git diff` to find the changes to `en.yml` since the last update.

### Starting a new language

As a rough guideline, at the moment we can only translate FetLife into languages which have a complete entry in the [Common Locale Data Repository.][cldr] Fortunately this includes most languages you’re likely to want to translate FetLife into. If your language isn’t there, you could start by [contributing basic translations][cldr-contrib] for it to the Unicode Consortium! That way you can help much more software than just FetLife to become available in your language.

[cldr]: http://www.unicode.org/cldr/charts/latest/summary/root.html
[cldr-contrib]: http://cldr.unicode.org/index/bug-reports

As you go along make sure you create an appropriate file in the ‘guidelines’ directory giving your translations for words in the `KEYWORDS.md` file so that future translators can easily make sure there’s consistent translations for them across the whole of FetLife.

You might find in some cases that you need to make things sound stilted or ungrammatical to make them work in FetLife’s translation data files. We’d like to avoid this as much as possible — please [create an issue][issues] whenever this happens so that FetLife’s user interface appears in your language as fluently as possible.

[issues]: https://github.com/fetlife/translations/issues

### Submitting your changes

Fork this repository and send a pull request to us. All new translations have to be vetted by pull request before being merged.

If you include your FL username in your pull request, you’ll get a shiny ‘I translate FetLife’ badge on your profile and you’ll be the envy of all your friends.
