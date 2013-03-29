# NetDNA REST Web Services NET Client

This is a Visual Studio 2012 project using .NET 4.5 

Make sure and obtain a proper account alias, consumer key, and consumer secret prior to using this library

## Usage

`var api = new NetDNARWS.Api("account alais", "consumer key","consumer secret");`

`var accountResult = api.Get("/account.json")`

## Methods
It has support for `GET` `DELETE` `PUT` & `POST` requests only at the moment

Every request can take an optional debug parameter which will write all objects returned to the console.

## GET
`var accountResult = api.Get("/account.json", true)`

## DELETE (Purge Cache)
`api.Delete("/zones/pull.json/" + pullZone.id + "/cache?file=" + pathToFile)`

