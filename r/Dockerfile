FROM rocker/r-ver:4.1.3
WORKDIR /usr/src/app

RUN R  -e 'install.packages("remotes")'

COPY . ./

RUN R -e 'remotes::install_deps()'

CMD R -e 'source("app.R")'

