[@sitecore-jss/sitecore-jss-nextjs](../README.md) / [editing](../modules/editing.md) / BasicEditingDataServiceConfig

# Interface: BasicEditingDataServiceConfig

[editing](../modules/editing.md).BasicEditingDataServiceConfig

## Table of contents

### Properties

- [editingDataCache](editing.BasicEditingDataServiceConfig.md#editingdatacache)

## Properties

### editingDataCache

• `Optional` **editingDataCache**: [`EditingDataCache`](editing.EditingDataCache.md)

An instance of the `EditingDataCache` implementation to use.
By default, this is `editingDataDiskCache` (an `EditingDataDiskCache` singleton).

**`Default`**

```ts
editingDataDiskCache
```

**`See`**

 - EditingDataCache
 - EditingDataDiskCache

#### Defined in

[sitecore-jss-nextjs/src/editing/editing-data-service.ts:63](https://github.com/Sitecore/jss/blob/e0c62f529/packages/sitecore-jss-nextjs/src/editing/editing-data-service.ts#L63)
