# 0x00. GraphQL - Character Retrieval

## Objective

The goal of this project is to demonstrate the ability to write a GraphQL query to retrieve a specific character's information using their ID. This task utilizes the `character(id: ID!)` field available on a public GraphQL endpoint (e.g., The Rick and Morty API).

## Files

The following files contain the GraphQL queries and their expected JSON output for character IDs 1, 2, 3, and 4:

* `character-id-1.graphql`
* `character-id-1-output.json`
* `character-id-2.graphql`
* `character-id-2-output.json`
* `character-id-3.graphql`
* `character-id-3-output.json`
* `character-id-4.graphql`
* `character-id-4-output.json`

## GraphQL Query Structure

All `.graphql` files contain a query that fetches the `id`, `name`, `status`, `species`, `type`, and `gender` for a specific character by passing the ID as an argument to the `character` field.

The general query format is:

```graphql
query {
  character(id: "YOUR_ID_HERE") {
    id
    name
    status
    species
    type
    gender
  }
}


### **B. GraphQL Query Files**

The query is the same for all IDs, only the value of the `id` argument changes.

#### **`character-id-1.graphql`**

```graphql
query {
  character(id: "1") {
    id
    name
    status
    species
    type
    gender
  }
}