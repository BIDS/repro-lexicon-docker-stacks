# To run the container, cd to the location of your Jupyter notebooks:

`cd /path/to/repro-lexicon-analysis-public`

```
docker run --name wip -p 8888:8888 -v $(pwd):/home/jovyan/work -d wip-lexicon
```

Get the secure token using:

```
docker logs wip
```
