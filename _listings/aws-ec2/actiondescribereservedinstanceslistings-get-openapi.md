---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Describe Reserved Instances Listings
  version: 1.0.0
  description: Describes your account's Reserved Instance listings in the Reserved
    Instance Marketplace.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CancelReservedInstancesListing:
    get:
      summary: Cancel Reserved Instances Listing
      description: Cancels the specified Reserved Instance listing in the Reserved
        Instance Marketplace.
      operationId: cancelreservedinstanceslisting
      x-api-path-slug: actioncancelreservedinstanceslisting-get
      parameters:
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure idempotency
          of yourlistings
        type: string
      - in: query
        name: InstanceCount
        description: The number of instances that are a part of a Reserved Instance
          account to be listed in the Reserved Instance Marketplace
        type: string
      - in: query
        name: PriceSchedules.N
        description: A list specifying the price of the Standard Reserved Instance
          for each month remaining in the Reserved Instance term
        type: string
      - in: query
        name: ReservedInstancesId
        description: The ID of the active Standard Reserved Instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instance
  /?Action=CreateReservedInstancesListing:
    get:
      summary: Create Reserved Instances Listing
      description: "Creates a listing for Amazon EC2 Standard Reserved Instances to
        be sold in the Reserved Instance\n\t\t\tMarketplace."
      operationId: createreservedinstanceslisting
      x-api-path-slug: actioncreatereservedinstanceslisting-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: OfferingClass
        description: Describes whether the Reserved Instance is Standard or Convertible
        type: string
      - in: query
        name: OfferingType
        description: The Reserved Instance offering type
        type: string
      - in: query
        name: ReservedInstancesId.N
        description: One or more Reserved Instance IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instance
  /?Action=DescribeReservedInstancesListings:
    get:
      summary: Describe Reserved Instances Listings
      description: Describes your account's Reserved Instance listings in the Reserved
        Instance Marketplace.
      operationId: describereservedinstanceslistings
      x-api-path-slug: actiondescribereservedinstanceslistings-get
      parameters:
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: NextToken
        description: The token to retrieve the next page of results
        type: string
      - in: query
        name: ReservedInstancesModificationId.N
        description: IDs for the submitted modification request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instances
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---