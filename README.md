 
# Survey goals
- Organization of publicly available information about Polish ASR speech datasets.
- Providing ASR community with the collectively maintained, up-to-date source of information about available resources.
- Identification of ASR speech datasets for Polish, which are freely available for reseach and commercial purposes.
<br>

# Survey results
- **Forty-eight datasets** intended for Polish ASR development were identified
- The **total** **size** of **documented Polish ASR speech data** amounts to over **20000** **hours** of **audio** and nearly **2500** **hours** of **transcribed** speech.
- **One thousand hours** worth speech data is **available** in a public domain
- Over **600 hours** of speech data available through commercial providers. See [Public domain PL ASR speech datasets]
- Each dataset is described with up to 57 attributes. See [Taxonomy](https://github.com/goodmike31/pl-asr-speech-data-survey#taxonomy) for details.
* Detailed analysis results are available at: 
* Resulting Polish ASR speech datasets catalog is available in 2 formats:
  * [Google Sheets](https://docs.google.com/spreadsheets/d/181EDfwZNtHgHFOMaKNtgKssrYDX4tXTJ9POMzBsCRlI/edit?usp=sharing)
  * [TSV](https://github.com/goodmike31/pl-asr-datasets-survey/blob/main/pl-asr-datasets-catalog-latest.tsv)
  
# How to contribute to the Polish ASR speech datasets catalog 

# How to identify public domain PL ASR speech datasets
1. Open [Catalog](https://docs.google.com/spreadsheets/d/181EDfwZNtHgHFOMaKNtgKssrYDX4tXTJ9POMzBsCRlI/edit?usp=sharing)
2. Filter results by column "Usage cost" by allowing only "free" values

# Addendum - Survey design  

## Dataset charateristics analysis process
- Publicly available Infomration sources were analyzed, annotated and standardized according to the Taxonomy
- Additionaly, the content of publicly available datasets was analyzed automatically
 
## Information sources
* Language Data Repositories
  * [Open Speech and Language Resources](https://www.openslr.org/resources.php)
  * [LDC Data Catalog](https://catalog.ldc.upenn.edu/)
  * [ELRA Catalog](http://catalogue.elra.info/en-us/)
  * [META-SHARE repository](http://www.meta-share.org/)
  * [CLARIN ERIC - Virtual Language Observatory](https://vlo.clarin.eu/)
  * [CLARIN-PL - D-space](https://clarin-pl.eu/dspace/)
  * [Open Science Resource Atlas 2.0 (AZON)](https://zasobynauki.pl/)
  * [PELCRA](http://pelcra.pl/new/tools_and_resources)
  * [Hamburger Zentrum fur Sprach Corpora HZSK](https://corpora.uni-hamburg.de/hzsk/)
* Other
  * [PolEval 2019 competition](http://2019.poleval.pl/)
  * [Google dataset search](https://datasetsearch.research.google.com/)
  * [Kaggle](https://www.kaggle.com/)
  * [Hugging face](https://huggingface.co/)
  * [Google Scholar Search](https://scholar.google.com/) (keywords: Polish, ASR, speech corpus, dataset, etc.)
  * [Google Web Search](https://www.google.com/) (keywords: Polish, ASR, speech corpus, dataset, etc.)

## Taxonomy
- The dataset cards taxonomy consists of 57 attributes.
- Each dataset is described ain terms of:
  - authorship, creation date, funding etc.
  - availability, licensing, pricing etc.
  - content e.g. audio format, number of speakers recorded, meta-data distributions, etc.
- Values of attributes not reported by dataset authors, publishers or researchers is recreated, when feasible (e.g. number of recordings)
- Below table shows the dataset card completion rates for manually annotated attributes is.
  - (tabelka)

- Full taxonomy is presented in the table below.

|Dataset descriptor                 |Purpose                                                                             |Allowed values                                                                    |
|-----------------------------------|------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
|Dataset name                       |Full name of the speech corpus                                                      |[a-z A-Z\-\_0-9]                                                                  |
|Codename                           |Codename used for reporting                                                         |[a-z\-]                                                                           |
|Access link                        |Link to resource providing access to dataset                                        |url                                                                               |
|Publisher                          |Creator and/or publisher of dataset                                                 |[a-z A-Z]                                                                         |
|Repository                         |Data repository where dataset is listed and/or hosted                               |                                                                                  |
|Languages                          |Language and country code.                                                          |pl-PL, multi                                                                      |
|Creation year                      |Year dataset was created or published.                                              |\d{4}                                                                             |
|License                            |License of dataset                                                                  |Apache, CC-BY, CC-0, Proprietary                                                  |
|ISLRN                              |International Standard Language Resource Number                                     |ISRLN format                                                                      |
|ISBN                               |International Standard Book Number                                                  |ISBN                                                                              |
|LR catalogue ID/URI                |Language data repository specific ID                                                |URL,  [a-z A-Z\-\_0-9]                                                            |
|Reference publication              |Link to relevant publication where dataset is described                             |URL                                                                               |
|Contact point                      |Contact point                                                                       |[a-z A-Z\-\_0-9\@]                                                                |
|Latest version                     |The latest version of released dataset                                              |[0-9\.]                                                                           |
|Last update year                   |Last update year                                                                    |\d{4}                                                                             |
|Available                          |Is dataset available online                                                         |yes, no                                                                           |
|Funding                            |Institution which funded the creation of dataset                                    |[a-z A-Z\-\_0-9]                                                                  |
|usage cost                         |Availability for non-commercial usage                                               |free, paid, no-info                                                               |
|Price - non commercial usage       |Price for non-commercial usage                                                      |[free&#124;\d+]                                                                        |
|Price - Commercial usage           |Price for commercial usage                                                          |[free&#124;\d+]                                                                        |
|Purpose and split                  |Target usage and data split                                                         |train, valid, test, none                                                          |
|Size audio total [hours]           |Audio material                                                                      |[\d+\.]                                                                           |
|Size audio transcribed [hours]     |Transcribed speech material                                                         |[\d+\.]                                                                           |
|Size [GB]                          |Size of dataset in gigabytes.                                                       |[\d+\.]                                                                           |
|Speakers                           |Number of speakers recordings orignate from                                         |[\d+]                                                                             |
|Audio recordings                   |Number of voice recordings in the corpus                                            |\d+                                                                               |
|Audio segmentation                 |Are audio recordings segmented                                                      |yes, no                                                                           |
|Tokens                             |Number of tokens in the corpus                                                      |[\d+]                                                                             |
|Unique tokens                      |Number of unique tokens                                                             |[\d+]                                                                             |
|Automatic QA                       |Type of automatic quality assurance process applied                                 |yes, no                                                                           |
|Manual QA                          |Type of manual quality assurance process applied                                    |yes, no                                                                           |
|Manual QA scope                    |Scope of manual QA applied                                                          |[a-zA-Z \d+]                                                                      |
|Transcription coverage             |Percent of recordings having corresponsing transcription                            |percent                                                                           |
|Transcription protocol             |Is a transcription protocol availble as reference?                                  |yes, no, description                                                              |
|Normalized transcriptions          |Are there available transcriptions without abbreviations, numerals, punctuation etc.|yes, no                                                                           |
|Transcription and annotation format|Format of transcription files                                                       |                                                                                  |
|Domain                             |Domain of utterances                                                                |                                                                                  |
|Speech type                        |Type of speech                                                                      |read, conversional, commands, isolated words, synthetic, multi-type               |
|Audio collection process           |Audio collection process                                                            |controlled, corpus                                                                |
|Speech recordings providers        |Who provided speech recordings                                                      |volunteers, university employees, crowd, public speakers, paid contributors       |
|Acoustic environment               |Acoustic conditions audio was collected in                                          |quiet, various, home, office, tv show, car, public places, entertainment, children|
|Audio device                       |Device audio was recorded with                                                      |various, condenser mic, headset, phone, mobile phone                              |
|Device model                       |Mode of recording device                                                            |[a-zA-Z\- ]                                                                       |
|Audio format                       |Audio encoding format                                                               |wav, flac, raw, mp3, riff                                                         |
|Audio codec                        |                                                                                    |mp3, ogg, vorbis, opus,                                                           |
|Channels                           |                                                                                    |                                                                                  |
|Sampling rate [Hz]                 |Sampling rate of recorded audio                                                     |                                                                                  |
|Bits per sample                    |Number of bits used for encoding each audio sample                                  |                                                                                  |
|Age coverage                       |Is meta-data about speaker age present?                                             |Percent                                                                           |
|Age balanced                       |                                                                                    |description                                                                       |

## Limitations
