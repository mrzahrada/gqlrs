# gqlrs
Client library which handles connection to GraphQL server, local caching, optimistic updates and local mutations

## GraphQL client

## Caching
gqlrs caches data received from the server for any type which implements Node interface. User should be allowed to defined what data should be invalidated for each mutation. 

## Optimistic updates
Optimistic update calls callback, which can update cache locally without waiting for the server update. if error is received, onError callback is called. if different data is received, data are updated in the cache

## local mutations
user can use local mutations to store any data locally which are then accessible with queries from all components

