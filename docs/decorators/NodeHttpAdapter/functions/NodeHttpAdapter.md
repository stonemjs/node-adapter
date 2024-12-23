[**Node Adapter Documentation v0.0.2**](../../../README.md)

***

[Node Adapter Documentation](../../../modules.md) / [decorators/NodeHttpAdapter](../README.md) / NodeHttpAdapter

# Function: NodeHttpAdapter()

> **NodeHttpAdapter**\<`T`\>(`options`): (`target`, `context`) => `void`

A class decorator for registering a Node.js HTTP adapter in the Stone.js framework.

The decorator modifies the `nodeHttpAdapterBlueprint` by merging the provided options
with the default configuration. It also registers the blueprint to the target class using
the `addBlueprint` utility.

## Type Parameters

• **T** *extends* `ClassType` = `ClassType`

The type of the class being decorated, defaulting to `ClassType`.

## Parameters

### options

[`NodeHttpAdapterOptions`](../interfaces/NodeHttpAdapterOptions.md) = `{}`

An object containing configuration options for the Node.js HTTP adapter.

## Returns

`Function`

A class decorator function.

### Parameters

#### target

`T`

#### context

`ClassDecoratorContext`\<`T`\>

### Returns

`void`

## Example

```typescript
import { NodeHttpAdapter } from '@stone-js/node-http';

@NodeHttpAdapter({
  url: 'http://localhost:3000',
  default: true,
})
class MyHttpService {
  // Service implementation
}
```

## Defined in

[src/decorators/NodeHttpAdapter.ts:38](https://github.com/stonemjs/node-http-adapter/blob/c40d3860d098a79d7e93912b877b62d235dc0a99/src/decorators/NodeHttpAdapter.ts#L38)
