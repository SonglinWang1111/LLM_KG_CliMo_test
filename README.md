## LLM-assisted Climate Mobility Knowledge Graph: A Test
### Description
This is a very first test on LLM assisted climate mobility knowledge graph construction, using prompting. The data I used was 11 emperical papers of climate mobility. One as example ('shot'), and others as testing data.

I first used [this tool](https://github.com/titipata/scipdf_parser#installation) in 'pdf2text' for parsing those papers into dictionaries (1->1), with section names as keys and section contents as values, then cleaned those dictionaries a bit, removing unrelated parts. Results were saved in 2 .npy files, for example and testing dataset respectively.

Those 2 files about prompting are for characteristic detection (like method, research area...) and triples extraction (heading, relationship, tail) respectively. Prompts are now not perfect I would say, but I already got some interesting results (see those two tables). Note that api key has been deleted before committing. I also have to merge them into one file later.

No automatic evaluation available now, but manually evaluated the characteristics detected. Around 30% records are different from the manual results did by literature reviewers before, however, honestly, I can't say whose false it is. The thing is for the example paper which I had to detect such characteristics by myself, I also have different ideas compared to them. I have to discuss with those folks about this.
