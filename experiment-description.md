This file documents the structure and meaning of experiment descriptions as the (abstract) template for experiments performed with the LabChain system.

An experiment description contains the prosumers and market design of the experiments, as well as description of the experiment, its length and its id.

Their structure is detailed in the following:

* prosumers: [{
  * id: number,
  * name?: string,
  * coordinates: {lat: number, lon: number},
  * startTokens: number,
  * assets: {
    * loads: [],
    * controllableGenerators: [],
    * noncontrollableGenerators: [],
    * storageUnits: [ ]}}]
* p2pMarketDesign: {
  * bidClosure: number
  * askClosure: number
  * timeSliceLength: number
  * minBidSize: number
  * minAskSize: number
  * maxPrice: number
  * feeAmount: number }
* description: string,
* experimentLength: number,
* id: string

