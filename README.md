For an intro to Docker images for R see https://jsta.github.io/r-docker-tutorial/

### Setup Notes
Pull base image
```
docker pull rocker/geospatial:4.3.1
```

Start image (don't forget to replace brackets \<like this\>)
```
docker run --rm \
--name geospatial-tutorial \
-p 8787:8787 \ 
-e PASSWORD=<YOUR-PASSWORD> \
-v <PATH-TO-LOCAL-REPO>/Geospatial-Tutorial:/home/rstudio/ \
rocker/geospatial:4.3.1
```

Navigate to http://localhost:8787
```
user: rstudio
password: <YOUR PASSWORD>
```
