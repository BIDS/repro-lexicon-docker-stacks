# To build the container, cd to the location of the docker-stacks:

```
cd /path/to/repro-lexicon-docker-stacks/container
docker build --rm --tag wip-repro-lexicon .
```


# To run the container, cd to the location of your Jupyter notebooks repo:

```
cd /path/to/repro-lexicon-analysis-public
```

```
docker run --name wip -p 8888:8888 -v $(pwd):/home/jovyan/work -d wip-repro-lexicon
```

Get the secure token using:

```
docker logs wip
```
NB: Linux users add ```sudo``` before all these commands.
