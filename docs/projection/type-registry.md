# Projection Type Registry

A projection type registry is bound to `MsgPhp\Domain\Projection\ProjectionTypeRegistry`. Its purpose is to manage all
available [projection](models.md) type information.

## API

### `initialize(string ...$type): void`

Initializes the registry. Usually needs to be called only once per environment, or after any type information has
changed.

### `destroy(string ...$type): void`

Destroys the registry and thus requires to be re-initialized after.

## Implementations

### Infrastructural

- [Elasticsearch](../infrastructure/elasticsearch.md#projection-type-registry)
