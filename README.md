# Named Entity Linking

Named Entity Linking (NEL) or Named Entity Disambiguation (NED) is the task of determining the identity of entities mentioned in text, linking it to an entity in a knowledge base (KB), such as Wikidata, Wikipedia or DBpedia.

A NEL system must first search for a set of candidate entities that the mention string might refer to, before selecting a single candidate given the document. For example, the mention “Python” was found in a text, after the disambiguation we may know if it refers to the entity Python as a snake, as a programming language, as an animal from Greek Mythology or as a movie.

NEL framework can be separated into 3 main components:

**1.	Extractor:** Extraction is the detection and preparation of named entity mentions. May also include other preprocessing such as tokenizatzion, sentence boundary detection, and in-document coreference.

**2.	Searcher:** Search is the process of generating a set of candidate KB entities for a mention. An ideal searcher should balance precision and recall to capture the correct entity while maintaining a small set of candidates.

**3.	Disambiguator:** In disambiguation, the best entity is selected for a mention. Ranking problem over the candidate set.

For more information about the detection of named entities, please refer to the repository [Named Entity Recognition](../../../Named-Entity-Recognition).

## NEL system

The API for the NEL system was developed with Python and Flask.

![](https://j.gifs.com/jZLAGR.gif)
