```python

#### Install dataset in local  ###########################
    cd webapi/asearch

    mkdir -p ztmp     ### ztmp is always in gitignore, you can install inside the repo

    cd ztmp/
    git clone  https://github.com/arita37/data2.git data

    cd data && git checkout text
    ls .



#### you need to instal git Large Ffile to handle large file commit.
        brew install git-lfs
        sudo apt-get install git-lfs


        cd ./ztmp/data/ && 
        git lfs install



#### Folder structure

   ######### classification Tasks   ######################
   cats/ 
       ag_news/ : News Dataset
           train/:   "text", "label"
           test/:    "text", "label"

       arxiv/
           raw/ :    raw file from itnernet
           train/ :  train split normalized
           val/:     val split normalized
           meta/meta.json:   Dict with encoding mapping for Label,s...

        "text_id": 
        "text" : str
        "labels":   "," separated labels


   ######### NER Tasks   ################################
   ner/
      ner_geo:  Location NER datasets

      legaldoc:  Legal dataset
         raw/:  TRAIN.json.zip   JSON records training data
                TEST.json.zip    JSON records training data

         train/df.parquet : parquet format
         train/df.parquet : parquet format

        "text_id": 
        "text" : str
        "ner_list":  list of dict{ "start", "end"  }






```
