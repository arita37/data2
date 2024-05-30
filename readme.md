```python
#### Folder strucyture

   cats/ 
       ag_news : News Dataset


       arxiv/
           raw/ :    raw file from itnernet
           train/ :  train split normalized
           val/:     val split normalized
           meta/meta.json:   Dict with encoding mapping for Label,s...


#### Install dataset in local
    cd webapi/asearch

    mkdir -p ztmp     ### ztmp is always in gitignore, you can install inside the repo

    cd ztmp/
    git clone  https://github.com/arita37/data2.git data

    cd data && git checkout text
    ls .



#### you need to instal git Large Ffile
        brew install git-lfs
        sudo apt-get install git-lfs

        cd ./ztmp/data/ && 
        git lfs install




#### data are ready to use




```
