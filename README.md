# IbanPlus
IbanPlus Solution Proposal

## IbanPlus.Importer.Func

Duralable Function app, lightweight app, function will call into the Importer.Service layer

## IbanPlus.Importer.Service

This is the code where the ImportManager will live this will control how an import takes place.
This is also the code that will call into SWIFT to download the files and unpacks them. 

## IbanPlus.Models

This is the project where the Models live that get used by the solution

## IbanPlus.Repository

This is the layer that controls how we access the data (read and write) it will also contain the code that controls DB Model --> App Model and back. (Transformers) This code connects to the Storage.SQL layer. Service layer has does not need to know what we access. 

## IbanPlus.Storage.SQL

This is the layer where we control how to access the Database.

## IbanPlus.Web.API

This is the layer that get's used by clients who want to use the API layer of IbanPlus

## IbanPlus.Core

Core utlities layer that will contain code that could be shared between projects. (When we start adding in )