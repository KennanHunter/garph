[garph](../index.md) / GarphSchema

# Class: GarphSchema

## Constructors

### constructor

• **new GarphSchema**(`«destructured»?`)

#### Parameters

| Name             | Type                               |
| :--------------- | :--------------------------------- |
| `«destructured»` | `Object`                           |
| › `types`        | [`AnyType`](../index.md#anytype)[] |

#### Defined in

[index.ts:618](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L618)

## Properties

### nodeType

• **nodeType**: `GInterface`<`"Node"`, { `id`: `GString`<`"ID"`\> }\>

#### Defined in

[index.ts:600](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L600)

---

### pageInfoArgs

• **pageInfoArgs**: `Object`

#### Type declaration

| Name     | Type                              |
| :------- | :-------------------------------- |
| `after`  | `GOptional`<`GString`<`"ID"`\>\>  |
| `before` | `GOptional`<`GString`<`"ID"`\>\>  |
| `first`  | `GOptional`<`GNumber`<`"Int"`\>\> |
| `last`   | `GOptional`<`GNumber`<`"Int"`\>\> |

#### Defined in

[index.ts:611](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L611)

---

### pageInfoType

• **pageInfoType**: `GType`<`"PageInfo"`, { `endCursor`: `GOptional`<`GString`<`"String"`\>\> ; `hasNextPage`: `GBoolean` ; `hasPreviousPage`: `GBoolean` ; `startCursor`: `GOptional`<`GString`<`"String"`\>\> }\>

#### Defined in

[index.ts:604](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L604)

---

### types

• **types**: [`AnyType`](../index.md#anytype)[] = `[]`

#### Defined in

[index.ts:599](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L599)

## Methods

### boolean

▸ **boolean**(): `GBoolean`

#### Returns

`GBoolean`

#### Defined in

[index.ts:703](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L703)

---

### connection

▸ **connection**<`N`, `T`\>(`name`, `shape`): `GType`<`string`, { `edges`: `GList`<`T`\> ; `pageInfo`: `GType`<`"PageInfo"`, { `endCursor`: `GOptional`<`GString`<`"String"`\>\> ; `hasNextPage`: `GBoolean` ; `hasPreviousPage`: `GBoolean` ; `startCursor`: `GOptional`<`GString`<`"String"`\>\> }\> }\>

#### Type parameters

| Name | Type                                            |
| :--- | :---------------------------------------------- |
| `N`  | extends `string`                                |
| `T`  | extends [`Type`](Type.md)<`any`, `"Ref"`, `T`\> |

#### Parameters

| Name    | Type |
| :------ | :--- |
| `name`  | `N`  |
| `shape` | `T`  |

#### Returns

`GType`<`string`, { `edges`: `GList`<`T`\> ; `pageInfo`: `GType`<`"PageInfo"`, { `endCursor`: `GOptional`<`GString`<`"String"`\>\> ; `hasNextPage`: `GBoolean` ; `hasPreviousPage`: `GBoolean` ; `startCursor`: `GOptional`<`GString`<`"String"`\>\> }\> }\>

#### Defined in

[index.ts:634](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L634)

---

### edge

▸ **edge**<`N`, `T`\>(`name`, `shape`): `GType`<`N`, { `cursor`: [`AnyString`](../index.md#anystring) ; `node`: `T` }\>

#### Type parameters

| Name | Type                                            |
| :--- | :---------------------------------------------- |
| `N`  | extends `string`                                |
| `T`  | extends [`Type`](Type.md)<`any`, `"Ref"`, `T`\> |

#### Parameters

| Name    | Type |
| :------ | :--- |
| `name`  | `N`  |
| `shape` | `T`  |

#### Returns

`GType`<`N`, { `cursor`: [`AnyString`](../index.md#anystring) ; `node`: `T` }\>

#### Defined in

[index.ts:644](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L644)

---

### enumType

▸ **enumType**<`N`, `T`\>(`name`, `args`): `GEnum`<`N`, `T`\>

#### Type parameters

| Name | Type                                        |
| :--- | :------------------------------------------ |
| `N`  | extends `string`                            |
| `T`  | extends readonly `string`[] \| `TSEnumType` |

#### Parameters

| Name   | Type |
| :----- | :--- |
| `name` | `N`  |
| `args` | `T`  |

#### Returns

`GEnum`<`N`, `T`\>

#### Defined in

[index.ts:663](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L663)

---

### float

▸ **float**(): `GNumber`<`"Float"`\>

#### Returns

`GNumber`<`"Float"`\>

#### Defined in

[index.ts:699](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L699)

---

### id

▸ **id**(): `GString`<`"ID"`\>

#### Returns

`GString`<`"ID"`\>

#### Defined in

[index.ts:691](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L691)

---

### inputType

▸ **inputType**<`N`, `T`\>(`name`, `shape`): `GInput`<`N`, `T`\>

#### Type parameters

| Name | Type                                       |
| :--- | :----------------------------------------- |
| `N`  | extends `string`                           |
| `T`  | extends [`AnyTypes`](../index.md#anytypes) |

#### Parameters

| Name    | Type |
| :------ | :--- |
| `name`  | `N`  |
| `shape` | `T`  |

#### Returns

`GInput`<`N`, `T`\>

#### Defined in

[index.ts:657](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L657)

---

### int

▸ **int**(): `GNumber`<`"Int"`\>

#### Returns

`GNumber`<`"Int"`\>

#### Defined in

[index.ts:695](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L695)

---

### interface

▸ **interface**<`N`, `T`\>(`name`, `shape`): `GInterface`<`N`, `T`\>

#### Type parameters

| Name | Type                                       |
| :--- | :----------------------------------------- |
| `N`  | extends `string`                           |
| `T`  | extends [`AnyTypes`](../index.md#anytypes) |

#### Parameters

| Name    | Type |
| :------ | :--- |
| `name`  | `N`  |
| `shape` | `T`  |

#### Returns

`GInterface`<`N`, `T`\>

#### Defined in

[index.ts:681](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L681)

---

### node

▸ **node**<`N`, `T`\>(`name`, `shape`): `GType`<`N`, `T` & { `id`: `GString`<`"ID"`\> }\>

#### Type parameters

| Name | Type                                       |
| :--- | :----------------------------------------- |
| `N`  | extends `string`                           |
| `T`  | extends [`AnyTypes`](../index.md#anytypes) |

#### Parameters

| Name    | Type |
| :------ | :--- |
| `name`  | `N`  |
| `shape` | `T`  |

#### Returns

`GType`<`N`, `T` & { `id`: `GString`<`"ID"`\> }\>

#### Defined in

[index.ts:628](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L628)

---

### ref

▸ **ref**<`T`\>(`ref`): `GRef`<`T`\>

#### Type parameters

| Name |
| :--- |
| `T`  |

#### Parameters

| Name  | Type |
| :---- | :--- |
| `ref` | `T`  |

#### Returns

`GRef`<`T`\>

#### Defined in

[index.ts:709](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L709)

---

### scalarType

▸ **scalarType**<`I`, `O`\>(`name`, `options?`): `GScalar`<`I`, `O`\>

#### Type parameters

| Name |
| :--- |
| `I`  |
| `O`  |

#### Parameters

| Name       | Type                       |
| :--------- | :------------------------- |
| `name`     | `string`                   |
| `options?` | `ScalarOptions`<`I`, `O`\> |

#### Returns

`GScalar`<`I`, `O`\>

#### Defined in

[index.ts:675](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L675)

---

### string

▸ **string**(): `GString`<`"String"`\>

#### Returns

`GString`<`"String"`\>

#### Defined in

[index.ts:687](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L687)

---

### type

▸ **type**<`N`, `T`\>(`name`, `shape`): `GType`<`N`, `T`\>

#### Type parameters

| Name | Type                                       |
| :--- | :----------------------------------------- |
| `N`  | extends `string`                           |
| `T`  | extends [`AnyTypes`](../index.md#anytypes) |

#### Parameters

| Name    | Type |
| :------ | :--- |
| `name`  | `N`  |
| `shape` | `T`  |

#### Returns

`GType`<`N`, `T`\>

#### Defined in

[index.ts:622](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L622)

---

### unionType

▸ **unionType**<`N`, `T`\>(`name`, `args`): `GUnion`<`N`, `T`\>

#### Type parameters

| Name | Type                                           |
| :--- | :--------------------------------------------- |
| `N`  | extends `string`                               |
| `T`  | extends [`AnyObjects`](../index.md#anyobjects) |

#### Parameters

| Name   | Type |
| :----- | :--- |
| `name` | `N`  |
| `args` | `T`  |

#### Returns

`GUnion`<`N`, `T`\>

#### Defined in

[index.ts:669](https://github.com/stepci/garph/blob/3c68aab/src/index.ts#L669)
