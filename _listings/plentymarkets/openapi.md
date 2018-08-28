swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/customer_contracts/{contractId}/document:
    get:
      summary: Starts download of contract document
      description: Starts download of contract document.
      operationId: getRestCustomerContractsContractDocument
      x-api-path-slug: restcustomer-contractscontractiddocument-get
      parameters:
      - in: path
        name: contractId
      responses:
        200:
          description: OK
      tags:
      - Starts
      - Download
      - Of
      - Contract
      - Document
  /rest/customer_contracts/{contractId}/sign/document:
    get:
      summary: Starts download of signed contract document
      description: Starts download of signed contract document.
      operationId: getRestCustomerContractsContractSignDocument
      x-api-path-slug: restcustomer-contractscontractidsigndocument-get
      parameters:
      - in: path
        name: contractId
      responses:
        200:
          description: OK
      tags:
      - Starts
      - Download
      - Of
      - Signed
      - Contract
      - Document
  /rest/listings/markets/start/{id?}:
    post:
      summary: Start the market listing on the designated market.
      description: Starts the market listing on the designated markets.
      operationId: postRestListingsMarketsStart
      x-api-path-slug: restlistingsmarketsstartid-post
      parameters:
      - in: query
        name: distribution
        description: The number of minutes that the listing should be started
      - in: query
        name: id
        description: The ID of the listing market that needs to be started
      - in: path
        name: id?
      - in: query
        name: startAt
        description: When should the listings be started
      responses:
        200:
          description: OK
      tags:
      - Start
      - Market
      - Listing
      - "On"
      - Designated
      - Market