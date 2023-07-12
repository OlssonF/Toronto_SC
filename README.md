# Forecasting short-course casestudy example

Vignette for running a WQ forecast using NEON data.

## Running the vignette
We will use a Docker container to ensure a consistent R environment when running the vignette. The docker container already contains the packages needed to run the vignette. 

### Installing Docker
Go to [https://docs.docker.com/get-docker/](https://docs.docker.com/get-docker/) to install the relevant install for your platform (available for PC, Mac and Linux). Also see [https://docs.docker.com/desktop/](https://docs.docker.com/desktop/).

### Running a docker container

1. Launch Docker. 
2. At the command line run the following
```
docker run --rm -ti -e PASSWORD=yourpassword -p 8787:8787 eco4cast/rocker-neon4cast
```
This can take a few minutes to download and install. 

3. Open up a web browser and navigate to `http://localhost:8787/`
4. Enter the username: `rstudio` and password: `yourpassword`
5. You should see a R Studio interface with all the packages etc. pre-installed and ready to go.

You can close this localhost window but if you close the container any changes will be lost unless you push them to Github

If you are _NOT_ running a Docker container then you will need to install the packages and the JAGS executable manually (see instructions in the vignette).

### Clone or fork the github repository

Cloning the repository to this container will not allow you to save and push any changes back and all modifications will be lost when the container is closed so it is recommended to fork and push to your own branch. 

