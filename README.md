# multialignet data export

The two zip files contained in the "/lrec_submission" directory contain the same data from two different sources:

  -   "multialignet_csv_data.zip" contains all the 1111 CSV files directly produced by the multialignet data ingestion system, so there's one CSV file 
      for each annotation process launched on a certain head MCk. Files are named in the following way: HeadMCkBabelNetSynsetCode_EnglishWordNetLemma_200.csv .
      Files are divided into 4 subfolders: 
        - "/semcor_freqh" contains 750 files generated using as head MCk senses amongst the most frequent senses that occur in the SemCor corpus (common senses).
        - "/semcor_freq1_polis1" contains 200 files generated using as head MCk monosemic terms that occur only one time in the SemCor corpus (rare senses).
        - "/basic_vocab" contains 100 files generated using as head MCk concepts found by inspecting basic vocabularies of each of the three languages.
        - "/terms_allsynsets" contains 61 files generated using as head MCk randomly-picked polysemous terms referring to exactly 61 senses.

  -   "multialignet_neo4j_export_json.zip" contains the JSON file with the Neo4j apoc.export.json.all export. It can be imported on Neo4j or on other NoSQL DBMSs.
