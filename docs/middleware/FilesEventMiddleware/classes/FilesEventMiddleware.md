[**Node Adapter Documentation v0.0.2**](../../../README.md)

***

[Node Adapter Documentation](../../../modules.md) / [middleware/FilesEventMiddleware](../README.md) / FilesEventMiddleware

# Class: FilesEventMiddleware

Class representing a FilesEventMiddleware.

## Author

Mr. Stone <evensstone@gmail.com>

## Constructors

### new FilesEventMiddleware()

> **new FilesEventMiddleware**(`options`): [`FilesEventMiddleware`](FilesEventMiddleware.md)

Create a FilesEventMiddleware.

#### Parameters

##### options

Options for creating the FilesEventMiddleware.

###### blueprint

`IBlueprint`

#### Returns

[`FilesEventMiddleware`](FilesEventMiddleware.md)

#### Defined in

[src/middleware/FilesEventMiddleware.ts:24](https://github.com/stonemjs/node-adapter/blob/3c6d11fbb2b43efd2628228369562f77db66c88f/src/middleware/FilesEventMiddleware.ts#L24)

## Methods

### handle()

> **handle**(`context`, `next`): `Promise`\<[`ServerResponseWrapper`](../../../ServerResponseWrapper/classes/ServerResponseWrapper.md)\>

Handles the incoming event, processes it, and invokes the next middleware in the pipeline.

#### Parameters

##### context

[`NodeHttpAdapterContext`](../../../declarations/interfaces/NodeHttpAdapterContext.md)

The adapter context containing the raw event, execution context, and other data.

##### next

`NextPipe`\<[`NodeHttpAdapterContext`](../../../declarations/interfaces/NodeHttpAdapterContext.md), [`ServerResponseWrapper`](../../../ServerResponseWrapper/classes/ServerResponseWrapper.md)\>

The next middleware to be invoked in the pipeline.

#### Returns

`Promise`\<[`ServerResponseWrapper`](../../../ServerResponseWrapper/classes/ServerResponseWrapper.md)\>

A promise that resolves to the destination type after processing.

#### Throws

If required components such as the rawEvent or IncomingEventBuilder are not provided.

#### Defined in

[src/middleware/FilesEventMiddleware.ts:37](https://github.com/stonemjs/node-adapter/blob/3c6d11fbb2b43efd2628228369562f77db66c88f/src/middleware/FilesEventMiddleware.ts#L37)
