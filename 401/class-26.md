# GraphQL @connection

## Directives

The Amplify CLI provides GraphQL directives to enhance your schema with additional capabilities such as custom indexes, authorization rules, function triggers.


## Amplify-provided directives

* @model: Defines top level object types in your API that are backed by Amazon DynamoDB
* @key: Configures custom index structures for @model types
* @auth: Defines authorization rules for your @model types and fields
* @connection: Defines 1:1, 1:M, and N:M relationships between @model types
* @function: Configures a Lambda function resolvers for a field
* @http: Configures an HTTP resolver for a field
* @predictions: Queries an orchestration of AI/ML services such as Amazon Rekognition, Amazon Translate, and/or Amazon Polly
* @searchable: Makes your data searchable by streaming it to Amazon OpenSearch
* @versioned: Defines the versioning and conflict resolution strategy for an @model type

## AWS AppSync-provided directives

The following directives are supported by the AppSync service and can be used within the Amplify GraphQL schemas. 

* @aws_api_key
* @aws_iam
* @aws_oidc
* @aws_cognito_user_pools
* @aws_auth
* @aws_subscribe

## 3rd party directives

* @algolia
* @ttl
* @firehose
* @retain