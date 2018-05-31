# Retrieval-Infomation
Website Search Engine with Solr  

## Requirements
- Solr 6.6 or higher 


## Config Solr:
- Create core:
```
~/solr/bin/solr start
~/solr/bin/solr create -c IT4853
```
 - Add field to indexing
 ```
Core Selector --> IT4853 --> Schema --> Add copy field: Sorce: *  / destination: _text_
==> Add CopyField
```
- Query with Vietnamese:
+ Using **Folding Filter**: setting var **preserveOriginal(Boolean)**
If boolean=true : "thé" -> "the", "thé".
- Add file stopword for vi: **stopwords_vi.txt(390 words)**

## Import data 
- Data: nhom8_export.json
- Access : http://localhost:8983 and import data 

## Start app
- Open index.html
-----------------------
