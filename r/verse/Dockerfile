FROM rocker/verse:3.6.2

LABEL maintainer="apoirel@ucsc.edu"
LABEL description="Used as a base for Popper workflows using R and rstudio"
# labels match the corresponding Rocker image
LABEL version="3.6.2"

# move configuration file where rstudio server will find it
COPY rsession.conf /etc/rstudio 

# install containerit
RUN R -e "devtools::install_github(\"o2r-project/containerit\")"
 
EXPOSE 8787
CMD ["bin/sh"] 