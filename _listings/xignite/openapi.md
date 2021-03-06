swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetMasterByIdentifier:
    get:
      summary: Get Master By Identifier
      description: Get master records by identifier.
      operationId: GetMasterByIdentifier
      x-api-path-slug: getmasterbyidentifier-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Identifier
  /GetMasterByIdentifiers:
    get:
      summary: Get Master By Identifiers
      description: Get master records by identifiers.
      operationId: GetMasterByIdentifiers
      x-api-path-slug: getmasterbyidentifiers-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Identifiers
  /GetMasterByExchange:
    get:
      summary: Get Master By Exchange
      description: Get master records by exchange.
      operationId: GetMasterByExchange
      x-api-path-slug: getmasterbyexchange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Exchange
  /GetMasterByExchangeChanges:
    get:
      summary: Get Master By Exchange Changes
      description: Get a master record by exchange and the last modified since date
      operationId: GetMasterByExchangeChanges
      x-api-path-slug: getmasterbyexchangechanges-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Exchange
      - Changes
  /GetMasterBySector:
    get:
      summary: Get Master By Sector
      description: Old version of the service. Customers should use GetMasterByGlobalSector
      operationId: GetMasterBySector
      x-api-path-slug: getmasterbysector-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Sector
  /GetMasterByIndustry:
    get:
      summary: Get Master By Industry
      description: Old version of the service. Customers should use GetMasterByGlobalIndustry
      operationId: GetMasterByIndustry
      x-api-path-slug: getmasterbyindustry-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Industry
  /GetMasterByGlobalSector:
    get:
      summary: Get Master By Global Sector
      description: Get master records by sector.
      operationId: GetMasterByGlobalSector
      x-api-path-slug: getmasterbyglobalsector-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Global
      - Sector
  /GetMasterByGlobalIndustry:
    get:
      summary: Get Master By Global Industry
      description: Get master records by industry.
      operationId: GetMasterByGlobalIndustry
      x-api-path-slug: getmasterbyglobalindustry-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Global
      - Industry
  /GetMasterStatisticsByExchange:
    get:
      summary: Get Master Statistics By Exchange
      description: Get statistical information about exchanges.
      operationId: GetMasterStatisticsByExchange
      x-api-path-slug: getmasterstatisticsbyexchange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Statistics
      - Exchange