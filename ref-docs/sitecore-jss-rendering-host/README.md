@sitecore-jss/sitecore-jss-rendering-host

# @sitecore-jss/sitecore-jss-rendering-host

## Table of contents

### Functions

- [getDefaultAppInvocationInfoResolver](README.md#getdefaultappinvocationinforesolver)
- [ssrMiddleware](README.md#ssrmiddleware)
- [startRenderHostTunnel](README.md#startrenderhosttunnel)
- [startRenderingHostServer](README.md#startrenderinghostserver)

## Functions

### getDefaultAppInvocationInfoResolver

▸ **getDefaultAppInvocationInfoResolver**(`baseAppPath?`): `AppInvocationInfoResolver`

Returns the default AppInvocationInfoResolver, which is responsible for resolving the function, within your app bundle,
that should be invoked for rendering your app.

By default, the resolver assumes a folder structure of:
`./{baseAppPath}/{JSSAppName}/{serverBundleName}.js`

`JSSAppName` is the `id` property of the JSON request body that is POSTed to the rendering host by Sitecore.

`serverBundleName` is the name of the JavaScript file (typically a bundle) that contains the function for rendering your app.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `baseAppPath?` | `Object` | The base path to your JSS app(s), defaults to `./dist` |

#### Returns

`AppInvocationInfoResolver`

resolver

#### Defined in

[defaultAppInvocationInfoResolver.ts:19](https://github.com/Sitecore/jss/blob/e0c62f529/packages/sitecore-jss-rendering-host/src/defaultAppInvocationInfoResolver.ts#L19)

___

### ssrMiddleware

▸ **ssrMiddleware**(`options`): `WebServerMiddleware`

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `SSRMiddlewareOptions` |

#### Returns

`WebServerMiddleware`

#### Defined in

[ssrMiddleware.ts:41](https://github.com/Sitecore/jss/blob/e0c62f529/packages/sitecore-jss-rendering-host/src/ssrMiddleware.ts#L41)

___

### startRenderHostTunnel

▸ **startRenderHostTunnel**(`renderHostname`, `options?`): `Promise`\<`string`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `renderHostname` | `string` |
| `options` | `Options` |

#### Returns

`Promise`\<`string`\>

#### Defined in

[tunnel.ts:12](https://github.com/Sitecore/jss/blob/e0c62f529/packages/sitecore-jss-rendering-host/src/tunnel.ts#L12)

___

### startRenderingHostServer

▸ **startRenderingHostServer**(`config`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `config` | `RenderingHostServerOptions` |

#### Returns

`void`

#### Defined in

[renderingHostServer.ts:47](https://github.com/Sitecore/jss/blob/e0c62f529/packages/sitecore-jss-rendering-host/src/renderingHostServer.ts#L47)
