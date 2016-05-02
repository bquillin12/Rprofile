
options(stringAsFactors = FALSE)
options(width = 90)
options(digits = 2)

# R interactive prompt
options(prompt = "R: ")

# puts a timestamp in my command history (stolen from Tony Fischetti)
.First <- function(){
if(interactive()){
library(utils)
library(Quandl)
Quandl.auth("#####")
cat("\Successfully loaded Rprofile at", date(), "\n")
}
}

# saving interactive command history (also stolen from Tony Fischetti)
.Last <- function(){
if(interactive()){
hist_file <- Sys.getenv("R_HISTFILE")
if(hist_file=="") hist_file <- "~/.RHistory"
cat("\nGoodbye at ", date(), "\n")
}
}

# surpress package imports messages
quiet <- function(a.package){
suppressWarnings(suppressPackageStartupMessages(
library(a.package, character.only = TRUE)))
}

## Strip row names from a data frame (stolen from plyr)
.env$unrowname <- function(x) {
    rownames(x) <- NULL
    x
}

# Plotly authentication API keys
Sys.setenv("plotly_username"="xyz")
Sys.setenv("plotly_api_key"="xyz")

