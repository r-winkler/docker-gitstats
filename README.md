# gitstats 

This is a gitstats container based on ubuntu image. 

The following software is installed:

* gitstats
* Python
* Gnuplot
	

## Usage

```
1) go to docker settings via icon in taskbar and share c drive 
2) connect to server (see below)
3) cd repos
4) gitstats my_repo outputfolder
5) open index.html
```

## Build

```
docker build . -t gitstats
```


## Launch

```
docker run -itd -v C:/dev/repos:/repos --name gitstats renewinkler/gitstats
```


## Connect to Server

```
docker exec -it gitstats /bin/bash
```