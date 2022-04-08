# Croatian Word Frequency List

## Summary
A list of the most frequently used words and lemmas in the Croatian language.

## Purpose
The 2,500 most common words from the combined word frequency lists are used to produce decks of Anki SRS cards [16] for words and lemmas. Cards for each word or lemma contain a lemma [12], dictionary definitions, example sentences, an image, text to speech and English translations. The cards are utilized in the Refold learning methodology [17].

## Usage

## Structure
Data, spreadsheet calculations and documentation are stored on Github. Binary objects such as images and sound are stored on Ankiweb.									

## Sources
The word frequency list was compiled from two corpus.

- Croatian news websites [1]
- OpenSubtitles [2]

This gives a mixture of both written and spoken words. Subtitles are often translations of speech from another language but suffices until a corpus of spoken Croatian is found.

These items were removed from the corpuses:
- Non-Ljekavian words
- Personal names
- English loanwords [21]
- Abbreviations
- Units of measurement
- Interjections
- Cardinal numbers
- Ordinal numbers
- Days
- Months
- Currencies
- Place names
- Residencies
- Colloquialisms
- Brands
- Sports team names
- Sports terminology
- Organizations
- Onomatopoeia

Dictionary definitions were sourced from Školski Rječnik Hrvatskoga Jezika [5], Hrvatski Jezični Portal [8] and Wiktionary [10].

Curated example sentences were sourced by the author and automated example sentences were sourced from Tr-ex.me [6]

Images are from various websites found via Google image search.

Text to speech was sourced from the Microsoft Azure Text to Speech service [13].

## Methodology
The Anki cards are compiled in a spreadsheet. The spreadsheet handles storage of all the text data sources and the calculations. The card fields are populated using spreadsheet data and various Anki plugins.

### Card Fields
- Croatian Word
  - Inflected word
- English Word
  - Automated translation created with the =GOOGLETRANSLATE() spreadsheet function and later author curated.
  - Translation of nouns is assumed to be singular when the inflection is inconclusive.
  - Translation of verbs is assumed to be neuter gender when the inflection is inconclusive.
- Croatian Lemma
  - Lemma for the word is looked up using the word to lemma relationship defined by the ENRI corpus.
- English Lemma
  - Automated translation created with the =GOOGLETRANSLATE() spreadsheet function and later author curated.
- Croatian Lemma Definition
  - Definition of the word's lemma from the Pravopis-anki-deck project [3] the data set or manually from alternative sources.
- English Lemma Definition
  - Definition of the word's lemma retrieved with a modified version of the wiktionaryCopy Anki add-on [15].
  - Definition is assumed to be the first usage defined in the dictionary.
- Croatian Sentence Curated
  - Example sentence selected by the author from various sources.
- English Sentence Curated
  - Translation taken from various sources or author created.
- Croatian Sentence Automated 1
  - Example sentence retrieved with an author created Anki add-on.
- English Sentence Automated 1
  - Example sentence translation retrieved with an author created Anki add-on.
- Croatian Sentence Automated 2
- English Sentence Automated 2
- Croatian Sentence Automated 3
- English Sentence Automated 3
- Croatian Sentence Curated TTS
  - Speech generated with the AwesomeTTS Anki add-on [19] using the Microsoft Azure Srecko (neural) voice [13] at 0.85 speed.
- Croatian Sentence Automated 1 TTS
  - Speech generated with the AwesomeTTS Anki add-on [19] using the Microsoft Azure Srecko (neural) voice [13] at 0.85 speed.
- Croatian Sentence Automated 2 TTS
- Croatian Sentence Automated 3 TTS
- Image
  - Author selected image of the Word's lemma found using the Batch Download Pictures from Google Images [20] anki add-on.
  - Different parts of speech (noun, verb, adverb, etc.) from the same root word have different images.
- Word List Position
  - Combined average word frequency position in the available corpuses.

### References

- [1]	“Corpus info: ENGRI (Croatian news portals),” Clarin.si. [Online]. Available: https://clarin.si/noske/run.cgi/corp_info?corpname=engri&struct_attr_stats=1&subcorpora=1.
- [2]	H. Dave, “FrequencyWords.” [Online]. Available: https://github.com/hermitdave/FrequencyWords.
- [3]	“Pravopis-anki-deck.” [Online]. Available: https://github.com/Juraj-B/Pravopis-anki-deck.
- [4]	“Hrvatski rječnik za aspell - Linux,” Linux.hr. [Online]. Available: http://cvs.linux.hr/spell/.
- [5]	“Školski rječnik hrvatskoga jezika,” Xn--rjenik-k2a.hr. [Online]. Available: http://xn--rjenik-k2a.hr/.
- [6]	“Croatian-English dictionary - translation,” Tr-ex.me. [Online]. Available: https://tr-ex.me/translation/croatian-english/.
- [7]	“hrvatski - engleski rječnik,” Glosbe.com. [Online]. Available: https://hr.glosbe.com/hr/en.
- [8]	“Hrvatski jezični portal,” Znanje.hr. [Online]. Available: https://hjp.znanje.hr/index.php?show=main.
- [9]	“Značenje, definicije i primjeri hrvatskih riječi - Jezikoslovac Rječnik,” Jezikoslovac.com. [Online]. Available: https://jezikoslovac.com/.
- [10]	“Wiktionary, the free dictionary,” Wiktionary.org. [Online]. Available: https://en.wiktionary.org/wiki/Wiktionary:Main_Page.
- [11]	“Hrvatski pravopis,” Hrvatski pravopis. [Online]. Available: https://geek.hr/pravopis/.
- [12]	R. Nordquist, “No, it’s not an animal: Find out about lemmas,” ThoughtCo. [Online]. Available: http://thoughtco.com/what-is-a-lemma-1691108.
- [13]	“Text to Speech,” Microsoft.com. [Online]. Available: https://azure.microsoft.com/en-us/services/cognitive-services/text-to-speech/.
- [14]	“Programsko sučelje aplikacije (API) – Ispravi.me,” Ispravi.me. [Online]. Available: https://ispravi.me/info/api/.
- [15]	“wiktionaryCopy: Anki add-on to copy the block of Wiktionary corresponding to a chosen language.” [Online]. Available: https://github.com/gustavklopp/wiktionaryCopy.
- [16]	“Anki - powerful, intelligent flashcards,” Ankiweb.net. [Online]. Available: https://apps.ankiweb.net/.
- [17]	“What is Refold?,” Refold.la. [Online]. Available: https://refold.la/about.
- [18]	“BibGuru - A new FREE APA, Harvard, & MLA citation generator,” Bibguru. [Online]. Available: http://bibguru.com.
- [19]	“AwesomeTTS - Add speech to your flashcards,” Ankiweb.net. [Online]. Available: https://ankiweb.net/shared/info/1436550454.
- [20]	“Batch download pictures from Google images,” Ankiweb.net. [Online]. Available: https://ankiweb.net/shared/info/561924305.
- [21]	R. Nordquist, “What loanwords do you use every day?,” ThoughtCo. [Online]. Available: https://www.thoughtco.com/what-is-a-loanword-1691256.
