# OML Template

[![Gitpod](https://img.shields.io/badge/gitpod-open-blue?logo=gitpod)](https://gitpod.io/#https://github.com/opencaesar/oml-template) 
[![Build Status](https://travis-ci.org/opencaesar/oml-template.svg?branch=master)](https://travis-ci.org/opencaesar/oml-template)
[![Documentation](https://img.shields.io/badge/Documentation-HTML-orange)](https://opencaesar.github.io/oml-template/) 

This repository has a template [OML](https://github.com/opencaesar/oml) project. It is meant to be forked as a starting point by pressing the 'Use this template' button above.

## Clone
```
  git clone https://github.com/opencaesar/oml-template.git
  cd oml-template
```

## Build
Equivalent to owlReason task
```
./gradlew build
```

## Generate Docs
You must first have Bikeshed (the app itself) installed from [here](https://tabatkins.github.io/bikeshed/#install-final)
```
./gradlew generateDocs
```
Note: if bikeshed is not in the PATH, you can add -pBIKESHED=path/to/bikeshed argument

## Run OWL Reasoner
```
./gradlew owlReason
```

## Start Fuseki Server
```
./gradlew startFuseki
```

## Stop Fuseki Server
```
./gradlew stopFuseki
```

## Load to Fuseki Dataset
```
./gradlew owlLoad
```
Pre-req: A Fuseki server with a firesat dataset must be running at http://localhost:3030/firesat (see below)  

## Run SPARQL Queries
```
./gradlew owlQuery
```
Pre-req: A Fuseki server with a firesat dataset must be running at http://localhost:3030/firesat (see below)  

## Run SHACL Rules
```
./gradlew owlShacl
```
Pre-req: A Fuseki server with a firesat dataset must be running at http://localhost:3030/firesat (see below) 

## Publish to Maven Local
```
./gradlew publishToMavenLocal
```
