# 0x00. GraphQL - Episode Retrieval

## Objective

The goal of this part of the project is to demonstrate the ability to write a GraphQL query to retrieve the specific details of an episode using its ID. This task utilizes the `episode(id: ID!)` field on the endpoint.

## Files

The following files contain the GraphQL queries and their expected JSON output for episode IDs 1, 2, 3, and 4:

* `episode-id-1.graphql`
* `episode-id-1-output.json`
* `episode-id-2.graphql`
* `episode-id-2-output.json`
* `episode-id-3.graphql`
* `episode-id-3-output.json`
* `episode-id-4.graphql`
* `episode-id-4-output.json`

## GraphQL Query Structure

All `.graphql` files contain a query that fetches the `id`, `name`, `air_date`, and `episode` code for a specific episode by passing the ID as an argument to the `episode` field.

The general query format is:

```graphql
query {
  episode(id: "YOUR_ID_HERE") {
    id
    name
    air_date
    episode
  }
}