# SnarkyJS API Reference

To write a zkApp, we recommend using the [Mina zkApp CLI](https://github.com/o1-labs/zkApp-cli), which makes writing a zkApp easy by including SnarkyJS & providing project scaffolding, a test framework, and formatting.

## Table of contents

### References

- [PublicKey](#publickey)

### Namespaces

- [Encoding](#modulesencodingmd)
- [Encryption](#modulesencryptionmd)
- [Experimental](#modulesexperimentalmd)
- [Mina](#modulesminamd)
- [Types](#modulestypesmd)
- [ZkProgram](#moduleszkprogrammd)

### Classes

- [Bool](#classesboolmd)
- [Character](#classescharactermd)
- [Circuit](#classescircuitmd)
- [CircuitString](#classescircuitstringmd)
- [CircuitValue](#classescircuitvaluemd)
- [Field](#classesfieldmd)
- [Group](#classesgroupmd)
- [Int64](#classesint64md)
- [Keypair](#classeskeypairmd)
- [Ledger](#classesledgermd)
- [Party](#classespartymd)
- [PrivateKey](#classesprivatekeymd)
- [Proof](#classesproofmd)
- [Scalar](#classesscalarmd)
- [SelfProof](#classesselfproofmd)
- [Sign](#classessignmd)
- [Signature](#classessignaturemd)
- [SmartContract](#classessmartcontractmd)
- [Token](#classestokenmd)
- [UInt32](#classesuint32md)
- [UInt64](#classesuint64md)
- [VerificationKey](#classesverificationkeymd)

### Interfaces

- [AsFieldElements](#interfacesasfieldelementsmd)
- [Permissions](#interfacespermissionsmd)

### Type Aliases

- [DeployArgs](#deployargs)
- [State](#state)
- [ZkappPublicInput](#zkapppublicinput)

### Variables

- [Permissions](#permissions)
- [Poseidon](#poseidon)
- [ZkappPublicInput](#zkapppublicinput-1)
- [isReady](#isready)

### Functions

- [State](#state-1)
- [ZkProgram](#zkprogram)
- [addCachedAccount](#addcachedaccount)
- [arrayProp](#arrayprop)
- [circuitMain](#circuitmain)
- [circuitValue](#circuitvalue)
- [declareMethods](#declaremethods)
- [declareState](#declarestate)
- [deploy](#deploy)
- [fetchAccount](#fetchaccount)
- [fetchLastBlock](#fetchlastblock)
- [getSrs](#getsrs)
- [matrixProp](#matrixprop)
- [method](#method)
- [partiesToJson](#partiestojson)
- [prop](#prop)
- [public\_](#public_)
- [recoverVerificationKey](#recoververificationkey)
- [sendZkapp](#sendzkapp)
- [serializeVerificationKey](#serializeverificationkey)
- [setGraphqlEndpoint](#setgraphqlendpoint)
- [shutdown](#shutdown)
- [signFeePayer](#signfeepayer)
- [state](#state-2)
- [verify](#verify)

# Classes


<a name="classesboolmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Bool

## Class: Bool

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [Unsafe](#unsafe)

#### Methods

- [and](#and)
- [assertEquals](#assertequals)
- [assertFalse](#assertfalse)
- [assertTrue](#asserttrue)
- [equals](#equals)
- [not](#not)
- [or](#or)
- [sizeInFields](#sizeinfields)
- [toBoolean](#toboolean)
- [toField](#tofield)
- [toFields](#tofields)
- [toJSON](#tojson)
- [toString](#tostring)
- [and](#and-1)
- [assertEqual](#assertequal)
- [check](#check)
- [count](#count)
- [equal](#equal)
- [fromJSON](#fromjson)
- [not](#not-1)
- [ofFields](#offields)
- [or](#or-1)
- [sizeInFields](#sizeinfields-1)
- [toField](#tofield-1)
- [toFields](#tofields-1)
- [toInput](#toinput)
- [toJSON](#tojson-1)

### Constructors

#### constructor

• **new Bool**(`x`)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `boolean` \| [`Bool`](#classesboolmd) |

##### Defined in

[snarky.d.ts:363](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L363)

### Properties

#### Unsafe

▪ `Static` **Unsafe**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `ofField` | (`x`: `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd)) => [`Bool`](#classesboolmd) |

##### Defined in

[snarky.d.ts:443](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L443)

### Methods

#### and

▸ **and**(`y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `y` | `boolean` \| [`Bool`](#classesboolmd) | A [[`Bool`]] to AND with this [[`Bool`]]. |

##### Returns

[`Bool`](#classesboolmd)

a new [[`Bool`]] that is set to true only if
this [[`Bool`]] and `y` are also true.

##### Defined in

[snarky.d.ts:380](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L380)

___

#### assertEquals

▸ **assertEquals**(`y`): `void`

Proves that this [[`Bool`]] is equal to `y`.

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `y` | `boolean` \| [`Bool`](#classesboolmd) | a [[`Bool`]]. |

##### Returns

`void`

##### Defined in

[snarky.d.ts:393](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L393)

___

#### assertFalse

▸ **assertFalse**(): `void`

Proves that this [[`Bool`]] is `false`.

##### Returns

`void`

##### Defined in

[snarky.d.ts:403](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L403)

___

#### assertTrue

▸ **assertTrue**(): `void`

Proves that this [[`Bool`]] is `true`.

##### Returns

`void`

##### Defined in

[snarky.d.ts:398](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L398)

___

#### equals

▸ **equals**(`y`): [`Bool`](#classesboolmd)

Returns true if this [[`Bool`]] is equal to `y`.

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `y` | `boolean` \| [`Bool`](#classesboolmd) | a [[`Bool`]]. |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:409](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L409)

___

#### not

▸ **not**(): [`Bool`](#classesboolmd)

##### Returns

[`Bool`](#classesboolmd)

a new [[`Bool`]] that is the negation of this [[`Bool`]].

##### Defined in

[snarky.d.ts:373](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L373)

___

#### or

▸ **or**(`y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `y` | `boolean` \| [`Bool`](#classesboolmd) | a [[`Bool`]] to OR with this [[`Bool`]]. |

##### Returns

[`Bool`](#classesboolmd)

a new [[`Bool`]] that is set to true if either
this [[`Bool`]] or `y` is true.

##### Defined in

[snarky.d.ts:387](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L387)

___

#### sizeInFields

▸ **sizeInFields**(): `number`

##### Returns

`number`

##### Defined in

[snarky.d.ts:411](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L411)

___

#### toBoolean

▸ **toBoolean**(): `boolean`

This converts the [[`Bool`]] to a javascript [[boolean]].
This can only be called on non-witness values.

##### Returns

`boolean`

##### Defined in

[snarky.d.ts:429](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L429)

___

#### toField

▸ **toField**(): [`Field`](#classesfieldmd)

Converts a [[`Bool`]] to a [[`Field`]]. `false` becomes 0 and `true` becomes 1.

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:368](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L368)

___

#### toFields

▸ **toFields**(): [`Field`](#classesfieldmd)[]

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[snarky.d.ts:412](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L412)

___

#### toJSON

▸ **toJSON**(): `JSONValue`

Serialize the [[`Bool`]] to a JSON string.
This operation does NOT affect the circuit and can't be used to prove anything about the string representation of the Field.

##### Returns

`JSONValue`

##### Defined in

[snarky.d.ts:423](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L423)

___

#### toString

▸ **toString**(): `string`

Serialize the [[`Bool`]] to a string, e.g. for printing.
This operation does NOT affect the circuit and can't be used to prove anything about the string representation of the Field.

##### Returns

`string`

##### Defined in

[snarky.d.ts:418](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L418)

___

#### and

▸ `Static` **and**(`x`, `y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `boolean` \| [`Bool`](#classesboolmd) |
| `y` | `boolean` \| [`Bool`](#classesboolmd) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:454](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L454)

___

#### assertEqual

▸ `Static` **assertEqual**(`x`, `y`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `boolean` \| [`Bool`](#classesboolmd) |
| `y` | `boolean` \| [`Bool`](#classesboolmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:457](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L457)

___

#### check

▸ `Static` **check**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Bool`](#classesboolmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:469](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L469)

___

#### count

▸ `Static` **count**(`x`): [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `boolean`[] \| [`Bool`](#classesboolmd) |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:461](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L461)

___

#### equal

▸ `Static` **equal**(`x`, `y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `boolean` \| [`Bool`](#classesboolmd) |
| `y` | `boolean` \| [`Bool`](#classesboolmd) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:459](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L459)

___

#### fromJSON

▸ `Static` **fromJSON**(`x`): ``null`` \| [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `JSONValue` |

##### Returns

``null`` \| [`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:468](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L468)

___

#### not

▸ `Static` **not**(`x`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `boolean` \| [`Bool`](#classesboolmd) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:453](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L453)

___

#### ofFields

▸ `Static` **ofFields**(`fields`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `fields` | [`Field`](#classesfieldmd)[] |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:465](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L465)

___

#### or

▸ `Static` **or**(`x`, `y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `boolean` \| [`Bool`](#classesboolmd) |
| `y` | `boolean` \| [`Bool`](#classesboolmd) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:455](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L455)

___

#### sizeInFields

▸ `Static` **sizeInFields**(): `number`

##### Returns

`number`

##### Defined in

[snarky.d.ts:463](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L463)

___

#### toField

▸ `Static` **toField**(`x`): [`Field`](#classesfieldmd)

The constant [[`Bool`]] that is `false`.

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `boolean` \| [`Bool`](#classesboolmd) |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:441](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L441)

___

#### toFields

▸ `Static` **toFields**(`x`): [`Field`](#classesfieldmd)[]

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Bool`](#classesboolmd) |

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[snarky.d.ts:464](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L464)

___

#### toInput

▸ `Static` **toInput**(`x`): `Object`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Bool`](#classesboolmd) |

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `packed` | [[`Field`](#classesfieldmd), `number`][] |

##### Defined in

[snarky.d.ts:472](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L472)

___

#### toJSON

▸ `Static` **toJSON**(`x`): `JSONValue`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Bool`](#classesboolmd) |

##### Returns

`JSONValue`

##### Defined in

[snarky.d.ts:467](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L467)


<a name="classescharactermd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Character

## Class: Character

### Hierarchy

- [`CircuitValue`](#classescircuitvaluemd)

  ↳ **`Character`**

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [value](#value)

#### Methods

- [assertEquals](#assertequals)
- [equals](#equals)
- [isConstant](#isconstant)
- [isNull](#isnull)
- [toConstant](#toconstant)
- [toField](#tofield)
- [toFields](#tofields)
- [toJSON](#tojson)
- [toString](#tostring)
- [check](#check)
- [fromJSON](#fromjson)
- [fromObject](#fromobject)
- [fromString](#fromstring)
- [ofFields](#offields)
- [sizeInFields](#sizeinfields)
- [toConstant](#toconstant-1)
- [toFields](#tofields-1)
- [toInput](#toinput)
- [toJSON](#tojson-1)

### Constructors

#### constructor

• **new Character**(...`props`)

##### Parameters

| Name | Type |
| :------ | :------ |
| `...props` | `any`[] |

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[constructor](#constructor)

##### Defined in

[lib/circuit_value.ts:42](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L42)

### Properties

#### value

• **value**: [`Field`](#classesfieldmd)

##### Defined in

[lib/string.ts:10](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L10)

### Methods

#### assertEquals

▸ **assertEquals**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Character`](#classescharactermd) |

##### Returns

`void`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[assertEquals](#assertequals)

##### Defined in

[lib/circuit_value.ts:126](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L126)

___

#### equals

▸ **equals**(`x`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Character`](#classescharactermd) |

##### Returns

[`Bool`](#classesboolmd)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[equals](#equals)

##### Defined in

[lib/circuit_value.ts:122](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L122)

___

#### isConstant

▸ **isConstant**(): `boolean`

##### Returns

`boolean`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[isConstant](#isconstant)

##### Defined in

[lib/circuit_value.ts:130](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L130)

___

#### isNull

▸ **isNull**(): [`Bool`](#classesboolmd)

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[lib/string.ts:12](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L12)

___

#### toConstant

▸ **toConstant**(): [`Character`](#classescharactermd)

##### Returns

[`Character`](#classescharactermd)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant)

##### Defined in

[lib/circuit_value.ts:118](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L118)

___

#### toField

▸ **toField**(): [`Field`](#classesfieldmd)

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[lib/string.ts:16](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L16)

___

#### toFields

▸ **toFields**(): [`Field`](#classesfieldmd)[]

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields)

##### Defined in

[lib/circuit_value.ts:110](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L110)

___

#### toJSON

▸ **toJSON**(): `JSONValue`

##### Returns

`JSONValue`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson)

##### Defined in

[lib/circuit_value.ts:114](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L114)

___

#### toString

▸ **toString**(): `string`

##### Returns

`string`

##### Defined in

[lib/string.ts:20](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L20)

___

#### check

▸ `Static` **check**(`c`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `c` | [`Character`](#classescharactermd) |

##### Returns

`void`

##### Overrides

[CircuitValue](#classescircuitvaluemd).[check](#check)

##### Defined in

[lib/string.ts:32](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L32)

___

#### fromJSON

▸ `Static` **fromJSON**<`T`\>(`this`, `value`): ``null`` \| `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `JSONValue` |

##### Returns

``null`` \| `InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromJSON](#fromjson)

##### Defined in

[lib/circuit_value.ts:192](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L192)

___

#### fromObject

▸ `Static` **fromObject**<`T`\>(`this`, `value`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `NonMethods`<`InstanceType`<`T`\>\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromObject](#fromobject)

##### Defined in

[lib/circuit_value.ts:59](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L59)

___

#### fromString

▸ `Static` **fromString**(`str`): [`Character`](#classescharactermd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `str` | `string` |

##### Returns

[`Character`](#classescharactermd)

##### Defined in

[lib/string.ts:25](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L25)

___

#### ofFields

▸ `Static` **ofFields**<`T`\>(`this`, `xs`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `xs` | [`Field`](#classesfieldmd)[] |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[ofFields](#offields)

##### Defined in

[lib/circuit_value.ts:134](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L134)

___

#### sizeInFields

▸ `Static` **sizeInFields**(): `number`

##### Returns

`number`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[sizeInFields](#sizeinfields)

##### Defined in

[lib/circuit_value.ts:66](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L66)

___

#### toConstant

▸ `Static` **toConstant**<`T`\>(`this`, `t`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `t` | `InstanceType`<`T`\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant-1)

##### Defined in

[lib/circuit_value.ts:170](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L170)

___

#### toFields

▸ `Static` **toFields**<`T`\>(`this`, `v`): [`Field`](#classesfieldmd)[]

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields-1)

##### Defined in

[lib/circuit_value.ts:71](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L71)

___

#### toInput

▸ `Static` **toInput**<`T`\>(`this`, `v`): `HashInput`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`HashInput`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toInput](#toinput)

##### Defined in

[lib/circuit_value.ts:88](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L88)

___

#### toJSON

▸ `Static` **toJSON**<`T`\>(`this`, `v`): `JSONValue`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`JSONValue`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson-1)

##### Defined in

[lib/circuit_value.ts:178](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L178)


<a name="classescircuitmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Circuit

## Class: Circuit

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Methods

- [addConstraint](#addconstraint)
- [asProver](#asprover)
- [assertEqual](#assertequal)
- [constraintSystem](#constraintsystem)
- [equal](#equal)
- [generateKeypair](#generatekeypair)
- [if](#if)
- [inCheckedComputation](#incheckedcomputation)
- [inProver](#inprover)
- [newVariable](#newvariable)
- [prove](#prove)
- [runAndCheck](#runandcheck)
- [switch](#switch)
- [toFields](#tofields)
- [verify](#verify)
- [witness](#witness)

### Constructors

#### constructor

• **new Circuit**()

### Methods

#### addConstraint

▸ `Static` **addConstraint**(`this`, `kind`, `x`, `y`, `z`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | [`Circuit`](#classescircuitmd) |
| `kind` | ``"multiply"`` |
| `x` | [`Field`](#classesfieldmd) |
| `y` | [`Field`](#classesfieldmd) |
| `z` | [`Field`](#classesfieldmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:492](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L492)

▸ `Static` **addConstraint**(`this`, `kind`, `x`, `y`, `z`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | [`Circuit`](#classescircuitmd) |
| `kind` | ``"add"`` |
| `x` | [`Field`](#classesfieldmd) |
| `y` | [`Field`](#classesfieldmd) |
| `z` | [`Field`](#classesfieldmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:499](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L499)

▸ `Static` **addConstraint**(`this`, `kind`, `x`, `y`, `z`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | [`Circuit`](#classescircuitmd) |
| `kind` | ``"equal"`` |
| `x` | [`Field`](#classesfieldmd) |
| `y` | [`Field`](#classesfieldmd) |
| `z` | [`Field`](#classesfieldmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:506](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L506)

▸ `Static` **addConstraint**(`this`, `kind`, `x`, `y`, `z`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | [`Circuit`](#classescircuitmd) |
| `kind` | ``"boolean"`` |
| `x` | [`Field`](#classesfieldmd) |
| `y` | [`Field`](#classesfieldmd) |
| `z` | [`Field`](#classesfieldmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:513](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L513)

___

#### asProver

▸ `Static` **asProver**(`f`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `f` | () => `void` |

##### Returns

`void`

##### Defined in

[snarky.d.ts:529](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L529)

___

#### assertEqual

▸ `Static` **assertEqual**<`T`\>(`ctor`, `x`, `y`): `void`

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `ctor` | `Object` |
| `ctor.toFields` | (`x`: `T`) => [`Field`](#classesfieldmd)[] |
| `x` | `T` |
| `y` | `T` |

##### Returns

`void`

##### Defined in

[snarky.d.ts:539](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L539)

▸ `Static` **assertEqual**<`T`\>(`x`, `y`): `void`

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `T` |
| `y` | `T` |

##### Returns

`void`

##### Defined in

[snarky.d.ts:541](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L541)

___

#### constraintSystem

▸ `Static` **constraintSystem**<`T`\>(`f`): `Object`

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `f` | () => `T` |

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `digest` | `string` |
| `result` | `T` |
| `rows` | `number` |

##### Defined in

[snarky.d.ts:533](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L533)

___

#### equal

▸ `Static` **equal**<`T`\>(`ctor`, `x`, `y`): [`Bool`](#classesboolmd)

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `ctor` | `Object` |
| `ctor.toFields` | (`x`: `T`) => [`Field`](#classesfieldmd)[] |
| `x` | `T` |
| `y` | `T` |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:543](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L543)

▸ `Static` **equal**<`T`\>(`x`, `y`): [`Bool`](#classesboolmd)

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `T` |
| `y` | `T` |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:545](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L545)

___

#### generateKeypair

▸ `Static` **generateKeypair**(): [`Keypair`](#classeskeypairmd)

##### Returns

[`Keypair`](#classeskeypairmd)

##### Defined in

[snarky.d.ts:567](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L567)

___

#### if

▸ `Static` **if**<`T`\>(`b`, `ctor`, `x`, `y`): `T`

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `b` | `boolean` \| [`Bool`](#classesboolmd) |
| `ctor` | [`AsFieldElements`](#interfacesasfieldelementsmd)<`T`\> |
| `x` | `T` |
| `y` | `T` |

##### Returns

`T`

##### Defined in

[snarky.d.ts:547](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L547)

▸ `Static` **if**<`T`\>(`b`, `x`, `y`): `T`

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `b` | `boolean` \| [`Bool`](#classesboolmd) |
| `x` | `T` |
| `y` | `T` |

##### Returns

`T`

##### Defined in

[snarky.d.ts:549](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L549)

___

#### inCheckedComputation

▸ `Static` **inCheckedComputation**(): `boolean`

##### Returns

`boolean`

##### Defined in

[snarky.d.ts:577](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L577)

___

#### inProver

▸ `Static` **inProver**(): `boolean`

##### Returns

`boolean`

##### Defined in

[snarky.d.ts:575](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L575)

___

#### newVariable

▸ `Static` **newVariable**(`f`): [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `f` | () => `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:521](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L521)

___

#### prove

▸ `Static` **prove**(`privateInput`, `publicInput`, `kp`): `Proof`

##### Parameters

| Name | Type |
| :------ | :------ |
| `privateInput` | `any`[] |
| `publicInput` | `any`[] |
| `kp` | [`Keypair`](#classeskeypairmd) |

##### Returns

`Proof`

##### Defined in

[snarky.d.ts:569](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L569)

___

#### runAndCheck

▸ `Static` **runAndCheck**<`T`\>(`f`): `T`

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `f` | () => `T` |

##### Returns

`T`

##### Defined in

[snarky.d.ts:531](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L531)

___

#### switch

▸ `Static` **switch**<`T`, `A`\>(`mask`, `type`, `values`): `T`

Generalization of `Circuit.if` for choosing between more than two different cases.
It takes a "mask", which is an array of `Bool`s that contains only one `true` element, as well as a type/constructor and an array of values of that type.
The result is that value which corresponds to the true element of the mask. Example:

```ts
let x = Circuit.switch([Bool(false), Bool(true)], Field, [Field(1), Field(2)]);
x.assertEquals(2);
```

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `T` |
| `A` | extends [`AsFieldElements`](#interfacesasfieldelementsmd)<`T`, `A`\> |

##### Parameters

| Name | Type |
| :------ | :------ |
| `mask` | [`Bool`](#classesboolmd)[] |
| `type` | `A` |
| `values` | `T`[] |

##### Returns

`T`

##### Defined in

[snarky.d.ts:561](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L561)

___

#### toFields

▸ `Static` **toFields**<`A`\>(`a`): [`Field`](#classesfieldmd)[]

##### Type parameters

| Name |
| :------ |
| `A` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `a` | `A` |

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[snarky.d.ts:573](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L573)

___

#### verify

▸ `Static` **verify**(`publicInput`, `vk`, `pi`): `boolean`

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicInput` | `any`[] |
| `vk` | [`VerificationKey`](#classesverificationkeymd) |
| `pi` | `Proof` |

##### Returns

`boolean`

##### Defined in

[snarky.d.ts:571](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L571)

___

#### witness

▸ `Static` **witness**<`T`, `S`\>(`ctor`, `f`): `T`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `T` |
| `S` | extends [`AsFieldElements`](#interfacesasfieldelementsmd)<`T`, `S`\> = [`AsFieldElements`](#interfacesasfieldelementsmd)<`T`\> |

##### Parameters

| Name | Type |
| :------ | :------ |
| `ctor` | `S` |
| `f` | () => `T` |

##### Returns

`T`

##### Defined in

[snarky.d.ts:524](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L524)


<a name="classescircuitstringmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / CircuitString

## Class: CircuitString

### Hierarchy

- [`CircuitValue`](#classescircuitvaluemd)

  ↳ **`CircuitString`**

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [values](#values)
- [maxLength](#maxlength)

#### Methods

- [append](#append)
- [assertEquals](#assertequals)
- [computeLengthAndMask](#computelengthandmask)
- [equals](#equals)
- [hash](#hash)
- [isConstant](#isconstant)
- [length](#length)
- [lengthMask](#lengthmask)
- [maxLength](#maxlength-1)
- [substring](#substring)
- [toConstant](#toconstant)
- [toFields](#tofields)
- [toJSON](#tojson)
- [toString](#tostring)
- [check](#check)
- [fromCharacters](#fromcharacters)
- [fromJSON](#fromjson)
- [fromObject](#fromobject)
- [fromString](#fromstring)
- [ofFields](#offields)
- [sizeInFields](#sizeinfields)
- [toConstant](#toconstant-1)
- [toFields](#tofields-1)
- [toInput](#toinput)
- [toJSON](#tojson-1)

### Constructors

#### constructor

• `Private` **new CircuitString**(`values`)

##### Parameters

| Name | Type |
| :------ | :------ |
| `values` | [`Character`](#classescharactermd)[] |

##### Overrides

[CircuitValue](#classescircuitvaluemd).[constructor](#constructor)

##### Defined in

[lib/string.ts:44](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L44)

### Properties

#### values

• **values**: [`Character`](#classescharactermd)[]

##### Defined in

[lib/string.ts:39](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L39)

___

#### maxLength

▪ `Static` **maxLength**: `number` = `DEFAULT_STRING_LENGTH`

##### Defined in

[lib/string.ts:38](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L38)

### Methods

#### append

▸ **append**(`str`): [`CircuitString`](#classescircuitstringmd)

appends another string to this one, returns the result and proves that it fits
within the `maxLength` of this string (the other string can have a different maxLength)

##### Parameters

| Name | Type |
| :------ | :------ |
| `str` | [`CircuitString`](#classescircuitstringmd) |

##### Returns

[`CircuitString`](#classescircuitstringmd)

##### Defined in

[lib/string.ts:87](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L87)

___

#### assertEquals

▸ **assertEquals**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`CircuitString`](#classescircuitstringmd) |

##### Returns

`void`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[assertEquals](#assertequals)

##### Defined in

[lib/circuit_value.ts:126](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L126)

___

#### computeLengthAndMask

▸ `Private` **computeLengthAndMask**(): `Object`

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `length` | [`Field`](#classesfieldmd) |
| `mask` | [`Bool`](#classesboolmd)[] |

##### Defined in

[lib/string.ts:57](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L57)

___

#### equals

▸ **equals**(`x`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`CircuitString`](#classescircuitstringmd) |

##### Returns

[`Bool`](#classesboolmd)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[equals](#equals)

##### Defined in

[lib/circuit_value.ts:122](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L122)

___

#### hash

▸ **hash**(): [`Field`](#classesfieldmd)

returns true if `str` is found in this `CircuitString`

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[lib/string.ts:123](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L123)

___

#### isConstant

▸ **isConstant**(): `boolean`

##### Returns

`boolean`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[isConstant](#isconstant)

##### Defined in

[lib/circuit_value.ts:130](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L130)

___

#### length

▸ `Private` **length**(): [`Field`](#classesfieldmd)

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[lib/string.ts:79](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L79)

___

#### lengthMask

▸ `Private` **lengthMask**(): [`Bool`](#classesboolmd)[]

##### Returns

[`Bool`](#classesboolmd)[]

##### Defined in

[lib/string.ts:76](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L76)

___

#### maxLength

▸ `Private` **maxLength**(): `number`

##### Returns

`number`

##### Defined in

[lib/string.ts:52](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L52)

___

#### substring

▸ **substring**(`start`, `end`): [`CircuitString`](#classescircuitstringmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `start` | `number` |
| `end` | `number` |

##### Returns

[`CircuitString`](#classescircuitstringmd)

##### Defined in

[lib/string.ts:127](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L127)

___

#### toConstant

▸ **toConstant**(): [`CircuitString`](#classescircuitstringmd)

##### Returns

[`CircuitString`](#classescircuitstringmd)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant)

##### Defined in

[lib/circuit_value.ts:118](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L118)

___

#### toFields

▸ **toFields**(): [`Field`](#classesfieldmd)[]

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields)

##### Defined in

[lib/circuit_value.ts:110](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L110)

___

#### toJSON

▸ **toJSON**(): `JSONValue`

##### Returns

`JSONValue`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson)

##### Defined in

[lib/circuit_value.ts:114](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L114)

___

#### toString

▸ **toString**(): `string`

##### Returns

`string`

##### Defined in

[lib/string.ts:131](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L131)

___

#### check

▸ `Static` **check**<`T`\>(`this`, `v`): `void`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`void`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[check](#check)

##### Defined in

[lib/circuit_value.ts:156](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L156)

___

#### fromCharacters

▸ `Static` **fromCharacters**(`chars`): [`CircuitString`](#classescircuitstringmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `chars` | [`Character`](#classescharactermd)[] |

##### Returns

[`CircuitString`](#classescircuitstringmd)

##### Defined in

[lib/string.ts:48](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L48)

___

#### fromJSON

▸ `Static` **fromJSON**<`T`\>(`this`, `value`): ``null`` \| `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `JSONValue` |

##### Returns

``null`` \| `InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromJSON](#fromjson)

##### Defined in

[lib/circuit_value.ts:192](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L192)

___

#### fromObject

▸ `Static` **fromObject**<`T`\>(`this`, `value`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `NonMethods`<`InstanceType`<`T`\>\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromObject](#fromobject)

##### Defined in

[lib/circuit_value.ts:59](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L59)

___

#### fromString

▸ `Static` **fromString**(`str`): [`CircuitString`](#classescircuitstringmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `str` | `string` |

##### Returns

[`CircuitString`](#classescircuitstringmd)

##### Defined in

[lib/string.ts:138](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/string.ts#L138)

___

#### ofFields

▸ `Static` **ofFields**<`T`\>(`this`, `xs`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `xs` | [`Field`](#classesfieldmd)[] |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[ofFields](#offields)

##### Defined in

[lib/circuit_value.ts:134](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L134)

___

#### sizeInFields

▸ `Static` **sizeInFields**(): `number`

##### Returns

`number`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[sizeInFields](#sizeinfields)

##### Defined in

[lib/circuit_value.ts:66](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L66)

___

#### toConstant

▸ `Static` **toConstant**<`T`\>(`this`, `t`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `t` | `InstanceType`<`T`\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant-1)

##### Defined in

[lib/circuit_value.ts:170](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L170)

___

#### toFields

▸ `Static` **toFields**<`T`\>(`this`, `v`): [`Field`](#classesfieldmd)[]

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields-1)

##### Defined in

[lib/circuit_value.ts:71](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L71)

___

#### toInput

▸ `Static` **toInput**<`T`\>(`this`, `v`): `HashInput`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`HashInput`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toInput](#toinput)

##### Defined in

[lib/circuit_value.ts:88](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L88)

___

#### toJSON

▸ `Static` **toJSON**<`T`\>(`this`, `v`): `JSONValue`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`JSONValue`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson-1)

##### Defined in

[lib/circuit_value.ts:178](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L178)


<a name="classescircuitvaluemd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / CircuitValue

## Class: CircuitValue

### Hierarchy

- **`CircuitValue`**

  ↳ [`UInt32`](#classesuint32md)

  ↳ [`UInt64`](#classesuint64md)

  ↳ [`Int64`](#classesint64md)

  ↳ [`Sign`](#classessignmd)

  ↳ [`PublicKey`](#classestypespublickeymd)

  ↳ [`Character`](#classescharactermd)

  ↳ [`CircuitString`](#classescircuitstringmd)

  ↳ [`PrivateKey`](#classesprivatekeymd)

  ↳ [`Signature`](#classessignaturemd)

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Methods

- [assertEquals](#assertequals)
- [equals](#equals)
- [isConstant](#isconstant)
- [toConstant](#toconstant)
- [toFields](#tofields)
- [toJSON](#tojson)
- [check](#check)
- [fromJSON](#fromjson)
- [fromObject](#fromobject)
- [ofFields](#offields)
- [sizeInFields](#sizeinfields)
- [toConstant](#toconstant-1)
- [toFields](#tofields-1)
- [toInput](#toinput)
- [toJSON](#tojson-1)

### Constructors

#### constructor

• **new CircuitValue**(...`props`)

##### Parameters

| Name | Type |
| :------ | :------ |
| `...props` | `any`[] |

##### Defined in

[lib/circuit_value.ts:42](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L42)

### Methods

#### assertEquals

▸ **assertEquals**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`CircuitValue`](#classescircuitvaluemd) |

##### Returns

`void`

##### Defined in

[lib/circuit_value.ts:126](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L126)

___

#### equals

▸ **equals**(`x`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`CircuitValue`](#classescircuitvaluemd) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[lib/circuit_value.ts:122](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L122)

___

#### isConstant

▸ **isConstant**(): `boolean`

##### Returns

`boolean`

##### Defined in

[lib/circuit_value.ts:130](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L130)

___

#### toConstant

▸ **toConstant**(): [`CircuitValue`](#classescircuitvaluemd)

##### Returns

[`CircuitValue`](#classescircuitvaluemd)

##### Defined in

[lib/circuit_value.ts:118](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L118)

___

#### toFields

▸ **toFields**(): [`Field`](#classesfieldmd)[]

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[lib/circuit_value.ts:110](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L110)

___

#### toJSON

▸ **toJSON**(): `JSONValue`

##### Returns

`JSONValue`

##### Defined in

[lib/circuit_value.ts:114](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L114)

___

#### check

▸ `Static` **check**<`T`\>(`this`, `v`): `void`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`void`

##### Defined in

[lib/circuit_value.ts:156](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L156)

___

#### fromJSON

▸ `Static` **fromJSON**<`T`\>(`this`, `value`): ``null`` \| `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `JSONValue` |

##### Returns

``null`` \| `InstanceType`<`T`\>

##### Defined in

[lib/circuit_value.ts:192](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L192)

___

#### fromObject

▸ `Static` **fromObject**<`T`\>(`this`, `value`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `NonMethods`<`InstanceType`<`T`\>\> |

##### Returns

`InstanceType`<`T`\>

##### Defined in

[lib/circuit_value.ts:59](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L59)

___

#### ofFields

▸ `Static` **ofFields**<`T`\>(`this`, `xs`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `xs` | [`Field`](#classesfieldmd)[] |

##### Returns

`InstanceType`<`T`\>

##### Defined in

[lib/circuit_value.ts:134](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L134)

___

#### sizeInFields

▸ `Static` **sizeInFields**(): `number`

##### Returns

`number`

##### Defined in

[lib/circuit_value.ts:66](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L66)

___

#### toConstant

▸ `Static` **toConstant**<`T`\>(`this`, `t`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `t` | `InstanceType`<`T`\> |

##### Returns

`InstanceType`<`T`\>

##### Defined in

[lib/circuit_value.ts:170](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L170)

___

#### toFields

▸ `Static` **toFields**<`T`\>(`this`, `v`): [`Field`](#classesfieldmd)[]

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[lib/circuit_value.ts:71](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L71)

___

#### toInput

▸ `Static` **toInput**<`T`\>(`this`, `v`): `HashInput`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`HashInput`

##### Defined in

[lib/circuit_value.ts:88](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L88)

___

#### toJSON

▸ `Static` **toJSON**<`T`\>(`this`, `v`): `JSONValue`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`JSONValue`

##### Defined in

[lib/circuit_value.ts:178](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L178)


<a name="classesfieldmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Field

## Class: Field

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [ORDER](#order)
- [minusOne](#minusone)
- [one](#one)
- [zero](#zero)

#### Methods

- [add](#add)
- [assertBoolean](#assertboolean)
- [assertEquals](#assertequals)
- [assertGt](#assertgt)
- [assertGte](#assertgte)
- [assertLt](#assertlt)
- [assertLte](#assertlte)
- [div](#div)
- [equals](#equals)
- [gt](#gt)
- [gte](#gte)
- [inv](#inv)
- [isConstant](#isconstant)
- [isZero](#iszero)
- [lt](#lt)
- [lte](#lte)
- [mul](#mul)
- [neg](#neg)
- [ofFields](#offields)
- [rangeCheckHelper](#rangecheckhelper)
- [seal](#seal)
- [sizeInFields](#sizeinfields)
- [sqrt](#sqrt)
- [square](#square)
- [sub](#sub)
- [toBigInt](#tobigint)
- [toBits](#tobits)
- [toConstant](#toconstant)
- [toFields](#tofields)
- [toJSON](#tojson)
- [toString](#tostring)
- [check](#check)
- [fromBigInt](#frombigint)
- [fromJSON](#fromjson)
- [fromNumber](#fromnumber)
- [fromString](#fromstring)
- [ofBits](#ofbits)
- [ofFields](#offields-1)
- [random](#random)
- [sizeInFields](#sizeinfields-1)
- [toFields](#tofields-1)
- [toInput](#toinput)
- [toJSON](#tojson-1)

### Constructors

#### constructor

• **new Field**(`x`)

Coerces anything field-like to a [[`Field`]].

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `string` \| `number` \| `bigint` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Defined in

[snarky.d.ts:28](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L28)

### Properties

#### ORDER

▪ `Static` **ORDER**: `bigint`

The field order as a `bigint`.

##### Defined in

[snarky.d.ts:266](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L266)

___

#### minusOne

▪ `Static` **minusOne**: [`Field`](#classesfieldmd)

The number -1 as a [[`Field`]].

##### Defined in

[snarky.d.ts:262](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L262)

___

#### one

▪ `Static` **one**: [`Field`](#classesfieldmd)

The number 1 as a [[`Field`]].

##### Defined in

[snarky.d.ts:254](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L254)

___

#### zero

▪ `Static` **zero**: [`Field`](#classesfieldmd)

The number 0 as a [[`Field`]].

##### Defined in

[snarky.d.ts:258](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L258)

### Methods

#### add

▸ **add**(`y`): [`Field`](#classesfieldmd)

Adds this [[`Field`]] element to another coercible to a field.

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:56](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L56)

___

#### assertBoolean

▸ **assertBoolean**(): `void`

Assert that this [[`Field`]] is either 0 or 1.

```ts
Field.zero.assertBoolean();
```

This function can only be called inside a checked computation, like a
SmartContract method, and throws an error if the assertion fails.

##### Returns

`void`

##### Defined in

[snarky.d.ts:216](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L216)

___

#### assertEquals

▸ **assertEquals**(`y`): `void`

Assert that this [[`Field`]] equals another Field-like value.
Throws an error if the assertion fails.

```ts
Field.one.assertEquals(1);
```

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:205](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L205)

___

#### assertGt

▸ **assertGt**(`y`): `void`

Assert that this [[`Field`]] is greater than another Field-like value.

```ts
Field.one.assertGt(0);
```

This function can only be called inside a checked computation, like a
SmartContract method, and causes it to fail if the assertion fails.

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:184](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L184)

___

#### assertGte

▸ **assertGte**(`y`): `void`

Assert that this [[`Field`]] is greater than or equal to another Field-like value.

```ts
Field.one.assertGte(0);
```

This function can only be called inside a checked computation, like a
SmartContract method, and causes it to fail if the assertion fails.

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:195](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L195)

___

#### assertLt

▸ **assertLt**(`y`): `void`

Assert that this [[`Field`]] is lower than another Field-like value.

```ts
Field.one.assertLt(2);
```

This function can only be called inside a checked computation, like a
SmartContract method, and causes it to fail if the assertion fails.

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:162](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L162)

___

#### assertLte

▸ **assertLte**(`y`): `void`

Assert that this [[`Field`]] is lower than or equal to another Field-like value.

```ts
Field.one.assertLte(2);
```

This function can only be called inside a checked computation, like a
SmartContract method, and causes it to fail if the assertion fails.

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:173](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L173)

___

#### div

▸ **div**(`y`): [`Field`](#classesfieldmd)

Divides this [[`Field`]] element through another coercible to a field.

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:71](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L71)

___

#### equals

▸ **equals**(`y`): [`Bool`](#classesboolmd)

Check if this [[`Field`]] equals another [[`Field`]]-like value.
Returns a [[`Bool`]].

```ts
Field(2).equals(2); // Bool(true)
```

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:238](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L238)

___

#### gt

▸ **gt**(`y`): [`Bool`](#classesboolmd)

Check if this [[`Field`]] is greater than another Field-like value.
Returns a [[`Bool`]].

```ts
Field(2).gt(1); // Bool(true)
```

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:140](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L140)

___

#### gte

▸ **gte**(`y`): [`Bool`](#classesboolmd)

Check if this [[`Field`]] is greater than or equal to another Field-like value.
Returns a [[`Bool`]].

```ts
Field(2).gte(1); // Bool(true)
```

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:149](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L149)

___

#### inv

▸ **inv**(): [`Field`](#classesfieldmd)

Inverts this [[`Field`]] element.

```typescript
const invX = x.inv();
invX.assertEquals(Field.one.div(x));
```

##### Returns

[`Field`](#classesfieldmd)

A field element that is equivalent to one divided by this element.

##### Defined in

[snarky.d.ts:51](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L51)

___

#### isConstant

▸ **isConstant**(): `boolean`

##### Returns

`boolean`

##### Defined in

[snarky.d.ts:245](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L245)

___

#### isZero

▸ **isZero**(): [`Bool`](#classesboolmd)

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:217](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L217)

___

#### lt

▸ **lt**(`y`): [`Bool`](#classesboolmd)

Check if this [[`Field`]] is lower than another Field-like value.
Returns a [[`Bool`]].

```ts
Field(2).lt(3); // Bool(true)
```

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:122](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L122)

___

#### lte

▸ **lte**(`y`): [`Bool`](#classesboolmd)

Check if this [[`Field`]] is lower than or equal to another Field-like value.
Returns a [[`Bool`]].

```ts
Field(2).lte(3); // Bool(true)
```

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:131](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L131)

___

#### mul

▸ **mul**(`y`): [`Field`](#classesfieldmd)

Multiplies this [[`Field`]] element with another coercible to a field.

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:66](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L66)

___

#### neg

▸ **neg**(): [`Field`](#classesfieldmd)

Negates this [[`Field`]]. This is equivalent to multiplying the [[`Field`]]
by -1.

```typescript
const negOne = Field.one.neg();
negOne.assertEquals(-1);
```

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:39](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L39)

___

#### ofFields

▸ **ofFields**(`fields`): [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `fields` | [`Field`](#classesfieldmd)[] |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:301](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L301)

___

#### rangeCheckHelper

▸ **rangeCheckHelper**(`numBits`): [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `numBits` | `number` |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:243](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L243)

___

#### seal

▸ **seal**(): [`Field`](#classesfieldmd)

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:241](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L241)

___

#### sizeInFields

▸ **sizeInFields**(): `number`

##### Returns

`number`

##### Defined in

[snarky.d.ts:109](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L109)

___

#### sqrt

▸ **sqrt**(): [`Field`](#classesfieldmd)

Square roots this [[`Field`]] element.

```typescript
x.square().sqrt().assertEquals(x);
```

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:90](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L90)

___

#### square

▸ **square**(): [`Field`](#classesfieldmd)

Squares this [[`Field`]] element.

```typescript
const x2 = x.square();
x2.assertEquals(x.mul(x));
```

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:81](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L81)

___

#### sub

▸ **sub**(`y`): [`Field`](#classesfieldmd)

Subtracts another [[`Field`]]-like element from this one.

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:61](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L61)

___

#### toBigInt

▸ **toBigInt**(): `bigint`

Serialize the [[`Field`]] to a bigint.
This operation does NOT affect the circuit and can't be used to prove anything about the bigint representation of the Field.

##### Returns

`bigint`

##### Defined in

[snarky.d.ts:101](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L101)

___

#### toBits

▸ **toBits**(): [`Bool`](#classesboolmd)[]

Little endian binary representation of the field element.

##### Returns

[`Bool`](#classesboolmd)[]

##### Defined in

[snarky.d.ts:222](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L222)

▸ **toBits**(`length`): [`Bool`](#classesboolmd)[]

Little endian binary representation of the field element.
Fails if the field element cannot fit in `length` bits.

##### Parameters

| Name | Type |
| :------ | :------ |
| `length` | `number` |

##### Returns

[`Bool`](#classesboolmd)[]

##### Defined in

[snarky.d.ts:228](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L228)

___

#### toConstant

▸ **toConstant**(): [`Field`](#classesfieldmd)

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:246](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L246)

___

#### toFields

▸ **toFields**(): [`Field`](#classesfieldmd)[]

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[snarky.d.ts:111](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L111)

___

#### toJSON

▸ **toJSON**(): `JSONValue`

Serialize the [[`Field`]] to a JSON string.
This operation does NOT affect the circuit and can't be used to prove anything about the string representation of the Field.

##### Returns

`JSONValue`

##### Defined in

[snarky.d.ts:106](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L106)

___

#### toString

▸ **toString**(): `string`

Serialize the [[`Field`]] to a string, e.g. for printing.
This operation does NOT affect the circuit and can't be used to prove anything about the string representation of the Field.

##### Returns

`string`

##### Defined in

[snarky.d.ts:96](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L96)

___

#### check

▸ `Static` **check**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Field`](#classesfieldmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:344](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L344)

___

#### fromBigInt

▸ `Static` **fromBigInt**(`x`): [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `bigint` |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:342](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L342)

___

#### fromJSON

▸ `Static` **fromJSON**(`x`): ``null`` \| [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `JSONValue` |

##### Returns

``null`` \| [`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:338](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L338)

___

#### fromNumber

▸ `Static` **fromNumber**(`x`): [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `number` |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:341](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L341)

___

#### fromString

▸ `Static` **fromString**(`x`): [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `string` |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:340](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L340)

___

#### ofBits

▸ `Static` **ofBits**(`x`): [`Field`](#classesfieldmd)

Converts a bit array into a field element (little endian)
Fails if the field element cannot fit given too many bits.

TODO: Rename to fromBits

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | (`boolean` \| [`Bool`](#classesboolmd))[] |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:325](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L325)

___

#### ofFields

▸ `Static` **ofFields**(`fields`): [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `fields` | [`Field`](#classesfieldmd)[] |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:304](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L304)

___

#### random

▸ `Static` **random**(): [`Field`](#classesfieldmd)

A random field element.

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:271](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L271)

___

#### sizeInFields

▸ `Static` **sizeInFields**(): `number`

##### Returns

`number`

##### Defined in

[snarky.d.ts:306](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L306)

___

#### toFields

▸ `Static` **toFields**(`x`): [`Field`](#classesfieldmd)[]

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Field`](#classesfieldmd) |

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[snarky.d.ts:308](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L308)

___

#### toInput

▸ `Static` **toInput**(`x`): `Object`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Field`](#classesfieldmd) |

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `fields` | [`Field`](#classesfieldmd)[] |

##### Defined in

[snarky.d.ts:347](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L347)

___

#### toJSON

▸ `Static` **toJSON**(`x`): `JSONValue`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Field`](#classesfieldmd) |

##### Returns

`JSONValue`

##### Defined in

[snarky.d.ts:337](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L337)


<a name="classesgroupmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Group

## Class: Group

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [x](#x)
- [y](#y)
- [generator](#generator)

#### Methods

- [add](#add)
- [assertEquals](#assertequals)
- [equals](#equals)
- [neg](#neg)
- [scale](#scale)
- [sub](#sub)
- [toJSON](#tojson)
- [add](#add-1)
- [assertEqual](#assertequal)
- [check](#check)
- [equal](#equal)
- [fromJSON](#fromjson)
- [neg](#neg-1)
- [ofFields](#offields)
- [scale](#scale-1)
- [sizeInFields](#sizeinfields)
- [sub](#sub-1)
- [toFields](#tofields)
- [toJSON](#tojson-1)

### Constructors

#### constructor

• **new Group**(`args`)

##### Parameters

| Name | Type |
| :------ | :------ |
| `args` | `Object` |
| `args.x` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |
| `args.y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Defined in

[snarky.d.ts:648](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L648)

• **new Group**(`x`, `y`)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |
| `y` | `string` \| `number` \| `boolean` \| [`Field`](#classesfieldmd) |

##### Defined in

[snarky.d.ts:652](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L652)

### Properties

#### x

• **x**: [`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:634](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L634)

___

#### y

• **y**: [`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:635](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L635)

___

#### generator

▪ `Static` **generator**: [`Group`](#classesgroupmd)

##### Defined in

[snarky.d.ts:657](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L657)

### Methods

#### add

▸ **add**(`y`): [`Group`](#classesgroupmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`Group`](#classesgroupmd) |

##### Returns

[`Group`](#classesgroupmd)

##### Defined in

[snarky.d.ts:637](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L637)

___

#### assertEquals

▸ **assertEquals**(`y`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`Group`](#classesgroupmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:643](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L643)

___

#### equals

▸ **equals**(`y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`Group`](#classesgroupmd) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:644](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L644)

___

#### neg

▸ **neg**(): [`Group`](#classesgroupmd)

##### Returns

[`Group`](#classesgroupmd)

##### Defined in

[snarky.d.ts:639](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L639)

___

#### scale

▸ **scale**(`y`): [`Group`](#classesgroupmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`Scalar`](#classesscalarmd) |

##### Returns

[`Group`](#classesgroupmd)

##### Defined in

[snarky.d.ts:640](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L640)

___

#### sub

▸ **sub**(`y`): [`Group`](#classesgroupmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`Group`](#classesgroupmd) |

##### Returns

[`Group`](#classesgroupmd)

##### Defined in

[snarky.d.ts:638](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L638)

___

#### toJSON

▸ **toJSON**(): `JSONValue`

##### Returns

`JSONValue`

##### Defined in

[snarky.d.ts:646](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L646)

___

#### add

▸ `Static` **add**(`x`, `y`): [`Group`](#classesgroupmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Group`](#classesgroupmd) |
| `y` | [`Group`](#classesgroupmd) |

##### Returns

[`Group`](#classesgroupmd)

##### Defined in

[snarky.d.ts:658](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L658)

___

#### assertEqual

▸ `Static` **assertEqual**(`x`, `y`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Group`](#classesgroupmd) |
| `y` | [`Group`](#classesgroupmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:664](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L664)

___

#### check

▸ `Static` **check**(`g`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `g` | [`Group`](#classesgroupmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:679](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L679)

___

#### equal

▸ `Static` **equal**(`x`, `y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Group`](#classesgroupmd) |
| `y` | [`Group`](#classesgroupmd) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[snarky.d.ts:665](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L665)

___

#### fromJSON

▸ `Static` **fromJSON**(`__namedParameters`): ``null`` \| [`Group`](#classesgroupmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | `Object` |
| `__namedParameters.x` | `string` \| `number` |
| `__namedParameters.y` | `string` \| `number` |

##### Returns

``null`` \| [`Group`](#classesgroupmd)

##### Defined in

[snarky.d.ts:672](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L672)

___

#### neg

▸ `Static` **neg**(`x`): [`Group`](#classesgroupmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Group`](#classesgroupmd) |

##### Returns

[`Group`](#classesgroupmd)

##### Defined in

[snarky.d.ts:660](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L660)

___

#### ofFields

▸ `Static` **ofFields**(`fields`): [`Group`](#classesgroupmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `fields` | [`Field`](#classesfieldmd)[] |

##### Returns

[`Group`](#classesgroupmd)

##### Defined in

[snarky.d.ts:668](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L668)

___

#### scale

▸ `Static` **scale**(`x`, `y`): [`Group`](#classesgroupmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Group`](#classesgroupmd) |
| `y` | [`Scalar`](#classesscalarmd) |

##### Returns

[`Group`](#classesgroupmd)

##### Defined in

[snarky.d.ts:661](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L661)

___

#### sizeInFields

▸ `Static` **sizeInFields**(): `number`

##### Returns

`number`

##### Defined in

[snarky.d.ts:669](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L669)

___

#### sub

▸ `Static` **sub**(`x`, `y`): [`Group`](#classesgroupmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Group`](#classesgroupmd) |
| `y` | [`Group`](#classesgroupmd) |

##### Returns

[`Group`](#classesgroupmd)

##### Defined in

[snarky.d.ts:659](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L659)

___

#### toFields

▸ `Static` **toFields**(`x`): [`Field`](#classesfieldmd)[]

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Group`](#classesgroupmd) |

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[snarky.d.ts:667](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L667)

___

#### toJSON

▸ `Static` **toJSON**(`x`): `JSONValue`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Group`](#classesgroupmd) |

##### Returns

`JSONValue`

##### Defined in

[snarky.d.ts:671](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L671)


<a name="classesint64md"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Int64

## Class: Int64

### Hierarchy

- [`CircuitValue`](#classescircuitvaluemd)

  ↳ **`Int64`**

### Implements

- `BalanceChange`

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [magnitude](#magnitude)
- [sgn](#sgn)

#### Accessors

- [minusOne](#minusone)
- [one](#one)
- [zero](#zero)

#### Methods

- [add](#add)
- [assertEquals](#assertequals)
- [div](#div)
- [equals](#equals)
- [isConstant](#isconstant)
- [isPositive](#ispositive)
- [mod](#mod)
- [mul](#mul)
- [neg](#neg)
- [sub](#sub)
- [toConstant](#toconstant)
- [toField](#tofield)
- [toFields](#tofields)
- [toJSON](#tojson)
- [toString](#tostring)
- [check](#check)
- [from](#from)
- [fromBigInt](#frombigint)
- [fromField](#fromfield)
- [fromFieldUnchecked](#fromfieldunchecked)
- [fromJSON](#fromjson)
- [fromNumber](#fromnumber)
- [fromObject](#fromobject)
- [fromString](#fromstring)
- [fromUnsigned](#fromunsigned)
- [ofFields](#offields)
- [sizeInFields](#sizeinfields)
- [toConstant](#toconstant-1)
- [toFields](#tofields-1)
- [toInput](#toinput)
- [toJSON](#tojson-1)

### Constructors

#### constructor

• **new Int64**(`magnitude`, `sgn?`)

##### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `magnitude` | [`UInt64`](#classesuint64md) | `undefined` |
| `sgn` | [`Sign`](#classessignmd) | `Sign.one` |

##### Overrides

[CircuitValue](#classescircuitvaluemd).[constructor](#constructor)

##### Defined in

[lib/int.ts:432](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L432)

### Properties

#### magnitude

• **magnitude**: [`UInt64`](#classesuint64md)

##### Implementation of

BalanceChange.magnitude

##### Defined in

[lib/int.ts:409](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L409)

___

#### sgn

• **sgn**: [`Sign`](#classessignmd)

##### Implementation of

BalanceChange.sgn

##### Defined in

[lib/int.ts:410](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L410)

### Accessors

#### minusOne

• `Static` `get` **minusOne**(): [`Int64`](#classesint64md)

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:492](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L492)

___

#### one

• `Static` `get` **one**(): [`Int64`](#classesint64md)

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:489](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L489)

___

#### zero

• `Static` `get` **zero**(): [`Int64`](#classesint64md)

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:486](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L486)

### Methods

#### add

▸ **add**(`y`): [`Int64`](#classesint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `bigint` \| [`UInt32`](#classesuint32md) \| [`UInt64`](#classesuint64md) \| [`Int64`](#classesint64md) |

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:514](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L514)

___

#### assertEquals

▸ **assertEquals**(`y`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `bigint` \| [`UInt32`](#classesuint32md) \| [`UInt64`](#classesuint64md) \| [`Int64`](#classesint64md) |

##### Returns

`void`

##### Overrides

[CircuitValue](#classescircuitvaluemd).[assertEquals](#assertequals)

##### Defined in

[lib/int.ts:543](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L543)

___

#### div

▸ **div**(`y`): [`Int64`](#classesint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `bigint` \| [`UInt32`](#classesuint32md) \| [`UInt64`](#classesuint64md) \| [`Int64`](#classesint64md) |

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:526](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L526)

___

#### equals

▸ **equals**(`y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `bigint` \| [`UInt32`](#classesuint32md) \| [`UInt64`](#classesuint64md) \| [`Int64`](#classesint64md) |

##### Returns

[`Bool`](#classesboolmd)

##### Overrides

[CircuitValue](#classescircuitvaluemd).[equals](#equals)

##### Defined in

[lib/int.ts:539](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L539)

___

#### isConstant

▸ **isConstant**(): `boolean`

##### Returns

`boolean`

##### Overrides

[CircuitValue](#classescircuitvaluemd).[isConstant](#isconstant)

##### Defined in

[lib/int.ts:477](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L477)

___

#### isPositive

▸ **isPositive**(): [`Bool`](#classesboolmd)

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[lib/int.ts:547](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L547)

___

#### mod

▸ **mod**(`y`): [`Int64`](#classesint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `bigint` \| [`UInt32`](#classesuint32md) \| [`UInt64`](#classesuint64md) |

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:532](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L532)

___

#### mul

▸ **mul**(`y`): [`Int64`](#classesint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `bigint` \| [`UInt32`](#classesuint32md) \| [`UInt64`](#classesuint64md) \| [`Int64`](#classesint64md) |

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:522](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L522)

___

#### neg

▸ **neg**(): [`Int64`](#classesint64md)

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:509](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L509)

___

#### sub

▸ **sub**(`y`): [`Int64`](#classesint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| `bigint` \| [`UInt32`](#classesuint32md) \| [`UInt64`](#classesuint64md) \| [`Int64`](#classesint64md) |

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:518](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L518)

___

#### toConstant

▸ **toConstant**(): [`Int64`](#classesint64md)

##### Returns

[`Int64`](#classesint64md)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant)

##### Defined in

[lib/circuit_value.ts:118](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L118)

___

#### toField

▸ **toField**(): [`Field`](#classesfieldmd)

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[lib/int.ts:496](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L496)

___

#### toFields

▸ **toFields**(): [`Field`](#classesfieldmd)[]

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields)

##### Defined in

[lib/circuit_value.ts:110](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L110)

___

#### toJSON

▸ **toJSON**(): `JSONValue`

##### Returns

`JSONValue`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson)

##### Defined in

[lib/circuit_value.ts:114](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L114)

___

#### toString

▸ **toString**(): `string`

##### Returns

`string`

##### Defined in

[lib/int.ts:471](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L471)

___

#### check

▸ `Static` **check**<`T`\>(`this`, `v`): `void`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`void`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[check](#check)

##### Defined in

[lib/circuit_value.ts:156](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L156)

___

#### from

▸ `Static` **from**(`x`): [`Int64`](#classesint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `string` \| `number` \| `bigint` \| [`Field`](#classesfieldmd) \| [`UInt32`](#classesuint32md) \| [`UInt64`](#classesuint64md) \| [`Int64`](#classesint64md) |

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:454](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L454)

___

#### fromBigInt

▸ `Static` **fromBigInt**(`x`): [`Int64`](#classesint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `bigint` |

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:467](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L467)

___

#### fromField

▸ `Static` **fromField**(`x`): [`Int64`](#classesint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Field`](#classesfieldmd) |

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:500](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L500)

___

#### fromFieldUnchecked

▸ `Static` `Private` **fromFieldUnchecked**(`x`): [`Int64`](#classesint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Field`](#classesfieldmd) |

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:436](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L436)

___

#### fromJSON

▸ `Static` **fromJSON**<`T`\>(`this`, `value`): ``null`` \| `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `JSONValue` |

##### Returns

``null`` \| `InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromJSON](#fromjson)

##### Defined in

[lib/circuit_value.ts:192](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L192)

___

#### fromNumber

▸ `Static` **fromNumber**(`x`): [`Int64`](#classesint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `number` |

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:461](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L461)

___

#### fromObject

▸ `Static` **fromObject**<`T`\>(`this`, `value`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `NonMethods`<`InstanceType`<`T`\>\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromObject](#fromobject)

##### Defined in

[lib/circuit_value.ts:59](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L59)

___

#### fromString

▸ `Static` **fromString**(`x`): [`Int64`](#classesint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `string` |

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:464](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L464)

___

#### fromUnsigned

▸ `Static` **fromUnsigned**(`x`): [`Int64`](#classesint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`UInt32`](#classesuint32md) \| [`UInt64`](#classesuint64md) |

##### Returns

[`Int64`](#classesint64md)

##### Defined in

[lib/int.ts:449](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L449)

___

#### ofFields

▸ `Static` **ofFields**<`T`\>(`this`, `xs`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `xs` | [`Field`](#classesfieldmd)[] |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[ofFields](#offields)

##### Defined in

[lib/circuit_value.ts:134](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L134)

___

#### sizeInFields

▸ `Static` **sizeInFields**(): `number`

##### Returns

`number`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[sizeInFields](#sizeinfields)

##### Defined in

[lib/circuit_value.ts:66](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L66)

___

#### toConstant

▸ `Static` **toConstant**<`T`\>(`this`, `t`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `t` | `InstanceType`<`T`\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant-1)

##### Defined in

[lib/circuit_value.ts:170](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L170)

___

#### toFields

▸ `Static` **toFields**<`T`\>(`this`, `v`): [`Field`](#classesfieldmd)[]

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields-1)

##### Defined in

[lib/circuit_value.ts:71](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L71)

___

#### toInput

▸ `Static` **toInput**<`T`\>(`this`, `v`): `HashInput`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`HashInput`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toInput](#toinput)

##### Defined in

[lib/circuit_value.ts:88](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L88)

___

#### toJSON

▸ `Static` **toJSON**<`T`\>(`this`, `v`): `JSONValue`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`JSONValue`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson-1)

##### Defined in

[lib/circuit_value.ts:178](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L178)


<a name="classeskeypairmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Keypair

## Class: Keypair

Contains a proving key and [[ VerificationKey ]] which can be used to verify proofs.

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Methods

- [verificationKey](#verificationkey)

### Constructors

#### constructor

• **new Keypair**()

### Methods

#### verificationKey

▸ **verificationKey**(): [`VerificationKey`](#classesverificationkeymd)

##### Returns

[`VerificationKey`](#classesverificationkeymd)

##### Defined in

[snarky.d.ts:709](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L709)


<a name="classesledgermd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Ledger

## Class: Ledger

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [encoding](#encoding)
- [hashInputFromJson](#hashinputfromjson)

#### Methods

- [addAccount](#addaccount)
- [applyJsonTransaction](#applyjsontransaction)
- [getAccount](#getaccount)
- [create](#create)
- [createTokenAccount](#createtokenaccount)
- [customTokenId](#customtokenid)
- [customTokenIdChecked](#customtokenidchecked)
- [dummySignature](#dummysignature)
- [fieldOfBase58](#fieldofbase58)
- [fieldToBase58](#fieldtobase58)
- [fieldsOfJson](#fieldsofjson)
- [hashPartyFromFields](#hashpartyfromfields)
- [hashPartyFromJson](#hashpartyfromjson)
- [memoToBase58](#memotobase58)
- [privateKeyOfString](#privatekeyofstring)
- [privateKeyToString](#privatekeytostring)
- [publicKeyOfString](#publickeyofstring)
- [publicKeyToString](#publickeytostring)
- [signFeePayer](#signfeepayer)
- [signFieldElement](#signfieldelement)
- [signOtherParty](#signotherparty)
- [transactionCommitments](#transactioncommitments)
- [zkappPublicInput](#zkapppublicinput)

### Constructors

#### constructor

• **new Ledger**()

### Properties

#### encoding

▪ `Static` **encoding**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `versionBytes` | `Record`<``"tokenIdKey"`` \| ``"receiptChainHash"`` \| ``"ledgerHash"`` \| ``"epochSeed"`` \| ``"stateHash"``, `number`\> |
| `ofBase58` | (`base58`: `string`, `versionByte`: `number`) => `MlBytes` |
| `toBase58` | (`s`: `MlBytes`, `versionByte`: `number`) => `string` |

##### Defined in

[snarky.d.ts:807](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L807)

___

#### hashInputFromJson

▪ `Static` **hashInputFromJson**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `accountPrecondition` | (`json`: `String`) => `OcamlInput` |
| `body` | (`json`: `String`) => `OcamlInput` |
| `networkPrecondition` | (`json`: `String`) => `OcamlInput` |
| `packInput` | (`input`: `OcamlInput`) => [`Field`](#classesfieldmd)[] |
| `permissions` | (`json`: `String`) => `OcamlInput` |
| `timing` | (`json`: `String`) => `OcamlInput` |
| `update` | (`json`: `String`) => `OcamlInput` |

##### Defined in

[snarky.d.ts:796](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L796)

### Methods

#### addAccount

▸ **addAccount**(`publicKey`, `balance`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | `PublicKey_` |
| `balance` | `string` |

##### Returns

`void`

##### Defined in

[snarky.d.ts:750](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L750)

___

#### applyJsonTransaction

▸ **applyJsonTransaction**(`txJson`, `accountCreationFee`, `networkState`): `Account`[]

##### Parameters

| Name | Type |
| :------ | :------ |
| `txJson` | `string` |
| `accountCreationFee` | `string` |
| `networkState` | `string` |

##### Returns

`Account`[]

##### Defined in

[snarky.d.ts:752](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L752)

___

#### getAccount

▸ **getAccount**(`publicKey`, `tokenId`): `undefined` \| `Account`

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | `PublicKey_` |
| `tokenId` | [`Field`](#classesfieldmd) |

##### Returns

`undefined` \| `Account`

##### Defined in

[snarky.d.ts:758](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L758)

___

#### create

▸ `Static` **create**(`genesisAccounts`): [`Ledger`](#classesledgermd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `genesisAccounts` | { `balance`: `string` ; `publicKey`: `PublicKey_`  }[] |

##### Returns

[`Ledger`](#classesledgermd)

##### Defined in

[snarky.d.ts:746](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L746)

___

#### createTokenAccount

▸ `Static` **createTokenAccount**(`publicKey`, `tokenId`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | `PublicKey_` |
| `tokenId` | [`Field`](#classesfieldmd) |

##### Returns

`string`

##### Defined in

[snarky.d.ts:782](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L782)

___

#### customTokenId

▸ `Static` **customTokenId**(`publicKey`, `tokenId`): [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | `PublicKey_` |
| `tokenId` | [`Field`](#classesfieldmd) |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:780](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L780)

___

#### customTokenIdChecked

▸ `Static` **customTokenIdChecked**(`publicKey`, `tokenId`): [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | `PublicKey_` |
| `tokenId` | [`Field`](#classesfieldmd) |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:781](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L781)

___

#### dummySignature

▸ `Static` **dummySignature**(): `string`

##### Returns

`string`

##### Defined in

[snarky.d.ts:772](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L772)

___

#### fieldOfBase58

▸ `Static` **fieldOfBase58**(`fieldBase58`): [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `fieldBase58` | `string` |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:789](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L789)

___

#### fieldToBase58

▸ `Static` **fieldToBase58**(`field`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `field` | [`Field`](#classesfieldmd) |

##### Returns

`string`

##### Defined in

[snarky.d.ts:788](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L788)

___

#### fieldsOfJson

▸ `Static` **fieldsOfJson**(`json`): [`Field`](#classesfieldmd)[]

##### Parameters

| Name | Type |
| :------ | :------ |
| `json` | `string` |

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[snarky.d.ts:792](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L792)

___

#### hashPartyFromFields

▸ `Static` **hashPartyFromFields**(`fields`): [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `fields` | [`Field`](#classesfieldmd)[] |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:793](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L793)

___

#### hashPartyFromJson

▸ `Static` **hashPartyFromJson**(`json`): [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `json` | `string` |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[snarky.d.ts:794](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L794)

___

#### memoToBase58

▸ `Static` **memoToBase58**(`memoString`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `memoString` | `string` |

##### Returns

`string`

##### Defined in

[snarky.d.ts:790](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L790)

___

#### privateKeyOfString

▸ `Static` **privateKeyOfString**(`privateKeyBase58`): [`Scalar`](#classesscalarmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `privateKeyBase58` | `string` |

##### Returns

[`Scalar`](#classesscalarmd)

##### Defined in

[snarky.d.ts:787](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L787)

___

#### privateKeyToString

▸ `Static` **privateKeyToString**(`privateKey`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `privateKey` | `Object` |
| `privateKey.s` | [`Scalar`](#classesscalarmd) |

##### Returns

`string`

##### Defined in

[snarky.d.ts:786](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L786)

___

#### publicKeyOfString

▸ `Static` **publicKeyOfString**(`publicKeyBase58`): `PublicKey_`

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKeyBase58` | `string` |

##### Returns

`PublicKey_`

##### Defined in

[snarky.d.ts:785](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L785)

___

#### publicKeyToString

▸ `Static` **publicKeyToString**(`publicKey`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | `PublicKey_` |

##### Returns

`string`

##### Defined in

[snarky.d.ts:784](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L784)

___

#### signFeePayer

▸ `Static` **signFeePayer**(`txJson`, `privateKey`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `txJson` | `string` |
| `privateKey` | `Object` |
| `privateKey.s` | [`Scalar`](#classesscalarmd) |

##### Returns

`string`

##### Defined in

[snarky.d.ts:773](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L773)

___

#### signFieldElement

▸ `Static` **signFieldElement**(`messageHash`, `privateKey`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `messageHash` | [`Field`](#classesfieldmd) |
| `privateKey` | `Object` |
| `privateKey.s` | [`Scalar`](#classesscalarmd) |

##### Returns

`string`

##### Defined in

[snarky.d.ts:768](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L768)

___

#### signOtherParty

▸ `Static` **signOtherParty**(`txJson`, `privateKey`, `i`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `txJson` | `string` |
| `privateKey` | `Object` |
| `privateKey.s` | [`Scalar`](#classesscalarmd) |
| `i` | `number` |

##### Returns

`string`

##### Defined in

[snarky.d.ts:774](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L774)

___

#### transactionCommitments

▸ `Static` **transactionCommitments**(`txJson`): `Object`

##### Parameters

| Name | Type |
| :------ | :------ |
| `txJson` | `string` |

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `commitment` | [`Field`](#classesfieldmd) |
| `fullCommitment` | [`Field`](#classesfieldmd) |

##### Defined in

[snarky.d.ts:760](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L760)

___

#### zkappPublicInput

▸ `Static` **zkappPublicInput**(`txJson`, `partyIndex`): `Object`

##### Parameters

| Name | Type |
| :------ | :------ |
| `txJson` | `string` |
| `partyIndex` | `number` |

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `calls` | [`Field`](#classesfieldmd) |
| `party` | [`Field`](#classesfieldmd) |

##### Defined in

[snarky.d.ts:764](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L764)


<a name="classespartymd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Party

## Class: Party

### Implements

- [`Party`](#party-1)

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [account](#account)
- [authorization](#authorization)
- [body](#body)
- [children](#children)
- [isSelf](#isself)
- [lazyAuthorization](#lazyauthorization)
- [network](#network)
- [parent](#parent)

#### Accessors

- [balance](#balance)
- [publicKey](#publickey)
- [tokenId](#tokenid)
- [tokenSymbol](#tokensymbol)
- [update](#update)

#### Methods

- [hash](#hash)
- [send](#send)
- [setNoncePrecondition](#setnonceprecondition)
- [sign](#sign)
- [signInPlace](#signinplace)
- [toFields](#tofields)
- [toJSON](#tojson)
- [toPublicInput](#topublicinput)
- [token](#token)
- [assertBetween](#assertbetween)
- [assertEquals](#assertequals)
- [clone](#clone)
- [createSigned](#createsigned)
- [createUnsigned](#createunsigned)
- [defaultFeePayer](#defaultfeepayer)
- [defaultParty](#defaultparty)
- [dummyFeePayer](#dummyfeepayer)
- [fundNewAccount](#fundnewaccount)
- [getNonce](#getnonce)
- [setValue](#setvalue)
- [signFeePayerInPlace](#signfeepayerinplace)
- [witness](#witness)

### Constructors

#### constructor

• **new Party**(`body`, `authorization?`)

##### Parameters

| Name | Type |
| :------ | :------ |
| `body` | `Body` |
| `authorization?` | `Object` |
| `authorization.proof?` | `string` |
| `authorization.signature?` | `string` |

##### Defined in

[lib/party.ts:579](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L579)

### Properties

#### account

• **account**: `PreconditionClassType`<`AccountPrecondition`\>

##### Defined in

[lib/party.ts:572](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L572)

___

#### authorization

• **authorization**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `proof?` | `string` |
| `signature?` | `string` |

##### Implementation of

Types.Party.authorization

##### Defined in

[lib/party.ts:570](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L570)

___

#### body

• **body**: `Body`

##### Implementation of

Types.Party.body

##### Defined in

[lib/party.ts:569](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L569)

___

#### children

• **children**: { `calls?`: [`Field`](#classesfieldmd) ; `party`: [`Party`](#classespartymd)  }[] = `[]`

##### Defined in

[lib/party.ts:574](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L574)

___

#### isSelf

• `Private` **isSelf**: `boolean`

##### Defined in

[lib/party.ts:577](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L577)

___

#### lazyAuthorization

• **lazyAuthorization**: `undefined` \| `LazySignature` \| `LazyProof` = `undefined`

##### Defined in

[lib/party.ts:571](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L571)

___

#### network

• **network**: `PreconditionClassType`<{ `blockchainLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceGenesis`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceHardFork`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `minWindowDensity`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `nextEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `snarkedLedgerHash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `stakingEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `timestamp`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  }\>

##### Defined in

[lib/party.ts:573](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L573)

___

#### parent

• **parent**: `undefined` \| [`Party`](#classespartymd) = `undefined`

##### Defined in

[lib/party.ts:575](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L575)

### Accessors

#### balance

• `get` **balance**(): `Object`

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `addInPlace` | (`x`: `string` \| `number` \| `bigint` \| [`UInt32`](#classesuint32md) \| [`UInt64`](#classesuint64md) \| [`Int64`](#classesint64md)) => `void` |
| `subInPlace` | (`x`: `string` \| `number` \| `bigint` \| [`UInt32`](#classesuint32md) \| [`UInt64`](#classesuint64md) \| [`Int64`](#classesint64md)) => `void` |

##### Defined in

[lib/party.ts:701](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L701)

___

#### publicKey

• `get` **publicKey**(): [`PublicKey`](#classestypespublickeymd)

##### Returns

[`PublicKey`](#classestypespublickeymd)

##### Defined in

[lib/party.ts:778](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L778)

___

#### tokenId

• `get` **tokenId**(): [`Field`](#classesfieldmd)

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[lib/party.ts:669](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L669)

___

#### tokenSymbol

• `get` **tokenSymbol**(): `Object`

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `set` | (`tokenSymbol`: `string`) => `void` |

##### Defined in

[lib/party.ts:673](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L673)

___

#### update

• `get` **update**(): `Object`

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `appState` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }[] |
| `delegate` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`PublicKey`](#classestypespublickeymd)  } |
| `delegate.isSome` | [`Bool`](#classesboolmd) |
| `delegate.value` | [`PublicKey`](#classestypespublickeymd) |
| `permissions` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `editSequenceState`: [`AuthRequired`](#authrequired-1) ; `editState`: [`AuthRequired`](#authrequired-1) ; `incrementNonce`: [`AuthRequired`](#authrequired-1) ; `receive`: [`AuthRequired`](#authrequired-1) ; `send`: [`AuthRequired`](#authrequired-1) ; `setDelegate`: [`AuthRequired`](#authrequired-1) ; `setPermissions`: [`AuthRequired`](#authrequired-1) ; `setTokenSymbol`: [`AuthRequired`](#authrequired-1) ; `setVerificationKey`: [`AuthRequired`](#authrequired-1) ; `setVotingFor`: [`AuthRequired`](#authrequired-1) ; `setZkappUri`: [`AuthRequired`](#authrequired-1)  }  } |
| `permissions.isSome` | [`Bool`](#classesboolmd) |
| `permissions.value` | { `editSequenceState`: [`AuthRequired`](#authrequired-1) ; `editState`: [`AuthRequired`](#authrequired-1) ; `incrementNonce`: [`AuthRequired`](#authrequired-1) ; `receive`: [`AuthRequired`](#authrequired-1) ; `send`: [`AuthRequired`](#authrequired-1) ; `setDelegate`: [`AuthRequired`](#authrequired-1) ; `setPermissions`: [`AuthRequired`](#authrequired-1) ; `setTokenSymbol`: [`AuthRequired`](#authrequired-1) ; `setVerificationKey`: [`AuthRequired`](#authrequired-1) ; `setVotingFor`: [`AuthRequired`](#authrequired-1) ; `setZkappUri`: [`AuthRequired`](#authrequired-1)  } |
| `permissions.value.editSequenceState` | [`AuthRequired`](#authrequired-1) |
| `permissions.value.editState` | [`AuthRequired`](#authrequired-1) |
| `permissions.value.incrementNonce` | [`AuthRequired`](#authrequired-1) |
| `permissions.value.receive` | [`AuthRequired`](#authrequired-1) |
| `permissions.value.send` | [`AuthRequired`](#authrequired-1) |
| `permissions.value.setDelegate` | [`AuthRequired`](#authrequired-1) |
| `permissions.value.setPermissions` | [`AuthRequired`](#authrequired-1) |
| `permissions.value.setTokenSymbol` | [`AuthRequired`](#authrequired-1) |
| `permissions.value.setVerificationKey` | [`AuthRequired`](#authrequired-1) |
| `permissions.value.setVotingFor` | [`AuthRequired`](#authrequired-1) |
| `permissions.value.setZkappUri` | [`AuthRequired`](#authrequired-1) |
| `timing` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `cliffAmount`: [`UInt64`](#classesuint64md) ; `cliffTime`: [`UInt32`](#classesuint32md) ; `initialMinimumBalance`: [`UInt64`](#classesuint64md) ; `vestingIncrement`: [`UInt64`](#classesuint64md) ; `vestingPeriod`: [`UInt32`](#classesuint32md)  }  } |
| `timing.isSome` | [`Bool`](#classesboolmd) |
| `timing.value` | { `cliffAmount`: [`UInt64`](#classesuint64md) ; `cliffTime`: [`UInt32`](#classesuint32md) ; `initialMinimumBalance`: [`UInt64`](#classesuint64md) ; `vestingIncrement`: [`UInt64`](#classesuint64md) ; `vestingPeriod`: [`UInt32`](#classesuint32md)  } |
| `timing.value.cliffAmount` | [`UInt64`](#classesuint64md) |
| `timing.value.cliffTime` | [`UInt32`](#classesuint32md) |
| `timing.value.initialMinimumBalance` | [`UInt64`](#classesuint64md) |
| `timing.value.vestingIncrement` | [`UInt64`](#classesuint64md) |
| `timing.value.vestingPeriod` | [`UInt32`](#classesuint32md) |
| `tokenSymbol` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`TokenSymbol`](#tokensymbol-1)  } |
| `tokenSymbol.isSome` | [`Bool`](#classesboolmd) |
| `tokenSymbol.value` | [`TokenSymbol`](#tokensymbol-1) |
| `verificationKey` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `data`: `string` ; `hash`: [`Field`](#classesfieldmd)  }  } |
| `verificationKey.isSome` | [`Bool`](#classesboolmd) |
| `verificationKey.value` | { `data`: `string` ; `hash`: [`Field`](#classesfieldmd)  } |
| `verificationKey.value.data` | `string` |
| `verificationKey.value.hash` | [`Field`](#classesfieldmd) |
| `votingFor` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } |
| `votingFor.isSome` | [`Bool`](#classesboolmd) |
| `votingFor.value` | [`Field`](#classesfieldmd) |
| `zkappUri` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `data`: `string` ; `hash`: [`Field`](#classesfieldmd)  }  } |
| `zkappUri.isSome` | [`Bool`](#classesboolmd) |
| `zkappUri.value` | { `data`: `string` ; `hash`: [`Field`](#classesfieldmd)  } |
| `zkappUri.value.data` | `string` |
| `zkappUri.value.hash` | [`Field`](#classesfieldmd) |

##### Defined in

[lib/party.ts:716](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L716)

### Methods

#### hash

▸ **hash**(): [`Field`](#classesfieldmd)

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[lib/party.ts:844](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L844)

___

#### send

▸ **send**(`__namedParameters`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | `Omit`<`SendParams`, ``"from"``\> |

##### Returns

`void`

##### Defined in

[lib/party.ts:683](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L683)

___

#### setNoncePrecondition

▸ **setNoncePrecondition**(`fallbackToZero?`): [`UInt32`](#classesuint32md)

##### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `fallbackToZero` | `boolean` | `false` |

##### Returns

[`UInt32`](#classesuint32md)

##### Defined in

[lib/party.ts:829](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L829)

___

#### sign

▸ **sign**(`privateKey?`): `any`

##### Parameters

| Name | Type |
| :------ | :------ |
| `privateKey?` | [`PrivateKey`](#classesprivatekeymd) |

##### Returns

`any`

##### Defined in

[lib/party.ts:788](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L788)

___

#### signInPlace

▸ **signInPlace**(`privateKey?`, `fallbackToZeroNonce?`): `void`

##### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `privateKey?` | [`PrivateKey`](#classesprivatekeymd) | `undefined` |
| `fallbackToZeroNonce` | `boolean` | `false` |

##### Returns

`void`

##### Defined in

[lib/party.ts:782](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L782)

___

#### toFields

▸ **toFields**(): [`Field`](#classesfieldmd)[]

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[lib/party.ts:836](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L836)

___

#### toJSON

▸ **toJSON**(): [`Party`](#party)

##### Returns

[`Party`](#party)

##### Defined in

[lib/party.ts:840](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L840)

___

#### toPublicInput

▸ **toPublicInput**(): [`ZkappPublicInput`](#zkapppublicinput-1)

##### Returns

[`ZkappPublicInput`](#zkapppublicinput-1)

##### Defined in

[lib/party.ts:862](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L862)

___

#### token

▸ **token**(): `Object`

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `id` | [`Field`](#classesfieldmd) |
| `parentTokenId` | [`Field`](#classesfieldmd) |
| `tokenOwner` | [`PublicKey`](#classestypespublickeymd) |
| `burn` | (`__namedParameters`: `MintOrBurnParams`) => `void` |
| `mint` | (`__namedParameters`: `MintOrBurnParams`) => `void` |
| `send` | (`__namedParameters`: `SendParams`) => `void` |

##### Defined in

[lib/party.ts:599](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L599)

___

#### assertBetween

▸ `Static` **assertBetween**<`T`\>(`property`, `lower`, `upper`): `void`

Constrain a property to lie between lower and upper bounds.

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `property` | `OrIgnore`<`ClosedInterval`<`T`\>\> | The property to constrain |
| `lower` | `T` | The lower bound |
| `upper` | `T` | The upper bound  Example: To constrain the account balance of a SmartContract to lie between 0 and 20 MINA, you can use  ```ts @method onlyRunsWhenBalanceIsLow() {   let lower = UInt64.zero;   let upper = UInt64.fromNumber(20e9);   Party.assertBetween(this.self.body.preconditions.account.balance, lower, upper);   // ... } ``` |

##### Returns

`void`

##### Defined in

[lib/party.ts:742](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L742)

___

#### assertEquals

▸ `Static` **assertEquals**<`T`\>(`property`, `value`): `void`

Fix a property to a certain value.

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `property` | `OrIgnore`<`T` \| `ClosedInterval`<`T`\>\> | The property to constrain |
| `value` | `T` | The value it is fixed to  Example: To fix the account nonce of a SmartContract to 0, you can use  ```ts @method onlyRunsWhenNonceIsZero() {   Party.assertEquals(this.self.body.preconditions.account.nonce, UInt32.zero);   // ... } ``` |

##### Returns

`void`

##### Defined in

[lib/party.ts:768](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L768)

___

#### clone

▸ `Static` **clone**(`party`): `any`

##### Parameters

| Name | Type |
| :------ | :------ |
| `party` | [`Party`](#classespartymd) |

##### Returns

`any`

##### Defined in

[lib/party.ts:589](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L589)

___

#### createSigned

▸ `Static` **createSigned**(`signer`): [`Party`](#classespartymd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `signer` | [`PrivateKey`](#classesprivatekeymd) |

##### Returns

[`Party`](#classespartymd)

##### Defined in

[lib/party.ts:897](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L897)

___

#### createUnsigned

▸ `Static` **createUnsigned**(`publicKey`): [`Party`](#classespartymd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | [`PublicKey`](#classestypespublickeymd) |

##### Returns

[`Party`](#classespartymd)

##### Defined in

[lib/party.ts:891](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L891)

___

#### defaultFeePayer

▸ `Static` **defaultFeePayer**(`address`, `key`, `nonce`): `FeePayerUnsigned`

##### Parameters

| Name | Type |
| :------ | :------ |
| `address` | [`PublicKey`](#classestypespublickeymd) |
| `key` | [`PrivateKey`](#classesprivatekeymd) |
| `nonce` | [`UInt32`](#classesuint32md) |

##### Returns

`FeePayerUnsigned`

##### Defined in

[lib/party.ts:873](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L873)

___

#### defaultParty

▸ `Static` **defaultParty**(`address`): [`Party`](#classespartymd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `address` | [`PublicKey`](#classestypespublickeymd) |

##### Returns

[`Party`](#classespartymd)

##### Defined in

[lib/party.ts:868](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L868)

___

#### dummyFeePayer

▸ `Static` **dummyFeePayer**(): `FeePayerUnsigned`

##### Returns

`FeePayerUnsigned`

##### Defined in

[lib/party.ts:886](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L886)

___

#### fundNewAccount

▸ `Static` **fundNewAccount**(`feePayerKey`, `initialBalance?`): `void`

Use this method to pay the account creation fee for another account.
Beware that you _don't_ need to pass in the new account!
Instead, the protocol will automatically identify accounts in your transaction that need funding.

If you provide an optional `initialBalance`, this will be subtracted from the fee-paying account as well,
but you have to separately ensure that it's added to the new account's balance.

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `feePayerKey` | [`PrivateKey`](#classesprivatekeymd) | the private key of the account that pays the fee |
| `initialBalance` | `Object` | the initial balance of the new account (default: 0) |
| `initialBalance.initialBalance` | `undefined` \| `string` \| `number` \| [`UInt64`](#classesuint64md) | - |

##### Returns

`void`

##### Defined in

[lib/party.ts:941](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L941)

___

#### getNonce

▸ `Static` **getNonce**(`party`, `fallbackToZero?`): [`UInt32`](#classesuint32md)

##### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `party` | [`Party`](#classespartymd) \| `FeePayerUnsigned` | `undefined` |
| `fallbackToZero` | `boolean` | `false` |

##### Returns

[`UInt32`](#classesuint32md)

##### Defined in

[lib/party.ts:805](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L805)

___

#### setValue

▸ `Static` **setValue**<`T`\>(`maybeValue`, `value`): `void`

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `maybeValue` | `SetOrKeep`<`T`\> |
| `value` | `T` |

##### Returns

`void`

##### Defined in

[lib/party.ts:720](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L720)

___

#### signFeePayerInPlace

▸ `Static` **signFeePayerInPlace**(`feePayer`, `privateKey?`, `fallbackToZeroNonce?`): `void`

##### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `feePayer` | `FeePayerUnsigned` | `undefined` |
| `privateKey?` | [`PrivateKey`](#classesprivatekeymd) | `undefined` |
| `fallbackToZeroNonce` | `boolean` | `false` |

##### Returns

`void`

##### Defined in

[lib/party.ts:794](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L794)

___

#### witness

▸ `Static` **witness**<`T`\>(`type`, `compute`, `skipCheck?`): `Object`

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `type` | [`AsFieldElements`](#interfacesasfieldelementsmd)<`T`\> | `undefined` |
| `compute` | () => { `party`: [`Party`](#classespartymd) ; `result`: `T`  } | `undefined` |
| `skipCheck` | `boolean` | `false` |

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `party` | [`Party`](#classespartymd) |
| `result` | `T` |

##### Defined in

[lib/party.ts:953](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L953)


<a name="classesprivatekeymd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / PrivateKey

## Class: PrivateKey

A signing key. You can generate one via [random](#random).

### Hierarchy

- [`CircuitValue`](#classescircuitvaluemd)

  ↳ **`PrivateKey`**

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [s](#s)

#### Methods

- [assertEquals](#assertequals)
- [equals](#equals)
- [isConstant](#isconstant)
- [toBase58](#tobase58)
- [toConstant](#toconstant)
- [toFields](#tofields)
- [toJSON](#tojson)
- [toPublicKey](#topublickey)
- [check](#check)
- [fromBase58](#frombase58)
- [fromJSON](#fromjson)
- [fromObject](#fromobject)
- [ofBits](#ofbits)
- [ofFields](#offields)
- [random](#random)
- [sizeInFields](#sizeinfields)
- [toBase58](#tobase58-1)
- [toConstant](#toconstant-1)
- [toFields](#tofields-1)
- [toInput](#toinput)
- [toJSON](#tojson-1)

### Constructors

#### constructor

• **new PrivateKey**(...`props`)

##### Parameters

| Name | Type |
| :------ | :------ |
| `...props` | `any`[] |

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[constructor](#constructor)

##### Defined in

[lib/circuit_value.ts:42](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L42)

### Properties

#### s

• **s**: [`Scalar`](#classesscalarmd)

##### Defined in

[lib/signature.ts:12](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L12)

### Methods

#### assertEquals

▸ **assertEquals**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`PrivateKey`](#classesprivatekeymd) |

##### Returns

`void`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[assertEquals](#assertequals)

##### Defined in

[lib/circuit_value.ts:126](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L126)

___

#### equals

▸ **equals**(`x`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`PrivateKey`](#classesprivatekeymd) |

##### Returns

[`Bool`](#classesboolmd)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[equals](#equals)

##### Defined in

[lib/circuit_value.ts:122](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L122)

___

#### isConstant

▸ **isConstant**(): `boolean`

##### Returns

`boolean`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[isConstant](#isconstant)

##### Defined in

[lib/circuit_value.ts:130](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L130)

___

#### toBase58

▸ **toBase58**(): `string`

##### Returns

`string`

##### Defined in

[lib/signature.ts:48](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L48)

___

#### toConstant

▸ **toConstant**(): [`PrivateKey`](#classesprivatekeymd)

##### Returns

[`PrivateKey`](#classesprivatekeymd)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant)

##### Defined in

[lib/circuit_value.ts:118](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L118)

___

#### toFields

▸ **toFields**(): [`Field`](#classesfieldmd)[]

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields)

##### Defined in

[lib/circuit_value.ts:110](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L110)

___

#### toJSON

▸ **toJSON**(): `JSONValue`

##### Returns

`JSONValue`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson)

##### Defined in

[lib/circuit_value.ts:114](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L114)

___

#### toPublicKey

▸ **toPublicKey**(): [`PublicKey`](#classestypespublickeymd)

Derives the associated public key.

##### Returns

[`PublicKey`](#classestypespublickeymd)

a [PublicKey](#publickey).

##### Defined in

[lib/signature.ts:40](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L40)

___

#### check

▸ `Static` **check**<`T`\>(`this`, `v`): `void`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`void`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[check](#check)

##### Defined in

[lib/circuit_value.ts:156](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L156)

___

#### fromBase58

▸ `Static` **fromBase58**(`privateKeyBase58`): [`PrivateKey`](#classesprivatekeymd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `privateKeyBase58` | `string` |

##### Returns

[`PrivateKey`](#classesprivatekeymd)

##### Defined in

[lib/signature.ts:44](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L44)

___

#### fromJSON

▸ `Static` **fromJSON**<`T`\>(`this`, `value`): ``null`` \| `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `JSONValue` |

##### Returns

``null`` \| `InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromJSON](#fromjson)

##### Defined in

[lib/circuit_value.ts:192](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L192)

___

#### fromObject

▸ `Static` **fromObject**<`T`\>(`this`, `value`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `NonMethods`<`InstanceType`<`T`\>\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromObject](#fromobject)

##### Defined in

[lib/circuit_value.ts:59](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L59)

___

#### ofBits

▸ `Static` **ofBits**(`bs`): [`PrivateKey`](#classesprivatekeymd)

Deserializes a list of bits into a [PrivateKey](#classesprivatekeymd).

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bs` | [`Bool`](#classesboolmd)[] | a list of [Bool](#classesboolmd)s. |

##### Returns

[`PrivateKey`](#classesprivatekeymd)

a [PrivateKey](#classesprivatekeymd).

##### Defined in

[lib/signature.ts:31](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L31)

___

#### ofFields

▸ `Static` **ofFields**<`T`\>(`this`, `xs`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `xs` | [`Field`](#classesfieldmd)[] |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[ofFields](#offields)

##### Defined in

[lib/circuit_value.ts:134](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L134)

___

#### random

▸ `Static` **random**(): [`PrivateKey`](#classesprivatekeymd)

You can use this method to generate a private key. You can then obtain
the associated public key via [toPublicKey](#topublickey). And generate signatures
via [Signature.create](#create).

##### Returns

[`PrivateKey`](#classesprivatekeymd)

a new [PrivateKey](#classesprivatekeymd).

##### Defined in

[lib/signature.ts:21](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L21)

___

#### sizeInFields

▸ `Static` **sizeInFields**(): `number`

##### Returns

`number`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[sizeInFields](#sizeinfields)

##### Defined in

[lib/circuit_value.ts:66](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L66)

___

#### toBase58

▸ `Static` **toBase58**(`privateKey`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `privateKey` | `Object` |
| `privateKey.s` | [`Scalar`](#classesscalarmd) |

##### Returns

`string`

##### Defined in

[lib/signature.ts:52](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L52)

___

#### toConstant

▸ `Static` **toConstant**<`T`\>(`this`, `t`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `t` | `InstanceType`<`T`\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant-1)

##### Defined in

[lib/circuit_value.ts:170](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L170)

___

#### toFields

▸ `Static` **toFields**<`T`\>(`this`, `v`): [`Field`](#classesfieldmd)[]

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields-1)

##### Defined in

[lib/circuit_value.ts:71](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L71)

___

#### toInput

▸ `Static` **toInput**<`T`\>(`this`, `v`): `HashInput`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`HashInput`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toInput](#toinput)

##### Defined in

[lib/circuit_value.ts:88](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L88)

___

#### toJSON

▸ `Static` **toJSON**<`T`\>(`this`, `v`): `JSONValue`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`JSONValue`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson-1)

##### Defined in

[lib/circuit_value.ts:178](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L178)


<a name="classesproofmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Proof

## Class: Proof<T\>

### Type parameters

| Name |
| :------ |
| `T` |

### Hierarchy

- **`Proof`**

  ↳ [`SelfProof`](#classesselfproofmd)

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [maxProofsVerified](#maxproofsverified)
- [proof](#proof)
- [publicInput](#publicinput)
- [shouldVerify](#shouldverify)
- [publicInputType](#publicinputtype)
- [tag](#tag)

#### Methods

- [toJSON](#tojson)
- [verify](#verify)
- [verifyIf](#verifyif)
- [fromJSON](#fromjson)

### Constructors

#### constructor

• **new Proof**<`T`\>(`__namedParameters`)

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | `Object` |
| `__namedParameters.maxProofsVerified` | ``0`` \| ``2`` \| ``1`` |
| `__namedParameters.proof` | `unknown` |
| `__namedParameters.publicInput` | `T` |

##### Defined in

[lib/proof_system.ts:91](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L91)

### Properties

#### maxProofsVerified

• **maxProofsVerified**: ``0`` \| ``2`` \| ``1``

##### Defined in

[lib/proof_system.ts:58](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L58)

___

#### proof

• **proof**: `unknown`

##### Defined in

[lib/proof_system.ts:57](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L57)

___

#### publicInput

• **publicInput**: `T`

##### Defined in

[lib/proof_system.ts:56](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L56)

___

#### shouldVerify

• **shouldVerify**: [`Bool`](#classesboolmd)

##### Defined in

[lib/proof_system.ts:59](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L59)

___

#### publicInputType

▪ `Static` **publicInputType**: [`AsFieldElements`](#interfacesasfieldelementsmd)<`any`\>

##### Defined in

[lib/proof_system.ts:49](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L49)

___

#### tag

▪ `Static` **tag**: () => { `name`: `string`  }

##### Type declaration

▸ (): `Object`

###### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `name` | `string` |

##### Defined in

[lib/proof_system.ts:50](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L50)

### Methods

#### toJSON

▸ **toJSON**(): `JsonProof`

##### Returns

`JsonProof`

##### Defined in

[lib/proof_system.ts:67](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L67)

___

#### verify

▸ **verify**(): `void`

##### Returns

`void`

##### Defined in

[lib/proof_system.ts:61](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L61)

___

#### verifyIf

▸ **verifyIf**(`condition`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `condition` | [`Bool`](#classesboolmd) |

##### Returns

`void`

##### Defined in

[lib/proof_system.ts:64](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L64)

___

#### fromJSON

▸ `Static` **fromJSON**<`S`\>(`this`, `__namedParameters`): [`Proof`](#classesproofmd)<`InferInstance`<`S`[``"publicInputType"``]\>\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `S` | extends `Subclass`<typeof [`Proof`](#classesproofmd)\> |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `S` |
| `__namedParameters` | `JsonProof` |

##### Returns

[`Proof`](#classesproofmd)<`InferInstance`<`S`[``"publicInputType"``]\>\>

##### Defined in

[lib/proof_system.ts:76](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L76)


<a name="classesscalarmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Scalar

## Class: Scalar

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Methods

- [add](#add)
- [div](#div)
- [mul](#mul)
- [neg](#neg)
- [sub](#sub)
- [toFields](#tofields)
- [toJSON](#tojson)
- [check](#check)
- [fromJSON](#fromjson)
- [ofBits](#ofbits)
- [ofFields](#offields)
- [random](#random)
- [sizeInFields](#sizeinfields)
- [toFields](#tofields-1)
- [toJSON](#tojson-1)

### Constructors

#### constructor

• **new Scalar**()

### Methods

#### add

▸ **add**(`y`): [`Scalar`](#classesscalarmd)

Add scalar field elements.
Can only be called outside of circuit execution

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`Scalar`](#classesscalarmd) |

##### Returns

[`Scalar`](#classesscalarmd)

##### Defined in

[snarky.d.ts:593](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L593)

___

#### div

▸ **div**(`y`): [`Scalar`](#classesscalarmd)

Divide scalar field elements.
Can only be called outside of circuit execution

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`Scalar`](#classesscalarmd) |

##### Returns

[`Scalar`](#classesscalarmd)

##### Defined in

[snarky.d.ts:611](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L611)

___

#### mul

▸ **mul**(`y`): [`Scalar`](#classesscalarmd)

Multiply scalar field elements.
Can only be called outside of circuit execution

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`Scalar`](#classesscalarmd) |

##### Returns

[`Scalar`](#classesscalarmd)

##### Defined in

[snarky.d.ts:605](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L605)

___

#### neg

▸ **neg**(): [`Scalar`](#classesscalarmd)

Negate a scalar field element.
Can only be called outside of circuit execution

##### Returns

[`Scalar`](#classesscalarmd)

##### Defined in

[snarky.d.ts:587](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L587)

___

#### sub

▸ **sub**(`y`): [`Scalar`](#classesscalarmd)

Subtract scalar field elements.
Can only be called outside of circuit execution

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`Scalar`](#classesscalarmd) |

##### Returns

[`Scalar`](#classesscalarmd)

##### Defined in

[snarky.d.ts:599](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L599)

___

#### toFields

▸ **toFields**(`this`): [`Field`](#classesfieldmd)[]

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | [`Scalar`](#classesscalarmd) |

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[snarky.d.ts:581](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L581)

___

#### toJSON

▸ **toJSON**(): `JSONValue`

##### Returns

`JSONValue`

##### Defined in

[snarky.d.ts:613](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L613)

___

#### check

▸ `Static` **check**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Scalar`](#classesscalarmd) |

##### Returns

`void`

##### Defined in

[snarky.d.ts:623](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L623)

___

#### fromJSON

▸ `Static` **fromJSON**(`x`): ``null`` \| [`Scalar`](#classesscalarmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `JSONValue` |

##### Returns

``null`` \| [`Scalar`](#classesscalarmd)

##### Defined in

[snarky.d.ts:622](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L622)

___

#### ofBits

▸ `Static` **ofBits**(`bits`): [`Scalar`](#classesscalarmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `bits` | [`Bool`](#classesboolmd)[] |

##### Returns

[`Scalar`](#classesscalarmd)

##### Defined in

[snarky.d.ts:618](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L618)

___

#### ofFields

▸ `Static` **ofFields**(`fields`): [`Scalar`](#classesscalarmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `fields` | [`Field`](#classesfieldmd)[] |

##### Returns

[`Scalar`](#classesscalarmd)

##### Defined in

[snarky.d.ts:616](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L616)

___

#### random

▸ `Static` **random**(): [`Scalar`](#classesscalarmd)

##### Returns

[`Scalar`](#classesscalarmd)

##### Defined in

[snarky.d.ts:619](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L619)

___

#### sizeInFields

▸ `Static` **sizeInFields**(): `number`

##### Returns

`number`

##### Defined in

[snarky.d.ts:617](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L617)

___

#### toFields

▸ `Static` **toFields**(`x`): [`Field`](#classesfieldmd)[]

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Scalar`](#classesscalarmd) |

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[snarky.d.ts:615](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L615)

___

#### toJSON

▸ `Static` **toJSON**(`x`): `JSONValue`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Scalar`](#classesscalarmd) |

##### Returns

`JSONValue`

##### Defined in

[snarky.d.ts:621](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L621)


<a name="classesselfproofmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / SelfProof

## Class: SelfProof<T\>

### Type parameters

| Name |
| :------ |
| `T` |

### Hierarchy

- [`Proof`](#classesproofmd)<`T`\>

  ↳ **`SelfProof`**

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [maxProofsVerified](#maxproofsverified)
- [proof](#proof)
- [publicInput](#publicinput)
- [shouldVerify](#shouldverify)
- [publicInputType](#publicinputtype)
- [tag](#tag)

#### Methods

- [toJSON](#tojson)
- [verify](#verify)
- [verifyIf](#verifyif)
- [fromJSON](#fromjson)

### Constructors

#### constructor

• **new SelfProof**<`T`\>(`__namedParameters`)

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | `Object` |
| `__namedParameters.maxProofsVerified` | ``0`` \| ``2`` \| ``1`` |
| `__namedParameters.proof` | `unknown` |
| `__namedParameters.publicInput` | `T` |

##### Inherited from

[Proof](#classesproofmd).[constructor](#constructor)

##### Defined in

[lib/proof_system.ts:91](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L91)

### Properties

#### maxProofsVerified

• **maxProofsVerified**: ``0`` \| ``2`` \| ``1``

##### Inherited from

[Proof](#classesproofmd).[maxProofsVerified](#maxproofsverified)

##### Defined in

[lib/proof_system.ts:58](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L58)

___

#### proof

• **proof**: `unknown`

##### Inherited from

[Proof](#classesproofmd).[proof](#proof)

##### Defined in

[lib/proof_system.ts:57](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L57)

___

#### publicInput

• **publicInput**: `T`

##### Inherited from

[Proof](#classesproofmd).[publicInput](#publicinput)

##### Defined in

[lib/proof_system.ts:56](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L56)

___

#### shouldVerify

• **shouldVerify**: [`Bool`](#classesboolmd)

##### Inherited from

[Proof](#classesproofmd).[shouldVerify](#shouldverify)

##### Defined in

[lib/proof_system.ts:59](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L59)

___

#### publicInputType

▪ `Static` **publicInputType**: [`AsFieldElements`](#interfacesasfieldelementsmd)<`any`\>

##### Inherited from

[Proof](#classesproofmd).[publicInputType](#publicinputtype)

##### Defined in

[lib/proof_system.ts:49](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L49)

___

#### tag

▪ `Static` **tag**: () => { `name`: `string`  }

##### Type declaration

▸ (): `Object`

###### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `name` | `string` |

##### Inherited from

[Proof](#classesproofmd).[tag](#tag)

##### Defined in

[lib/proof_system.ts:50](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L50)

### Methods

#### toJSON

▸ **toJSON**(): `JsonProof`

##### Returns

`JsonProof`

##### Inherited from

[Proof](#classesproofmd).[toJSON](#tojson)

##### Defined in

[lib/proof_system.ts:67](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L67)

___

#### verify

▸ **verify**(): `void`

##### Returns

`void`

##### Inherited from

[Proof](#classesproofmd).[verify](#verify)

##### Defined in

[lib/proof_system.ts:61](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L61)

___

#### verifyIf

▸ **verifyIf**(`condition`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `condition` | [`Bool`](#classesboolmd) |

##### Returns

`void`

##### Inherited from

[Proof](#classesproofmd).[verifyIf](#verifyif)

##### Defined in

[lib/proof_system.ts:64](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L64)

___

#### fromJSON

▸ `Static` **fromJSON**<`S`\>(`this`, `__namedParameters`): [`Proof`](#classesproofmd)<`InferInstance`<`S`[``"publicInputType"``]\>\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `S` | extends `Subclass`<typeof [`Proof`](#classesproofmd)\> |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `S` |
| `__namedParameters` | `JsonProof` |

##### Returns

[`Proof`](#classesproofmd)<`InferInstance`<`S`[``"publicInputType"``]\>\>

##### Inherited from

[Proof](#classesproofmd).[fromJSON](#fromjson)

##### Defined in

[lib/proof_system.ts:76](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L76)


<a name="classessignmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Sign

## Class: Sign

### Hierarchy

- [`CircuitValue`](#classescircuitvaluemd)

  ↳ **`Sign`**

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [value](#value)

#### Accessors

- [minusOne](#minusone)
- [one](#one)

#### Methods

- [assertEquals](#assertequals)
- [equals](#equals)
- [isConstant](#isconstant)
- [isPositive](#ispositive)
- [mul](#mul)
- [neg](#neg)
- [toConstant](#toconstant)
- [toFields](#tofields)
- [toJSON](#tojson)
- [toString](#tostring)
- [check](#check)
- [fromJSON](#fromjson)
- [fromObject](#fromobject)
- [ofFields](#offields)
- [sizeInFields](#sizeinfields)
- [toConstant](#toconstant-1)
- [toFields](#tofields-1)
- [toInput](#toinput)
- [toJSON](#tojson-1)

### Constructors

#### constructor

• **new Sign**(...`props`)

##### Parameters

| Name | Type |
| :------ | :------ |
| `...props` | `any`[] |

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[constructor](#constructor)

##### Defined in

[lib/circuit_value.ts:42](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L42)

### Properties

#### value

• **value**: [`Field`](#classesfieldmd)

##### Defined in

[lib/int.ts:369](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L369)

### Accessors

#### minusOne

• `Static` `get` **minusOne**(): [`Sign`](#classessignmd)

##### Returns

[`Sign`](#classessignmd)

##### Defined in

[lib/int.ts:374](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L374)

___

#### one

• `Static` `get` **one**(): [`Sign`](#classessignmd)

##### Returns

[`Sign`](#classessignmd)

##### Defined in

[lib/int.ts:371](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L371)

### Methods

#### assertEquals

▸ **assertEquals**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Sign`](#classessignmd) |

##### Returns

`void`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[assertEquals](#assertequals)

##### Defined in

[lib/circuit_value.ts:126](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L126)

___

#### equals

▸ **equals**(`x`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Sign`](#classessignmd) |

##### Returns

[`Bool`](#classesboolmd)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[equals](#equals)

##### Defined in

[lib/circuit_value.ts:122](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L122)

___

#### isConstant

▸ **isConstant**(): `boolean`

##### Returns

`boolean`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[isConstant](#isconstant)

##### Defined in

[lib/circuit_value.ts:130](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L130)

___

#### isPositive

▸ **isPositive**(): [`Bool`](#classesboolmd)

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[lib/int.ts:395](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L395)

___

#### mul

▸ **mul**(`y`): [`Sign`](#classessignmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`Sign`](#classessignmd) |

##### Returns

[`Sign`](#classessignmd)

##### Defined in

[lib/int.ts:392](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L392)

___

#### neg

▸ **neg**(): [`Sign`](#classessignmd)

##### Returns

[`Sign`](#classessignmd)

##### Defined in

[lib/int.ts:389](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L389)

___

#### toConstant

▸ **toConstant**(): [`Sign`](#classessignmd)

##### Returns

[`Sign`](#classessignmd)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant)

##### Defined in

[lib/circuit_value.ts:118](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L118)

___

#### toFields

▸ **toFields**(): [`Field`](#classesfieldmd)[]

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields)

##### Defined in

[lib/circuit_value.ts:110](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L110)

___

#### toJSON

▸ **toJSON**(): `JSONValue`

##### Returns

`JSONValue`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson)

##### Defined in

[lib/circuit_value.ts:114](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L114)

___

#### toString

▸ **toString**(): `string`

##### Returns

`string`

##### Defined in

[lib/int.ts:398](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L398)

___

#### check

▸ `Static` **check**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Sign`](#classessignmd) |

##### Returns

`void`

##### Overrides

[CircuitValue](#classescircuitvaluemd).[check](#check)

##### Defined in

[lib/int.ts:377](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L377)

___

#### fromJSON

▸ `Static` **fromJSON**<`T`\>(`this`, `value`): ``null`` \| `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `JSONValue` |

##### Returns

``null`` \| `InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromJSON](#fromjson)

##### Defined in

[lib/circuit_value.ts:192](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L192)

___

#### fromObject

▸ `Static` **fromObject**<`T`\>(`this`, `value`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `NonMethods`<`InstanceType`<`T`\>\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromObject](#fromobject)

##### Defined in

[lib/circuit_value.ts:59](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L59)

___

#### ofFields

▸ `Static` **ofFields**<`T`\>(`this`, `xs`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `xs` | [`Field`](#classesfieldmd)[] |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[ofFields](#offields)

##### Defined in

[lib/circuit_value.ts:134](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L134)

___

#### sizeInFields

▸ `Static` **sizeInFields**(): `number`

##### Returns

`number`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[sizeInFields](#sizeinfields)

##### Defined in

[lib/circuit_value.ts:66](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L66)

___

#### toConstant

▸ `Static` **toConstant**<`T`\>(`this`, `t`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `t` | `InstanceType`<`T`\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant-1)

##### Defined in

[lib/circuit_value.ts:170](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L170)

___

#### toFields

▸ `Static` **toFields**<`T`\>(`this`, `v`): [`Field`](#classesfieldmd)[]

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields-1)

##### Defined in

[lib/circuit_value.ts:71](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L71)

___

#### toInput

▸ `Static` **toInput**(`x`): `HashInput`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Sign`](#classessignmd) |

##### Returns

`HashInput`

##### Overrides

[CircuitValue](#classescircuitvaluemd).[toInput](#toinput)

##### Defined in

[lib/int.ts:381](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L381)

___

#### toJSON

▸ `Static` **toJSON**(`x`): ``"Positive"`` \| ``"Negative"``

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Sign`](#classessignmd) |

##### Returns

``"Positive"`` \| ``"Negative"``

##### Overrides

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson-1)

##### Defined in

[lib/int.ts:384](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L384)


<a name="classessignaturemd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Signature

## Class: Signature

### Hierarchy

- [`CircuitValue`](#classescircuitvaluemd)

  ↳ **`Signature`**

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [r](#r)
- [s](#s)

#### Methods

- [assertEquals](#assertequals)
- [equals](#equals)
- [isConstant](#isconstant)
- [toConstant](#toconstant)
- [toFields](#tofields)
- [toJSON](#tojson)
- [verify](#verify)
- [check](#check)
- [create](#create)
- [fromJSON](#fromjson)
- [fromObject](#fromobject)
- [ofFields](#offields)
- [sizeInFields](#sizeinfields)
- [toConstant](#toconstant-1)
- [toFields](#tofields-1)
- [toInput](#toinput)
- [toJSON](#tojson-1)

### Constructors

#### constructor

• **new Signature**(...`props`)

##### Parameters

| Name | Type |
| :------ | :------ |
| `...props` | `any`[] |

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[constructor](#constructor)

##### Defined in

[lib/circuit_value.ts:42](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L42)

### Properties

#### r

• **r**: [`Field`](#classesfieldmd)

##### Defined in

[lib/signature.ts:118](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L118)

___

#### s

• **s**: [`Scalar`](#classesscalarmd)

##### Defined in

[lib/signature.ts:119](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L119)

### Methods

#### assertEquals

▸ **assertEquals**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Signature`](#classessignaturemd) |

##### Returns

`void`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[assertEquals](#assertequals)

##### Defined in

[lib/circuit_value.ts:126](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L126)

___

#### equals

▸ **equals**(`x`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Signature`](#classessignaturemd) |

##### Returns

[`Bool`](#classesboolmd)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[equals](#equals)

##### Defined in

[lib/circuit_value.ts:122](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L122)

___

#### isConstant

▸ **isConstant**(): `boolean`

##### Returns

`boolean`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[isConstant](#isconstant)

##### Defined in

[lib/circuit_value.ts:130](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L130)

___

#### toConstant

▸ **toConstant**(): [`Signature`](#classessignaturemd)

##### Returns

[`Signature`](#classessignaturemd)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant)

##### Defined in

[lib/circuit_value.ts:118](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L118)

___

#### toFields

▸ **toFields**(): [`Field`](#classesfieldmd)[]

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields)

##### Defined in

[lib/circuit_value.ts:110](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L110)

___

#### toJSON

▸ **toJSON**(): `JSONValue`

##### Returns

`JSONValue`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson)

##### Defined in

[lib/circuit_value.ts:114](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L114)

___

#### verify

▸ **verify**(`publicKey`, `msg`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | [`PublicKey`](#classestypespublickeymd) |
| `msg` | [`Field`](#classesfieldmd)[] |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[lib/signature.ts:134](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L134)

___

#### check

▸ `Static` **check**<`T`\>(`this`, `v`): `void`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`void`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[check](#check)

##### Defined in

[lib/circuit_value.ts:156](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L156)

___

#### create

▸ `Static` **create**(`privKey`, `msg`): [`Signature`](#classessignaturemd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `privKey` | [`PrivateKey`](#classesprivatekeymd) |
| `msg` | [`Field`](#classesfieldmd)[] |

##### Returns

[`Signature`](#classessignaturemd)

##### Defined in

[lib/signature.ts:121](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L121)

___

#### fromJSON

▸ `Static` **fromJSON**<`T`\>(`this`, `value`): ``null`` \| `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `JSONValue` |

##### Returns

``null`` \| `InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromJSON](#fromjson)

##### Defined in

[lib/circuit_value.ts:192](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L192)

___

#### fromObject

▸ `Static` **fromObject**<`T`\>(`this`, `value`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `NonMethods`<`InstanceType`<`T`\>\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromObject](#fromobject)

##### Defined in

[lib/circuit_value.ts:59](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L59)

___

#### ofFields

▸ `Static` **ofFields**<`T`\>(`this`, `xs`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `xs` | [`Field`](#classesfieldmd)[] |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[ofFields](#offields)

##### Defined in

[lib/circuit_value.ts:134](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L134)

___

#### sizeInFields

▸ `Static` **sizeInFields**(): `number`

##### Returns

`number`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[sizeInFields](#sizeinfields)

##### Defined in

[lib/circuit_value.ts:66](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L66)

___

#### toConstant

▸ `Static` **toConstant**<`T`\>(`this`, `t`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `t` | `InstanceType`<`T`\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant-1)

##### Defined in

[lib/circuit_value.ts:170](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L170)

___

#### toFields

▸ `Static` **toFields**<`T`\>(`this`, `v`): [`Field`](#classesfieldmd)[]

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields-1)

##### Defined in

[lib/circuit_value.ts:71](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L71)

___

#### toInput

▸ `Static` **toInput**<`T`\>(`this`, `v`): `HashInput`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`HashInput`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toInput](#toinput)

##### Defined in

[lib/circuit_value.ts:88](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L88)

___

#### toJSON

▸ `Static` **toJSON**<`T`\>(`this`, `v`): `JSONValue`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`JSONValue`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson-1)

##### Defined in

[lib/circuit_value.ts:178](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L178)


<a name="classessmartcontractmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / SmartContract

## Class: SmartContract

The main zkapp class. To write a zkapp, extend this class as such:

```
class YourSmartContract extends SmartContract {
  // your smart contract code here
}
```

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [\_executionState](#_executionstate)
- [address](#address)
- [events](#events)
- [\_maxProofsVerified](#_maxproofsverified)
- [\_methodMetadata](#_methodmetadata)
- [\_methods](#_methods)
- [\_provers](#_provers)
- [\_verificationKey](#_verificationkey)

#### Accessors

- [account](#account)
- [balance](#balance)
- [experimental](#experimental)
- [network](#network)
- [nonce](#nonce)
- [self](#self)
- [tokenId](#tokenid)
- [tokenSymbol](#tokensymbol)
- [Proof](#proof)

#### Methods

- [deploy](#deploy)
- [emitEvent](#emitevent)
- [executionState](#executionstate)
- [fetchEvents](#fetchevents)
- [send](#send)
- [setPermissions](#setpermissions)
- [setValue](#setvalue)
- [sign](#sign)
- [analyzeMethods](#analyzemethods)
- [compile](#compile)
- [digest](#digest)
- [runOutsideCircuit](#runoutsidecircuit)

### Constructors

#### constructor

• **new SmartContract**(`address`)

##### Parameters

| Name | Type |
| :------ | :------ |
| `address` | [`PublicKey`](#classestypespublickeymd) |

##### Defined in

[lib/zkapp.ts:453](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L453)

### Properties

#### \_executionState

• `Private` **\_executionState**: `undefined` \| `ExecutionState`

##### Defined in

[lib/zkapp.ts:435](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L435)

___

#### address

• **address**: [`PublicKey`](#classestypespublickeymd)

##### Defined in

[lib/zkapp.ts:433](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L433)

___

#### events

• **events**: `Object` = `{}`

##### Index signature

▪ [key: `string`]: [`AsFieldElements`](#interfacesasfieldelementsmd)<`any`\>

##### Defined in

[lib/zkapp.ts:591](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L591)

___

#### \_maxProofsVerified

▪ `Static` `Optional` **\_maxProofsVerified**: ``0`` \| ``2`` \| ``1``

##### Defined in

[lib/zkapp.ts:442](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L442)

___

#### \_methodMetadata

▪ `Static` `Private` **\_methodMetadata**: `Record`<`string`, { `digest`: `string` ; `hasReturn`: `boolean` ; `rows`: `number` ; `sequenceEvents`: `number`  }\> = `{}`

##### Defined in

[lib/zkapp.ts:437](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L437)

___

#### \_methods

▪ `Static` `Optional` **\_methods**: `MethodInterface`[]

##### Defined in

[lib/zkapp.ts:436](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L436)

___

#### \_provers

▪ `Static` `Optional` **\_provers**: `Prover`[]

##### Defined in

[lib/zkapp.ts:441](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L441)

___

#### \_verificationKey

▪ `Static` `Optional` **\_verificationKey**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `data` | `string` |
| `hash` | [`Field`](#classesfieldmd) |

##### Defined in

[lib/zkapp.ts:443](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L443)

### Accessors

#### account

• `get` **account**(): `PreconditionClassType`<`AccountPrecondition`\>

##### Returns

`PreconditionClassType`<`AccountPrecondition`\>

##### Defined in

[lib/zkapp.ts:554](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L554)

___

#### balance

• `get` **balance**(): `Object`

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `addInPlace` | (`x`: `string` \| `number` \| `bigint` \| [`UInt32`](#classesuint32md) \| [`UInt64`](#classesuint64md) \| [`Int64`](#classesint64md)) => `void` |
| `subInPlace` | (`x`: `string` \| `number` \| `bigint` \| [`UInt32`](#classesuint32md) \| [`UInt64`](#classesuint64md) \| [`Int64`](#classesint64md)) => `void` |

##### Defined in

[lib/zkapp.ts:583](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L583)

___

#### experimental

• `get` **experimental**(): `Object`

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| ``get` **token**(): `Object`` | {} |

##### Defined in

[lib/zkapp.ts:562](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L562)

___

#### network

• `get` **network**(): `PreconditionClassType`<{ `blockchainLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceGenesis`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceHardFork`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `minWindowDensity`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `nextEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `snarkedLedgerHash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `stakingEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `timestamp`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  }\>

##### Returns

`PreconditionClassType`<{ `blockchainLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceGenesis`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceHardFork`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `minWindowDensity`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `nextEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `snarkedLedgerHash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `stakingEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `timestamp`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  }\>

##### Defined in

[lib/zkapp.ts:558](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L558)

___

#### nonce

• `get` **nonce**(): [`UInt32`](#classesuint32md)

##### Returns

[`UInt32`](#classesuint32md)

##### Defined in

[lib/zkapp.ts:587](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L587)

___

#### self

• `get` **self**(): [`Party`](#classespartymd)

##### Returns

[`Party`](#classespartymd)

##### Defined in

[lib/zkapp.ts:550](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L550)

___

#### tokenId

• `get` **tokenId**(): [`Field`](#classesfieldmd)

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[lib/zkapp.ts:575](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L575)

___

#### tokenSymbol

• `get` **tokenSymbol**(): `Object`

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `set` | (`tokenSymbol`: `string`) => `void` |

##### Defined in

[lib/zkapp.ts:579](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L579)

___

#### Proof

• `Static` `get` **Proof**(): typeof `__class`

##### Returns

typeof `__class`

##### Defined in

[lib/zkapp.ts:445](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L445)

### Methods

#### deploy

▸ **deploy**(`__namedParameters`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | `Object` |
| `__namedParameters.verificationKey?` | `Object` |
| `__namedParameters.verificationKey.data` | `string` |
| `__namedParameters.verificationKey.hash` | `string` \| [`Field`](#classesfieldmd) |
| `__namedParameters.zkappKey?` | [`PrivateKey`](#classesprivatekeymd) |

##### Returns

`void`

##### Defined in

[lib/zkapp.ts:504](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L504)

___

#### emitEvent

▸ **emitEvent**<`K`\>(`type`, `event`): `void`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `K` | extends `string` \| `number` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `type` | `K` |
| `event` | `any` |

##### Returns

`void`

##### Defined in

[lib/zkapp.ts:594](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L594)

___

#### executionState

▸ `Private` **executionState**(): `ExecutionState`

##### Returns

`ExecutionState`

##### Defined in

[lib/zkapp.ts:525](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L525)

___

#### fetchEvents

▸ **fetchEvents**(`start?`, `end?`): `Promise`<{ `event`: [`AsFieldElements`](#interfacesasfieldelementsmd)<`any`\> ; `type`: `string`  }[]\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `start` | [`UInt32`](#classesuint32md) |
| `end?` | [`UInt32`](#classesuint32md) |

##### Returns

`Promise`<{ `event`: [`AsFieldElements`](#interfacesasfieldelementsmd)<`any`\> ; `type`: `string`  }[]\>

##### Defined in

[lib/zkapp.ts:624](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L624)

___

#### send

▸ **send**(`args`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `args` | `Omit`<`SendParams`, ``"from"``\> |

##### Returns

`void`

##### Defined in

[lib/zkapp.ts:571](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L571)

___

#### setPermissions

▸ **setPermissions**(`permissions`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `permissions` | [`Permissions`](#permissions) |

##### Returns

`void`

##### Defined in

[lib/zkapp.ts:715](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L715)

___

#### setValue

▸ **setValue**<`T`\>(`maybeValue`, `value`): `void`

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `maybeValue` | `SetOrKeep`<`T`\> |
| `value` | `T` |

##### Returns

`void`

##### Defined in

[lib/zkapp.ts:709](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L709)

___

#### sign

▸ **sign**(`zkappKey?`, `fallbackToZeroNonce?`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `zkappKey?` | [`PrivateKey`](#classesprivatekeymd) |
| `fallbackToZeroNonce?` | `boolean` |

##### Returns

`void`

##### Defined in

[lib/zkapp.ts:521](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L521)

___

#### analyzeMethods

▸ `Static` **analyzeMethods**(`address`): `Record`<`string`, { `digest`: `string` ; `hasReturn`: `boolean` ; `rows`: `number` ; `sequenceEvents`: `number`  }\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `address` | [`PublicKey`](#classestypespublickeymd) |

##### Returns

`Record`<`string`, { `digest`: `string` ; `hasReturn`: `boolean` ; `rows`: `number` ; `sequenceEvents`: `number`  }\>

##### Defined in

[lib/zkapp.ts:675](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L675)

___

#### compile

▸ `Static` **compile**(`address`): `Promise`<{ `provers`: `Prover`[] ; `verificationKey`: { `data`: `string` ; `hash`: `string`  } ; `verify`: (`publicInput`: `PublicInput`, `proof`: `unknown`) => `Promise`<`boolean`\>  }\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `address` | [`PublicKey`](#classestypespublickeymd) |

##### Returns

`Promise`<{ `provers`: `Prover`[] ; `verificationKey`: { `data`: `string` ; `hash`: `string`  } ; `verify`: (`publicInput`: `PublicInput`, `proof`: `unknown`) => `Promise`<`boolean`\>  }\>

##### Defined in

[lib/zkapp.ts:465](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L465)

___

#### digest

▸ `Static` **digest**(`address`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `address` | [`PublicKey`](#classestypespublickeymd) |

##### Returns

`string`

##### Defined in

[lib/zkapp.ts:495](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L495)

___

#### runOutsideCircuit

▸ `Static` **runOutsideCircuit**(`run`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `run` | () => `void` |

##### Returns

`void`

##### Defined in

[lib/zkapp.ts:668](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L668)


<a name="classestokenmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Token

## Class: Token

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [id](#id)
- [parentTokenId](#parenttokenid)
- [tokenOwner](#tokenowner)
- [Id](#id-1)

### Constructors

#### constructor

• **new Token**(`options`)

##### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `Object` |
| `options.parentTokenId?` | [`Field`](#classesfieldmd) |
| `options.tokenOwner` | [`PublicKey`](#classestypespublickeymd) |

##### Defined in

[lib/party.ts:529](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L529)

### Properties

#### id

• `Readonly` **id**: [`Field`](#classesfieldmd)

##### Defined in

[lib/party.ts:523](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L523)

___

#### parentTokenId

• `Readonly` **parentTokenId**: [`Field`](#classesfieldmd)

##### Defined in

[lib/party.ts:524](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L524)

___

#### tokenOwner

• `Readonly` **tokenOwner**: [`PublicKey`](#classestypespublickeymd)

##### Defined in

[lib/party.ts:525](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L525)

___

#### Id

▪ `Static` **Id**: `Object` = `TokenId`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `default` | [`Field`](#classesfieldmd) |
| `check` | (`x`: `T`) => `void` |
| `fromBase58` | (`base58`: `string`) => [`Field`](#classesfieldmd) |
| `ofFields` | (`x`: [`Field`](#classesfieldmd)[]) => `T` |
| `sizeInFields` | () => `number` |
| `toBase58` | (`field`: [`Field`](#classesfieldmd)) => `string` |
| `toFields` | (`x`: `T`) => [`Field`](#classesfieldmd)[] |
| `toInput` | (`x`: `T`) => { `fields?`: [`Field`](#classesfieldmd)[] ; `packed?`: [[`Field`](#classesfieldmd), `number`][]  } |
| `toJSON` | (`x`: `T`) => `JSONValue` |

##### Defined in

[lib/party.ts:527](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L527)


<a name="classestypespublickeymd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / [Types](#modulestypesmd) / PublicKey

## Class: PublicKey

[Types](#modulestypesmd).PublicKey

### Hierarchy

- [`CircuitValue`](#classescircuitvaluemd)

  ↳ **`PublicKey`**

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [isOdd](#isodd)
- [x](#x)

#### Methods

- [assertEquals](#assertequals)
- [equals](#equals)
- [isConstant](#isconstant)
- [isEmpty](#isempty)
- [toBase58](#tobase58)
- [toConstant](#toconstant)
- [toFields](#tofields)
- [toGroup](#togroup)
- [toJSON](#tojson)
- [check](#check)
- [empty](#empty)
- [from](#from)
- [fromBase58](#frombase58)
- [fromGroup](#fromgroup)
- [fromJSON](#fromjson)
- [fromObject](#fromobject)
- [fromPrivateKey](#fromprivatekey)
- [ofFields](#offields)
- [sizeInFields](#sizeinfields)
- [toBase58](#tobase58-1)
- [toConstant](#toconstant-1)
- [toFields](#tofields-1)
- [toInput](#toinput)
- [toJSON](#tojson-1)

### Constructors

#### constructor

• **new PublicKey**(...`props`)

##### Parameters

| Name | Type |
| :------ | :------ |
| `...props` | `any`[] |

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[constructor](#constructor)

##### Defined in

[lib/circuit_value.ts:42](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L42)

### Properties

#### isOdd

• **isOdd**: [`Bool`](#classesboolmd)

##### Defined in

[lib/signature.ts:60](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L60)

___

#### x

• **x**: [`Field`](#classesfieldmd)

##### Defined in

[lib/signature.ts:59](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L59)

### Methods

#### assertEquals

▸ **assertEquals**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`PublicKey`](#classestypespublickeymd) |

##### Returns

`void`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[assertEquals](#assertequals)

##### Defined in

[lib/circuit_value.ts:126](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L126)

___

#### equals

▸ **equals**(`x`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`PublicKey`](#classestypespublickeymd) |

##### Returns

[`Bool`](#classesboolmd)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[equals](#equals)

##### Defined in

[lib/circuit_value.ts:122](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L122)

___

#### isConstant

▸ **isConstant**(): `boolean`

##### Returns

`boolean`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[isConstant](#isconstant)

##### Defined in

[lib/circuit_value.ts:130](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L130)

___

#### isEmpty

▸ **isEmpty**(): [`Bool`](#classesboolmd)

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[lib/signature.ts:93](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L93)

___

#### toBase58

▸ **toBase58**(): `string`

##### Returns

`string`

##### Defined in

[lib/signature.ts:102](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L102)

___

#### toConstant

▸ **toConstant**(): [`PublicKey`](#classestypespublickeymd)

##### Returns

[`PublicKey`](#classestypespublickeymd)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant)

##### Defined in

[lib/circuit_value.ts:118](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L118)

___

#### toFields

▸ **toFields**(): [`Field`](#classesfieldmd)[]

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields)

##### Defined in

[lib/circuit_value.ts:110](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L110)

___

#### toGroup

▸ **toGroup**(): [`Group`](#classesgroupmd)

##### Returns

[`Group`](#classesgroupmd)

##### Defined in

[lib/signature.ts:62](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L62)

___

#### toJSON

▸ **toJSON**(): `JSONValue`

##### Returns

`JSONValue`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson)

##### Defined in

[lib/circuit_value.ts:114](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L114)

___

#### check

▸ `Static` **check**<`T`\>(`this`, `v`): `void`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`void`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[check](#check)

##### Defined in

[lib/circuit_value.ts:156](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L156)

___

#### empty

▸ `Static` **empty**(): [`PublicKey`](#classestypespublickeymd)

##### Returns

[`PublicKey`](#classestypespublickeymd)

##### Defined in

[lib/signature.ts:89](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L89)

___

#### from

▸ `Static` **from**(`g`): [`PublicKey`](#classestypespublickeymd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `g` | `Object` |
| `g.isOdd` | [`Bool`](#classesboolmd) |
| `g.x` | [`Field`](#classesfieldmd) |

##### Returns

[`PublicKey`](#classestypespublickeymd)

##### Defined in

[lib/signature.ts:85](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L85)

___

#### fromBase58

▸ `Static` **fromBase58**(`publicKeyBase58`): [`PublicKey`](#classestypespublickeymd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKeyBase58` | `string` |

##### Returns

[`PublicKey`](#classestypespublickeymd)

##### Defined in

[lib/signature.ts:98](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L98)

___

#### fromGroup

▸ `Static` **fromGroup**(`__namedParameters`): [`PublicKey`](#classestypespublickeymd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | [`Group`](#classesgroupmd) |

##### Returns

[`PublicKey`](#classestypespublickeymd)

##### Defined in

[lib/signature.ts:76](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L76)

___

#### fromJSON

▸ `Static` **fromJSON**<`T`\>(`this`, `publicKey`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `publicKey` | `string` |

##### Returns

`InstanceType`<`T`\>

##### Overrides

[CircuitValue](#classescircuitvaluemd).[fromJSON](#fromjson)

##### Defined in

[lib/signature.ts:112](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L112)

___

#### fromObject

▸ `Static` **fromObject**<`T`\>(`this`, `value`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `NonMethods`<`InstanceType`<`T`\>\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromObject](#fromobject)

##### Defined in

[lib/circuit_value.ts:59](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L59)

___

#### fromPrivateKey

▸ `Static` **fromPrivateKey**(`__namedParameters`): [`PublicKey`](#classestypespublickeymd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | [`PrivateKey`](#classesprivatekeymd) |

##### Returns

[`PublicKey`](#classestypespublickeymd)

##### Defined in

[lib/signature.ts:81](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L81)

___

#### ofFields

▸ `Static` **ofFields**<`T`\>(`this`, `xs`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `xs` | [`Field`](#classesfieldmd)[] |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[ofFields](#offields)

##### Defined in

[lib/circuit_value.ts:134](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L134)

___

#### sizeInFields

▸ `Static` **sizeInFields**(): `number`

##### Returns

`number`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[sizeInFields](#sizeinfields)

##### Defined in

[lib/circuit_value.ts:66](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L66)

___

#### toBase58

▸ `Static` **toBase58**(`publicKey`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | [`PublicKey`](#classestypespublickeymd) |

##### Returns

`string`

##### Defined in

[lib/signature.ts:106](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L106)

___

#### toConstant

▸ `Static` **toConstant**<`T`\>(`this`, `t`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `t` | `InstanceType`<`T`\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant-1)

##### Defined in

[lib/circuit_value.ts:170](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L170)

___

#### toFields

▸ `Static` **toFields**<`T`\>(`this`, `v`): [`Field`](#classesfieldmd)[]

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields-1)

##### Defined in

[lib/circuit_value.ts:71](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L71)

___

#### toInput

▸ `Static` **toInput**<`T`\>(`this`, `v`): `HashInput`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

`HashInput`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toInput](#toinput)

##### Defined in

[lib/circuit_value.ts:88](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L88)

___

#### toJSON

▸ `Static` **toJSON**(`publicKey`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | [`PublicKey`](#classestypespublickeymd) |

##### Returns

`string`

##### Overrides

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson-1)

##### Defined in

[lib/signature.ts:109](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/signature.ts#L109)


<a name="classesuint32md"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / UInt32

## Class: UInt32

### Hierarchy

- [`CircuitValue`](#classescircuitvaluemd)

  ↳ **`UInt32`**

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [value](#value)
- [NUM\_BITS](#num_bits)

#### Accessors

- [one](#one)
- [zero](#zero)

#### Methods

- [add](#add)
- [assertEquals](#assertequals)
- [assertGt](#assertgt)
- [assertGte](#assertgte)
- [assertLt](#assertlt)
- [assertLte](#assertlte)
- [div](#div)
- [divMod](#divmod)
- [equals](#equals)
- [gt](#gt)
- [gte](#gte)
- [isConstant](#isconstant)
- [lt](#lt)
- [lte](#lte)
- [mod](#mod)
- [mul](#mul)
- [sub](#sub)
- [toConstant](#toconstant)
- [toFields](#tofields)
- [toJSON](#tojson)
- [toString](#tostring)
- [toUInt64](#touint64)
- [MAXINT](#maxint)
- [check](#check)
- [checkConstant](#checkconstant)
- [from](#from)
- [fromBigInt](#frombigint)
- [fromJSON](#fromjson)
- [fromNumber](#fromnumber)
- [fromObject](#fromobject)
- [fromString](#fromstring)
- [ofFields](#offields)
- [sizeInFields](#sizeinfields)
- [toConstant](#toconstant-1)
- [toFields](#tofields-1)
- [toInput](#toinput)
- [toJSON](#tojson-1)

### Constructors

#### constructor

• **new UInt32**(...`props`)

##### Parameters

| Name | Type |
| :------ | :------ |
| `...props` | `any`[] |

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[constructor](#constructor)

##### Defined in

[lib/circuit_value.ts:42](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L42)

### Properties

#### value

• **value**: [`Field`](#classesfieldmd)

##### Defined in

[lib/int.ts:198](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L198)

___

#### NUM\_BITS

▪ `Static` **NUM\_BITS**: `number` = `32`

##### Defined in

[lib/int.ts:199](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L199)

### Accessors

#### one

• `Static` `get` **one**(): [`UInt32`](#classesuint32md)

##### Returns

[`UInt32`](#classesuint32md)

##### Defined in

[lib/int.ts:205](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L205)

___

#### zero

• `Static` `get` **zero**(): [`UInt32`](#classesuint32md)

##### Returns

[`UInt32`](#classesuint32md)

##### Defined in

[lib/int.ts:201](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L201)

### Methods

#### add

▸ **add**(`y`): [`UInt32`](#classesuint32md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `number` \| [`UInt32`](#classesuint32md) |

##### Returns

[`UInt32`](#classesuint32md)

##### Defined in

[lib/int.ts:309](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L309)

___

#### assertEquals

▸ **assertEquals**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`UInt32`](#classesuint32md) |

##### Returns

`void`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[assertEquals](#assertequals)

##### Defined in

[lib/circuit_value.ts:126](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L126)

___

#### assertGt

▸ **assertGt**(`y`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt32`](#classesuint32md) |

##### Returns

`void`

##### Defined in

[lib/int.ts:355](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L355)

___

#### assertGte

▸ **assertGte**(`y`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt32`](#classesuint32md) |

##### Returns

`void`

##### Defined in

[lib/int.ts:363](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L363)

___

#### assertLt

▸ **assertLt**(`y`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt32`](#classesuint32md) |

##### Returns

`void`

##### Defined in

[lib/int.ts:347](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L347)

___

#### assertLte

▸ **assertLte**(`y`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt32`](#classesuint32md) |

##### Returns

`void`

##### Defined in

[lib/int.ts:338](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L338)

___

#### div

▸ **div**(`y`): [`UInt32`](#classesuint32md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `number` \| [`UInt32`](#classesuint32md) |

##### Returns

[`UInt32`](#classesuint32md)

##### Defined in

[lib/int.ts:295](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L295)

___

#### divMod

▸ **divMod**(`y`): `Object`

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| [`UInt32`](#classesuint32md) |

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `quotient` | [`UInt32`](#classesuint32md) |
| `rest` | [`UInt32`](#classesuint32md) |

##### Defined in

[lib/int.ts:259](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L259)

___

#### equals

▸ **equals**(`x`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`UInt32`](#classesuint32md) |

##### Returns

[`Bool`](#classesboolmd)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[equals](#equals)

##### Defined in

[lib/circuit_value.ts:122](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L122)

___

#### gt

▸ **gt**(`y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt32`](#classesuint32md) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[lib/int.ts:351](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L351)

___

#### gte

▸ **gte**(`y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt32`](#classesuint32md) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[lib/int.ts:359](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L359)

___

#### isConstant

▸ **isConstant**(): `boolean`

##### Returns

`boolean`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[isConstant](#isconstant)

##### Defined in

[lib/circuit_value.ts:130](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L130)

___

#### lt

▸ **lt**(`y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt32`](#classesuint32md) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[lib/int.ts:343](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L343)

___

#### lte

▸ **lte**(`y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt32`](#classesuint32md) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[lib/int.ts:321](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L321)

___

#### mod

▸ **mod**(`y`): [`UInt32`](#classesuint32md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `number` \| [`UInt32`](#classesuint32md) |

##### Returns

[`UInt32`](#classesuint32md)

##### Defined in

[lib/int.ts:299](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L299)

___

#### mul

▸ **mul**(`y`): [`UInt32`](#classesuint32md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `number` \| [`UInt32`](#classesuint32md) |

##### Returns

[`UInt32`](#classesuint32md)

##### Defined in

[lib/int.ts:303](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L303)

___

#### sub

▸ **sub**(`y`): [`UInt32`](#classesuint32md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `number` \| [`UInt32`](#classesuint32md) |

##### Returns

[`UInt32`](#classesuint32md)

##### Defined in

[lib/int.ts:315](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L315)

___

#### toConstant

▸ **toConstant**(): [`UInt32`](#classesuint32md)

##### Returns

[`UInt32`](#classesuint32md)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant)

##### Defined in

[lib/circuit_value.ts:118](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L118)

___

#### toFields

▸ **toFields**(): [`Field`](#classesfieldmd)[]

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields)

##### Defined in

[lib/circuit_value.ts:110](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L110)

___

#### toJSON

▸ **toJSON**(): `JSONValue`

##### Returns

`JSONValue`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson)

##### Defined in

[lib/circuit_value.ts:114](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L114)

___

#### toString

▸ **toString**(): `string`

##### Returns

`string`

##### Defined in

[lib/int.ts:209](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L209)

___

#### toUInt64

▸ **toUInt64**(): [`UInt64`](#classesuint64md)

##### Returns

[`UInt64`](#classesuint64md)

##### Defined in

[lib/int.ts:213](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L213)

___

#### MAXINT

▸ `Static` **MAXINT**(): [`UInt32`](#classesuint32md)

##### Returns

[`UInt32`](#classesuint32md)

##### Defined in

[lib/int.ts:255](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L255)

___

#### check

▸ `Static` **check**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`UInt32`](#classesuint32md) |

##### Returns

`void`

##### Overrides

[CircuitValue](#classescircuitvaluemd).[check](#check)

##### Defined in

[lib/int.ts:218](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L218)

___

#### checkConstant

▸ `Static` `Private` **checkConstant**(`x`): [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Field`](#classesfieldmd) |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[lib/int.ts:229](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L229)

___

#### from

▸ `Static` **from**(`x`): [`UInt32`](#classesuint32md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `string` \| `number` \| `bigint` \| [`Field`](#classesfieldmd) \| [`UInt32`](#classesuint32md) |

##### Returns

[`UInt32`](#classesuint32md)

##### Defined in

[lib/int.ts:241](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L241)

___

#### fromBigInt

▸ `Static` **fromBigInt**(`x`): [`UInt32`](#classesuint32md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `bigint` |

##### Returns

[`UInt32`](#classesuint32md)

##### Defined in

[lib/int.ts:251](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L251)

___

#### fromJSON

▸ `Static` **fromJSON**<`T`\>(`this`, `value`): ``null`` \| `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `JSONValue` |

##### Returns

``null`` \| `InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromJSON](#fromjson)

##### Defined in

[lib/circuit_value.ts:192](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L192)

___

#### fromNumber

▸ `Static` **fromNumber**(`x`): [`UInt32`](#classesuint32md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `number` |

##### Returns

[`UInt32`](#classesuint32md)

##### Defined in

[lib/int.ts:245](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L245)

___

#### fromObject

▸ `Static` **fromObject**<`T`\>(`this`, `value`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `NonMethods`<`InstanceType`<`T`\>\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromObject](#fromobject)

##### Defined in

[lib/circuit_value.ts:59](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L59)

___

#### fromString

▸ `Static` **fromString**(`x`): [`UInt32`](#classesuint32md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `string` |

##### Returns

[`UInt32`](#classesuint32md)

##### Defined in

[lib/int.ts:248](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L248)

___

#### ofFields

▸ `Static` **ofFields**<`T`\>(`this`, `xs`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `xs` | [`Field`](#classesfieldmd)[] |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[ofFields](#offields)

##### Defined in

[lib/circuit_value.ts:134](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L134)

___

#### sizeInFields

▸ `Static` **sizeInFields**(): `number`

##### Returns

`number`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[sizeInFields](#sizeinfields)

##### Defined in

[lib/circuit_value.ts:66](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L66)

___

#### toConstant

▸ `Static` **toConstant**<`T`\>(`this`, `t`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `t` | `InstanceType`<`T`\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant-1)

##### Defined in

[lib/circuit_value.ts:170](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L170)

___

#### toFields

▸ `Static` **toFields**<`T`\>(`this`, `v`): [`Field`](#classesfieldmd)[]

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields-1)

##### Defined in

[lib/circuit_value.ts:71](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L71)

___

#### toInput

▸ `Static` **toInput**(`x`): `HashInput`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`UInt32`](#classesuint32md) |

##### Returns

`HashInput`

##### Overrides

[CircuitValue](#classescircuitvaluemd).[toInput](#toinput)

##### Defined in

[lib/int.ts:222](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L222)

___

#### toJSON

▸ `Static` **toJSON**(`x`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`UInt32`](#classesuint32md) |

##### Returns

`string`

##### Overrides

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson-1)

##### Defined in

[lib/int.ts:225](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L225)


<a name="classesuint64md"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / UInt64

## Class: UInt64

### Hierarchy

- [`CircuitValue`](#classescircuitvaluemd)

  ↳ **`UInt64`**

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Properties

- [value](#value)
- [NUM\_BITS](#num_bits)

#### Accessors

- [one](#one)
- [zero](#zero)

#### Methods

- [add](#add)
- [assertEquals](#assertequals)
- [assertGt](#assertgt)
- [assertGte](#assertgte)
- [assertLt](#assertlt)
- [assertLte](#assertlte)
- [div](#div)
- [divMod](#divmod)
- [equals](#equals)
- [gt](#gt)
- [gte](#gte)
- [isConstant](#isconstant)
- [lt](#lt)
- [lte](#lte)
- [mod](#mod)
- [mul](#mul)
- [sub](#sub)
- [toConstant](#toconstant)
- [toFields](#tofields)
- [toJSON](#tojson)
- [toString](#tostring)
- [MAXINT](#maxint)
- [check](#check)
- [checkConstant](#checkconstant)
- [from](#from)
- [fromBigInt](#frombigint)
- [fromJSON](#fromjson)
- [fromNumber](#fromnumber)
- [fromObject](#fromobject)
- [fromString](#fromstring)
- [ofFields](#offields)
- [sizeInFields](#sizeinfields)
- [toConstant](#toconstant-1)
- [toFields](#tofields-1)
- [toInput](#toinput)
- [toJSON](#tojson-1)

### Constructors

#### constructor

• **new UInt64**(...`props`)

##### Parameters

| Name | Type |
| :------ | :------ |
| `...props` | `any`[] |

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[constructor](#constructor)

##### Defined in

[lib/circuit_value.ts:42](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L42)

### Properties

#### value

• **value**: [`Field`](#classesfieldmd)

##### Defined in

[lib/int.ts:10](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L10)

___

#### NUM\_BITS

▪ `Static` **NUM\_BITS**: `number` = `64`

##### Defined in

[lib/int.ts:11](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L11)

### Accessors

#### one

• `Static` `get` **one**(): [`UInt64`](#classesuint64md)

##### Returns

[`UInt64`](#classesuint64md)

##### Defined in

[lib/int.ts:17](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L17)

___

#### zero

• `Static` `get` **zero**(): [`UInt64`](#classesuint64md)

##### Returns

[`UInt64`](#classesuint64md)

##### Defined in

[lib/int.ts:13](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L13)

### Methods

#### add

▸ **add**(`y`): [`UInt64`](#classesuint64md)

Addition with overflow checking.

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `number` \| [`UInt64`](#classesuint64md) |

##### Returns

[`UInt64`](#classesuint64md)

##### Defined in

[lib/int.ts:135](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L135)

___

#### assertEquals

▸ **assertEquals**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`UInt64`](#classesuint64md) |

##### Returns

`void`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[assertEquals](#assertequals)

##### Defined in

[lib/circuit_value.ts:126](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L126)

___

#### assertGt

▸ **assertGt**(`y`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt64`](#classesuint64md) |

##### Returns

`void`

##### Defined in

[lib/int.ts:184](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L184)

___

#### assertGte

▸ **assertGte**(`y`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt64`](#classesuint64md) |

##### Returns

`void`

##### Defined in

[lib/int.ts:192](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L192)

___

#### assertLt

▸ **assertLt**(`y`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt64`](#classesuint64md) |

##### Returns

`void`

##### Defined in

[lib/int.ts:176](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L176)

___

#### assertLte

▸ **assertLte**(`y`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt64`](#classesuint64md) |

##### Returns

`void`

##### Defined in

[lib/int.ts:167](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L167)

___

#### div

▸ **div**(`y`): [`UInt64`](#classesuint64md)

Integer division.

`x.div(y)` returns the floor of `x / y`, that is, the greatest
`z` such that `x * y <= x`.

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `number` \| [`UInt64`](#classesuint64md) |

##### Returns

[`UInt64`](#classesuint64md)

##### Defined in

[lib/int.ts:109](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L109)

___

#### divMod

▸ **divMod**(`y`): `Object`

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `string` \| `number` \| [`UInt64`](#classesuint64md) |

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `quotient` | [`UInt64`](#classesuint64md) |
| `rest` | [`UInt64`](#classesuint64md) |

##### Defined in

[lib/int.ts:66](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L66)

___

#### equals

▸ **equals**(`x`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`UInt64`](#classesuint64md) |

##### Returns

[`Bool`](#classesboolmd)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[equals](#equals)

##### Defined in

[lib/circuit_value.ts:122](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L122)

___

#### gt

▸ **gt**(`y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt64`](#classesuint64md) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[lib/int.ts:180](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L180)

___

#### gte

▸ **gte**(`y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt64`](#classesuint64md) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[lib/int.ts:188](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L188)

___

#### isConstant

▸ **isConstant**(): `boolean`

##### Returns

`boolean`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[isConstant](#isconstant)

##### Defined in

[lib/circuit_value.ts:130](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L130)

___

#### lt

▸ **lt**(`y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt64`](#classesuint64md) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[lib/int.ts:172](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L172)

___

#### lte

▸ **lte**(`y`): [`Bool`](#classesboolmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | [`UInt64`](#classesuint64md) |

##### Returns

[`Bool`](#classesboolmd)

##### Defined in

[lib/int.ts:150](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L150)

___

#### mod

▸ **mod**(`y`): [`UInt64`](#classesuint64md)

Integer remainder.

`x.mod(y)` returns the value `z` such that `0 <= z < y` and
`x - z` is divisble by `y`.

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `number` \| [`UInt64`](#classesuint64md) |

##### Returns

[`UInt64`](#classesuint64md)

##### Defined in

[lib/int.ts:119](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L119)

___

#### mul

▸ **mul**(`y`): [`UInt64`](#classesuint64md)

Multiplication with overflow checking.

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `number` \| [`UInt64`](#classesuint64md) |

##### Returns

[`UInt64`](#classesuint64md)

##### Defined in

[lib/int.ts:126](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L126)

___

#### sub

▸ **sub**(`y`): [`UInt64`](#classesuint64md)

Subtraction with underflow checking.

##### Parameters

| Name | Type |
| :------ | :------ |
| `y` | `number` \| [`UInt64`](#classesuint64md) |

##### Returns

[`UInt64`](#classesuint64md)

##### Defined in

[lib/int.ts:144](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L144)

___

#### toConstant

▸ **toConstant**(): [`UInt64`](#classesuint64md)

##### Returns

[`UInt64`](#classesuint64md)

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant)

##### Defined in

[lib/circuit_value.ts:118](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L118)

___

#### toFields

▸ **toFields**(): [`Field`](#classesfieldmd)[]

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields)

##### Defined in

[lib/circuit_value.ts:110](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L110)

___

#### toJSON

▸ **toJSON**(): `JSONValue`

##### Returns

`JSONValue`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson)

##### Defined in

[lib/circuit_value.ts:114](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L114)

___

#### toString

▸ **toString**(): `string`

##### Returns

`string`

##### Defined in

[lib/int.ts:21](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L21)

___

#### MAXINT

▸ `Static` **MAXINT**(): [`UInt64`](#classesuint64md)

##### Returns

[`UInt64`](#classesuint64md)

##### Defined in

[lib/int.ts:62](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L62)

___

#### check

▸ `Static` **check**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`UInt64`](#classesuint64md) |

##### Returns

`void`

##### Overrides

[CircuitValue](#classescircuitvaluemd).[check](#check)

##### Defined in

[lib/int.ts:25](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L25)

___

#### checkConstant

▸ `Static` `Private` **checkConstant**(`x`): [`Field`](#classesfieldmd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Field`](#classesfieldmd) |

##### Returns

[`Field`](#classesfieldmd)

##### Defined in

[lib/int.ts:36](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L36)

___

#### from

▸ `Static` **from**(`x`): [`UInt64`](#classesuint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `string` \| `number` \| `bigint` \| [`Field`](#classesfieldmd) \| [`UInt32`](#classesuint32md) \| [`UInt64`](#classesuint64md) |

##### Returns

[`UInt64`](#classesuint64md)

##### Defined in

[lib/int.ts:48](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L48)

___

#### fromBigInt

▸ `Static` **fromBigInt**(`x`): [`UInt64`](#classesuint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `bigint` |

##### Returns

[`UInt64`](#classesuint64md)

##### Defined in

[lib/int.ts:58](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L58)

___

#### fromJSON

▸ `Static` **fromJSON**<`T`\>(`this`, `value`): ``null`` \| `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `JSONValue` |

##### Returns

``null`` \| `InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromJSON](#fromjson)

##### Defined in

[lib/circuit_value.ts:192](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L192)

___

#### fromNumber

▸ `Static` **fromNumber**(`x`): [`UInt64`](#classesuint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `number` |

##### Returns

[`UInt64`](#classesuint64md)

##### Defined in

[lib/int.ts:52](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L52)

___

#### fromObject

▸ `Static` **fromObject**<`T`\>(`this`, `value`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `value` | `NonMethods`<`InstanceType`<`T`\>\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[fromObject](#fromobject)

##### Defined in

[lib/circuit_value.ts:59](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L59)

___

#### fromString

▸ `Static` **fromString**(`x`): [`UInt64`](#classesuint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `string` |

##### Returns

[`UInt64`](#classesuint64md)

##### Defined in

[lib/int.ts:55](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L55)

___

#### ofFields

▸ `Static` **ofFields**<`T`\>(`this`, `xs`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `xs` | [`Field`](#classesfieldmd)[] |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[ofFields](#offields)

##### Defined in

[lib/circuit_value.ts:134](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L134)

___

#### sizeInFields

▸ `Static` **sizeInFields**(): `number`

##### Returns

`number`

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[sizeInFields](#sizeinfields)

##### Defined in

[lib/circuit_value.ts:66](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L66)

___

#### toConstant

▸ `Static` **toConstant**<`T`\>(`this`, `t`): `InstanceType`<`T`\>

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `t` | `InstanceType`<`T`\> |

##### Returns

`InstanceType`<`T`\>

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toConstant](#toconstant-1)

##### Defined in

[lib/circuit_value.ts:170](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L170)

___

#### toFields

▸ `Static` **toFields**<`T`\>(`this`, `v`): [`Field`](#classesfieldmd)[]

##### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `AnyConstructor` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `T` |
| `v` | `InstanceType`<`T`\> |

##### Returns

[`Field`](#classesfieldmd)[]

##### Inherited from

[CircuitValue](#classescircuitvaluemd).[toFields](#tofields-1)

##### Defined in

[lib/circuit_value.ts:71](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L71)

___

#### toInput

▸ `Static` **toInput**(`x`): `HashInput`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`UInt64`](#classesuint64md) |

##### Returns

`HashInput`

##### Overrides

[CircuitValue](#classescircuitvaluemd).[toInput](#toinput)

##### Defined in

[lib/int.ts:29](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L29)

___

#### toJSON

▸ `Static` **toJSON**(`x`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`UInt64`](#classesuint64md) |

##### Returns

`string`

##### Overrides

[CircuitValue](#classescircuitvaluemd).[toJSON](#tojson-1)

##### Defined in

[lib/int.ts:32](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/int.ts#L32)


<a name="classesverificationkeymd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / VerificationKey

## Class: VerificationKey

Part of the circuit [[ Keypair ]]. A verification key can be used to verify a [[ Proof ]] when you provide the correct public input.

### Table of contents

#### Constructors

- [constructor](#constructor)

#### Methods

- [verify](#verify)

### Constructors

#### constructor

• **new VerificationKey**()

### Methods

#### verify

▸ **verify**(`publicInput`, `proof`): `boolean`

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicInput` | `any`[] |
| `proof` | `Proof` |

##### Returns

`boolean`

##### Defined in

[snarky.d.ts:702](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L702)

# Interfaces


<a name="interfacesasfieldelementsmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / AsFieldElements

## Interface: AsFieldElements<T\>

### Type parameters

| Name |
| :------ |
| `T` |

### Table of contents

#### Methods

- [check](#check)
- [ofFields](#offields)
- [sizeInFields](#sizeinfields)
- [toFields](#tofields)

### Methods

#### check

▸ **check**(`x`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `T` |

##### Returns

`void`

##### Defined in

[snarky.d.ts:479](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L479)

___

#### ofFields

▸ **ofFields**(`x`): `T`

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | [`Field`](#classesfieldmd)[] |

##### Returns

`T`

##### Defined in

[snarky.d.ts:477](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L477)

___

#### sizeInFields

▸ **sizeInFields**(): `number`

##### Returns

`number`

##### Defined in

[snarky.d.ts:478](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L478)

___

#### toFields

▸ **toFields**(`x`): [`Field`](#classesfieldmd)[]

##### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `T` |

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[snarky.d.ts:476](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L476)


<a name="interfacespermissionsmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Permissions

## Interface: Permissions

Permissions specify how specific aspects of the zkapp account are allowed to
be modified. All fields are denominated by a [[ Permission ]].

### Hierarchy

- `Permissions_`

  ↳ **`Permissions`**

### Table of contents

#### Properties

- [editSequenceState](#editsequencestate)
- [editState](#editstate)
- [incrementNonce](#incrementnonce)
- [receive](#receive)
- [send](#send)
- [setDelegate](#setdelegate)
- [setPermissions](#setpermissions)
- [setTokenSymbol](#settokensymbol)
- [setVerificationKey](#setverificationkey)
- [setVotingFor](#setvotingfor)
- [setZkappUri](#setzkappuri)

### Properties

#### editSequenceState

• **editSequenceState**: [`AuthRequired`](#authrequired-1)

The [[ Permission ]] corresponding to the ability to change the sequence state
associated with the account.

TODO: Define sequence state here as well.

##### Overrides

Permissions\_.editSequenceState

##### Defined in

[lib/party.ts:200](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L200)

___

#### editState

• **editState**: [`AuthRequired`](#authrequired-1)

The [[ Permission ]] corresponding to the 8 state fields associated with an
account.

##### Overrides

Permissions\_.editState

##### Defined in

[lib/party.ts:153](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L153)

___

#### incrementNonce

• **incrementNonce**: [`AuthRequired`](#authrequired-1)

##### Overrides

Permissions\_.incrementNonce

##### Defined in

[lib/party.ts:209](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L209)

___

#### receive

• **receive**: [`AuthRequired`](#authrequired-1)

The [[ Permission ]] corresponding to the ability to receive transactions to this
account.

##### Overrides

Permissions\_.receive

##### Defined in

[lib/party.ts:165](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L165)

___

#### send

• **send**: [`AuthRequired`](#authrequired-1)

The [[ Permission ]] corresponding to the ability to send transactions from this
account.

##### Overrides

Permissions\_.send

##### Defined in

[lib/party.ts:159](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L159)

___

#### setDelegate

• **setDelegate**: [`AuthRequired`](#authrequired-1)

The [[ Permission ]] corresponding to the ability to set the delegate field of
the account.

##### Overrides

Permissions\_.setDelegate

##### Defined in

[lib/party.ts:171](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L171)

___

#### setPermissions

• **setPermissions**: [`AuthRequired`](#authrequired-1)

The [[ Permission ]] corresponding to the ability to set the permissions field of
the account.

##### Overrides

Permissions\_.setPermissions

##### Defined in

[lib/party.ts:177](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L177)

___

#### setTokenSymbol

• **setTokenSymbol**: [`AuthRequired`](#authrequired-1)

The [[ Permission ]] corresponding to the ability to set the token symbol for
this account.

##### Overrides

Permissions\_.setTokenSymbol

##### Defined in

[lib/party.ts:206](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L206)

___

#### setVerificationKey

• **setVerificationKey**: [`AuthRequired`](#authrequired-1)

The [[ Permission ]] corresponding to the ability to set the verification key
associated with the circuit tied to this account. Effectively
"upgradability" of the smart contract.

##### Overrides

Permissions\_.setVerificationKey

##### Defined in

[lib/party.ts:184](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L184)

___

#### setVotingFor

• **setVotingFor**: [`AuthRequired`](#authrequired-1)

##### Overrides

Permissions\_.setVotingFor

##### Defined in

[lib/party.ts:210](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L210)

___

#### setZkappUri

• **setZkappUri**: [`AuthRequired`](#authrequired-1)

The [[ Permission ]] corresponding to the ability to set the zkapp uri typically
pointing to the source code of the smart contract. Usually this should be
changed whenever the [[ Permissions.setVerificationKey ]] is changed.
Effectively "upgradability" of the smart contract.

##### Overrides

Permissions\_.setZkappUri

##### Defined in

[lib/party.ts:192](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L192)

## References

### PublicKey

Re-exports [PublicKey](#classestypespublickeymd)

## Type Aliases

### DeployArgs

Ƭ **DeployArgs**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `verificationKey?` | { `data`: `string` ; `hash`: `string` \| [`Field`](#classesfieldmd)  } |
| `verificationKey.data` | `string` |
| `verificationKey.hash` | `string` \| [`Field`](#classesfieldmd) |
| `zkappKey?` | [`PrivateKey`](#classesprivatekeymd) |

#### Defined in

[lib/zkapp.ts:840](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L840)

___

### State

Ƭ **State**<`A`\>: `Object`

Gettable and settable state that can be checked for equality.

#### Type parameters

| Name |
| :------ |
| `A` |

#### Type declaration

| Name | Type |
| :------ | :------ |
| `assertEquals` | (`a`: `A`) => `void` |
| `assertNothing` | () => `void` |
| `fetch` | () => `Promise`<`undefined` \| `A`\> |
| `get` | () => `A` |
| `set` | (`a`: `A`) => `void` |

#### Defined in

[lib/state.ts:23](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/state.ts#L23)

___

### ZkappPublicInput

Ƭ **ZkappPublicInput**: `Object`

The public input for zkApps consists of certain hashes of the proving Party (and its child parties) which is constructed during method execution.

For SmartContract proving, a method is run twice: First outside the proof, to obtain the public input, and once in the prover,
which takes the public input as input. The current transaction is hashed again inside the prover, which asserts that the result equals the input public input,
as part of the snark circuit. The block producer will also hash the transaction they receive and pass it as a public input to the verifier.
Thus, the transaction is fully constrained by the proof - the proof couldn't be used to attest to a different transaction.

#### Type declaration

| Name | Type |
| :------ | :------ |
| `calls` | [`Field`](#classesfieldmd) |
| `party` | [`Field`](#classesfieldmd) |

#### Defined in

[lib/party.ts:1165](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L1165)

## Variables

### Permissions

• **Permissions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `default` | () => [`Permissions`](#permissions) |
| `impossible` | () => [`AuthRequired`](#authrequired-1) |
| `initial` | () => [`Permissions`](#permissions) |
| `none` | () => [`AuthRequired`](#authrequired-1) |
| `proof` | () => [`AuthRequired`](#authrequired-1) |
| `proofOrSignature` | () => [`AuthRequired`](#authrequired-1) |
| `signature` | () => [`AuthRequired`](#authrequired-1) |

#### Defined in

[lib/party.ts:212](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L212)

___

### Poseidon

• `Const` **Poseidon**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `Sponge` | typeof `Sponge` |
| ``get` **initialState**(): [[`Field`](#classesfieldmd), [`Field`](#classesfieldmd), [`Field`](#classesfieldmd)]` | {} |
| `hash` | (`input`: [`Field`](#classesfieldmd)[]) => [`Field`](#classesfieldmd) |
| `update` | (`state`: [[`Field`](#classesfieldmd), [`Field`](#classesfieldmd), [`Field`](#classesfieldmd)], `input`: [`Field`](#classesfieldmd)[]) => [[`Field`](#classesfieldmd), [`Field`](#classesfieldmd), [`Field`](#classesfieldmd)] |

#### Defined in

[lib/hash.ts:37](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/hash.ts#L37)

___

### ZkappPublicInput

• **ZkappPublicInput**: `AsFieldsExtended`<[`ZkappPublicInput`](#zkapppublicinput-1)\>

#### Defined in

[lib/party.ts:1166](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L1166)

___

### isReady

• **isReady**: `Promise`<`undefined`\>

A Promise that resolves when SnarkyJS is ready to be used

#### Defined in

[snarky.d.ts:834](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L834)

## Functions

### State

▸ **State**<`A`\>(): [`State`](#state)<`A`\>

#### Type parameters

| Name |
| :------ |
| `A` |

#### Returns

[`State`](#state)<`A`\>

#### Defined in

[lib/state.ts:30](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/state.ts#L30)

___

### ZkProgram

▸ **ZkProgram**<`PublicInputType`, `Types`\>(`__namedParameters`): { `name`: `string` ; `publicInputType`: `PublicInputType` ; `compile`: () => `Promise`<{ `verificationKey`: `string`  }\> ; `digest`: () => `string` ; `verify`: (`proof`: [`Proof`](#classesproofmd)<`InferInstance`<`PublicInputType`\>\>) => `Promise`<`boolean`\>  } & { [I in keyof Types]: Prover<InferInstance<PublicInputType\>, Types[I]\> }

#### Type parameters

| Name | Type |
| :------ | :------ |
| `PublicInputType` | extends [`AsFieldElements`](#interfacesasfieldelementsmd)<`any`, `PublicInputType`\> |
| `Types` | extends `Object` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | `Object` |
| `__namedParameters.methods` | { [I in string \| number \| symbol]: Method<InferInstance<PublicInputType\>, Types[I]\> } |
| `__namedParameters.publicInput` | `PublicInputType` |

#### Returns

{ `name`: `string` ; `publicInputType`: `PublicInputType` ; `compile`: () => `Promise`<{ `verificationKey`: `string`  }\> ; `digest`: () => `string` ; `verify`: (`proof`: [`Proof`](#classesproofmd)<`InferInstance`<`PublicInputType`\>\>) => `Promise`<`boolean`\>  } & { [I in keyof Types]: Prover<InferInstance<PublicInputType\>, Types[I]\> }

#### Defined in

[lib/proof_system.ts:144](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L144)

___

### addCachedAccount

▸ **addCachedAccount**(`account`, `graphqlEndpoint?`): `void`

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `account` | `Object` | `undefined` |
| `account.balance?` | `string` \| `number` \| [`UInt64`](#classesuint64md) | `undefined` |
| `account.nonce` | `string` \| `number` \| [`UInt32`](#classesuint32md) | `undefined` |
| `account.publicKey` | `string` \| [`PublicKey`](#classestypespublickeymd) | `undefined` |
| `account.tokenId` | `string` | `undefined` |
| `account.zkapp?` | `Object` | `undefined` |
| `account.zkapp.appState` | (`string` \| `number` \| [`Field`](#classesfieldmd))[] | `undefined` |
| `graphqlEndpoint` | `string` | `defaultGraphqlEndpoint` |

#### Returns

`void`

#### Defined in

[lib/fetch.ts:357](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/fetch.ts#L357)

___

### arrayProp

▸ **arrayProp**<`T`\>(`elementType`, `length`): (`target`: `any`, `key`: `string`) => `void`

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `elementType` | [`AsFieldElements`](#interfacesasfieldelementsmd)<`T`\> |
| `length` | `number` |

#### Returns

`fn`

▸ (`target`, `key`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `target` | `any` |
| `key` | `string` |

##### Returns

`void`

#### Defined in

[lib/circuit_value.ts:283](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L283)

___

### circuitMain

▸ **circuitMain**(`target`, `propertyName`, `_descriptor?`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | `any` |
| `propertyName` | `string` |
| `_descriptor?` | `PropertyDescriptor` |

#### Returns

`any`

#### Defined in

[lib/circuit_value.ts:352](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L352)

___

### circuitValue

▸ **circuitValue**<`T`\>(`typeObj`, `options?`): `AsFieldsExtended`<`T`\>

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `typeObj` | `any` |
| `options?` | `Object` |
| `options.customObjectKeys` | `string`[] |

#### Returns

`AsFieldsExtended`<`T`\>

#### Defined in

[lib/circuit_value.ts:406](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L406)

___

### declareMethods

▸ **declareMethods**<`T`\>(`SmartContract`, `methodArguments`): `void`

`declareMethods` can be used in place of the `@method` decorator
to declare SmartContract methods along with their list of arguments.
It should be placed _after_ the class declaration.
Here is an example of declaring a method `update`, which takes a single argument of type `Field`:
```ts
class MyContract extends SmartContract {
  // ...
  update(x: Field) {
    // ...
  }
}
declareMethods(MyContract, { update: [Field] }); // `[Field]` is the list of arguments!
```
Note that a method of the same name must still be defined on the class, just without the decorator.

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends typeof [`SmartContract`](#classessmartcontractmd) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `SmartContract` | `T` |
| `methodArguments` | `Record`<`string`, [`AsFieldElements`](#interfacesasfieldelementsmd)<`unknown`\>[]\> |

#### Returns

`void`

#### Defined in

[lib/zkapp.ts:961](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L961)

___

### declareState

▸ **declareState**<`T`\>(`SmartContract`, `states`): `void`

`declareState` can be used in place of the `@state` decorator to declare on-chain state on a SmartContract.
It should be placed _after_ the class declaration.
Here is an example of declaring a state property `x` of type `Field`.
```ts
class MyContract extends SmartContract {
  x = State<Field>();
  // ...
}
declareState(MyContract, { x: Field });
```

If you're using pure JS, it's _not_ possible to use the built-in class field syntax,
i.e. the following will _not_ work:

```js
// THIS IS WRONG IN JS!
class MyContract extends SmartContract {
  x = State();
}
declareState(MyContract, { x: Field });
```

Instead, add a constructor where you assign the property:
```js
class MyContract extends SmartContract {
  constructor(x) {
    super();
    this.x = State();
  }
}
declareState(MyContract, { x: Field });
```

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends typeof [`SmartContract`](#classessmartcontractmd) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `SmartContract` | `T` |
| `states` | `Record`<`string`, [`AsFieldElements`](#interfacesasfieldelementsmd)<`unknown`\>\> |

#### Returns

`void`

#### Defined in

[lib/state.ts:120](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/state.ts#L120)

___

### deploy

▸ **deploy**<`S`\>(`SmartContract`, `__namedParameters`): `Promise`<`string`\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `S` | extends typeof [`SmartContract`](#classessmartcontractmd) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `SmartContract` | `S` |
| `__namedParameters` | `Object` |
| `__namedParameters.feePayer?` | [`FeePayerSpec`](#feepayerspec) |
| `__namedParameters.initialBalance?` | `string` \| `number` |
| `__namedParameters.verificationKey` | `Object` |
| `__namedParameters.verificationKey.data` | `string` |
| `__namedParameters.verificationKey.hash` | `string` \| [`Field`](#classesfieldmd) |
| `__namedParameters.zkappKey` | [`PrivateKey`](#classesprivatekeymd) |

#### Returns

`Promise`<`string`\>

#### Defined in

[lib/zkapp.ts:847](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L847)

___

### fetchAccount

▸ **fetchAccount**(`accountInfo`, `graphqlEndpoint?`, `config?`): `Promise`<{ `account`: `Account` ; `error`: `undefined`  } \| { `account`: `undefined` ; `error`: `FetchError`  }\>

Gets account information on the specified publicKey by performing a GraphQL query
to the specified endpoint. This will call the 'GetAccountInfo' query which fetches
zkapp related account information.

If an error is returned by the specified endpoint, an error is thrown. Otherwise,
the data is returned.

#### Parameters

| Name | Type | Default value | Description |
| :------ | :------ | :------ | :------ |
| `accountInfo` | `Object` | `undefined` | - |
| `accountInfo.publicKey` | `string` \| [`PublicKey`](#classestypespublickeymd) | `undefined` | - |
| `accountInfo.tokenId?` | `string` | `undefined` | - |
| `graphqlEndpoint` | `string` | `defaultGraphqlEndpoint` | The graphql endpoint to fetch from |
| `config` | `Object` | `{}` | An object that exposes an additional timeout option |
| `config.timeout` | `undefined` \| `number` | `undefined` | - |

#### Returns

`Promise`<{ `account`: `Account` ; `error`: `undefined`  } \| { `account`: `undefined` ; `error`: `FetchError`  }\>

zkapp information on the specified account or an error is thrown

#### Defined in

[lib/fetch.ts:45](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/fetch.ts#L45)

___

### fetchLastBlock

▸ **fetchLastBlock**(`graphqlEndpoint?`): `Promise`<`PreconditionBaseTypes`<{ `blockchainLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceGenesis`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceHardFork`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `minWindowDensity`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `nextEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `snarkedLedgerHash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `stakingEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `timestamp`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  }\>\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `graphqlEndpoint` | `string` | `defaultGraphqlEndpoint` |

#### Returns

`Promise`<`PreconditionBaseTypes`<{ `blockchainLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceGenesis`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceHardFork`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `minWindowDensity`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `nextEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `snarkedLedgerHash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `stakingEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `timestamp`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  }\>\>

#### Defined in

[lib/fetch.ts:383](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/fetch.ts#L383)

___

### getSrs

▸ **getSrs**(`keypair`): typeof `WasmFpSrs`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `keypair` | [`Keypair`](#classeskeypairmd) | SNARK keypair, as returned by Circuit.generateKeypair |

#### Returns

typeof `WasmFpSrs`

The SRS (structured reference string), needed to reconstruct the keypair later

#### Defined in

[snarky/addons.js:18](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/addons.js#L18)

___

### matrixProp

▸ **matrixProp**<`T`\>(`elementType`, `nRows`, `nColumns`): (`target`: `any`, `key`: `string`) => `void`

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `elementType` | [`AsFieldElements`](#interfacesasfieldelementsmd)<`T`\> |
| `nRows` | `number` |
| `nColumns` | `number` |

#### Returns

`fn`

▸ (`target`, `key`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `target` | `any` |
| `key` | `string` |

##### Returns

`void`

#### Defined in

[lib/circuit_value.ts:292](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L292)

___

### method

▸ **method**<`T`\>(`target`, `methodName`, `descriptor`): `void`

A decorator to use in a zkapp to mark a method as callable by anyone.
You can use inside your zkapp class as:

```
@method myMethod(someArg: Field) {
 // your code here
}
```

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`SmartContract`](#classessmartcontractmd)<`T`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | `T` & { `constructor`: `any`  } |
| `methodName` | keyof `T` & `string` |
| `descriptor` | `PropertyDescriptor` |

#### Returns

`void`

#### Defined in

[lib/zkapp.ts:88](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L88)

___

### partiesToJson

▸ **partiesToJson**(`__namedParameters`): [`Parties`](#parties)

#### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | `Parties` |

#### Returns

[`Parties`](#parties)

#### Defined in

[lib/party.ts:1066](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/party.ts#L1066)

___

### prop

▸ **prop**(`this`, `target`, `key`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `this` | `any` |
| `target` | `any` |
| `key` | `string` |

#### Returns

`void`

#### Defined in

[lib/circuit_value.ts:224](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L224)

___

### public\_

▸ **public_**(`target`, `_key`, `index`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | `any` |
| `_key` | `string` \| `symbol` |
| `index` | `number` |

#### Returns

`void`

#### Defined in

[lib/circuit_value.ts:308](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/circuit_value.ts#L308)

___

### recoverVerificationKey

▸ **recoverVerificationKey**(`srs`, `serializedVk`): [`VerificationKey`](#classesverificationkeymd)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `srs` | typeof `WasmFpSrs` | the "structured reference string", a set of precomputed values needed for verifying proofs |
| `serializedVk` | `string` | string representation of a Circuit verification key |

#### Returns

[`VerificationKey`](#classesverificationkeymd)

the recovered verification key

#### Defined in

[snarky/addons.js:49](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/addons.js#L49)

___

### sendZkapp

▸ **sendZkapp**(`json`, `graphqlEndpoint?`, `__namedParameters?`): `Promise`<[`FetchResponse`, `undefined`] \| [`undefined`, `FetchError`]\>

#### Parameters

| Name | Type | Default value |
| :------ | :------ | :------ |
| `json` | `string` | `undefined` |
| `graphqlEndpoint` | `string` | `defaultGraphqlEndpoint` |
| `__namedParameters` | `Object` | `{}` |
| `__namedParameters.timeout` | `undefined` \| `number` | `undefined` |

#### Returns

`Promise`<[`FetchResponse`, `undefined`] \| [`undefined`, `FetchError`]\>

#### Defined in

[lib/fetch.ts:527](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/fetch.ts#L527)

___

### serializeVerificationKey

▸ **serializeVerificationKey**(`verificationKey`): `string`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `verificationKey` | [`VerificationKey`](#classesverificationkeymd) | the verification key of a Circuit |

#### Returns

`string`

string representation of the verification key

#### Defined in

[snarky/addons.js:27](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/addons.js#L27)

___

### setGraphqlEndpoint

▸ **setGraphqlEndpoint**(`graphqlEndpoint`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `graphqlEndpoint` | `string` |

#### Returns

`void`

#### Defined in

[lib/fetch.ts:28](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/fetch.ts#L28)

___

### shutdown

▸ **shutdown**(): `Promise`<`undefined`\>

This function *must* be called at the end of a nodejs program, otherwise the
worker threads will continue running and the program will never terminate.
From web applications, this function is a no-op.

#### Returns

`Promise`<`undefined`\>

#### Defined in

[snarky.d.ts:829](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky.d.ts#L829)

___

### signFeePayer

▸ **signFeePayer**(`transactionJson`, `feePayerKey`, `__namedParameters`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `transactionJson` | `string` |
| `feePayerKey` | `string` \| [`PrivateKey`](#classesprivatekeymd) |
| `__namedParameters` | `Object` |

#### Returns

`string`

#### Defined in

[lib/zkapp.ts:919](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/zkapp.ts#L919)

___

### state

▸ **state**<`A`\>(`stateType`): (`target`: [`SmartContract`](#classessmartcontractmd) & { `constructor`: `any`  }, `key`: `string`, `_descriptor?`: `PropertyDescriptor`) => `void`

A decorator to use within a zkapp to indicate what will be stored on-chain.
For example, if you want to store a field element `some_state` in a zkapp,
you can use the following in the declaration of your zkapp:

```
@state(Field) some_state = State<Field>();
```

#### Type parameters

| Name |
| :------ |
| `A` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `stateType` | [`AsFieldElements`](#interfacesasfieldelementsmd)<`A`\> |

#### Returns

`fn`

▸ (`target`, `key`, `_descriptor?`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `target` | [`SmartContract`](#classessmartcontractmd) & { `constructor`: `any`  } |
| `key` | `string` |
| `_descriptor?` | `PropertyDescriptor` |

##### Returns

`void`

#### Defined in

[lib/state.ts:44](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/state.ts#L44)

___

### verify

▸ **verify**(`proof`, `verificationKey`): `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `proof` | `JsonProof` \| [`Proof`](#classesproofmd)<`any`\> |
| `verificationKey` | `string` |

#### Returns

`Promise`<`boolean`\>

#### Defined in

[lib/proof_system.ts:106](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L106)

# Modules


<a name="modulesencodingmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Encoding

## Namespace: Encoding

### Table of contents

#### Variables

- [Bijective](#bijective)
- [EpochSeed](#epochseed)
- [LedgerHash](#ledgerhash)
- [ReceiptChainHash](#receiptchainhash)
- [StateHash](#statehash)
- [TokenId](#tokenid)

#### Functions

- [bytesFromFields](#bytesfromfields)
- [bytesToFields](#bytestofields)
- [stringFromFields](#stringfromfields)
- [stringToFields](#stringtofields)

### Variables

#### Bijective

• `Const` **Bijective**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `Fp` | { `fromBytes`: (`bytes`: `Uint8Array`) => [`Field`](#classesfieldmd)[] ; `toBytes`: (`fields`: [`Field`](#classesfieldmd)[]) => `Uint8Array` ; `fromString`: (`message`: `string`) => [`Field`](#classesfieldmd)[] ; `toString`: (`fields`: [`Field`](#classesfieldmd)[]) => `string`  } |
| `Fp.fromBytes` | (`bytes`: `Uint8Array`) => [`Field`](#classesfieldmd)[] |
| `Fp.toBytes` | (`fields`: [`Field`](#classesfieldmd)[]) => `Uint8Array` |
| `Fp.fromString` | [object Object] |
| `Fp.toString` | [object Object] |
| `Fq` | { `fromBytes`: (`bytes`: `Uint8Array`) => [`Field`](#classesfieldmd)[] ; `toBytes`: (`fields`: [`Field`](#classesfieldmd)[]) => `Uint8Array` ; `fromString`: (`message`: `string`) => [`Field`](#classesfieldmd)[] ; `toString`: (`fields`: [`Field`](#classesfieldmd)[]) => `string`  } |
| `Fq.fromBytes` | (`bytes`: `Uint8Array`) => [`Field`](#classesfieldmd)[] |
| `Fq.toBytes` | (`fields`: [`Field`](#classesfieldmd)[]) => `Uint8Array` |
| `Fq.fromString` | [object Object] |
| `Fq.toString` | [object Object] |

##### Defined in

[lib/encoding.ts:88](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/encoding.ts#L88)

___

#### EpochSeed

• `Const` **EpochSeed**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `fromBase58` | (`base58`: `string`) => [`Field`](#classesfieldmd) |
| `toBase58` | (`field`: [`Field`](#classesfieldmd)) => `string` |

##### Defined in

[lib/encoding.ts:312](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/encoding.ts#L312)

___

#### LedgerHash

• `Const` **LedgerHash**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `fromBase58` | (`base58`: `string`) => [`Field`](#classesfieldmd) |
| `toBase58` | (`field`: [`Field`](#classesfieldmd)) => `string` |

##### Defined in

[lib/encoding.ts:308](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/encoding.ts#L308)

___

#### ReceiptChainHash

• `Const` **ReceiptChainHash**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `fromBase58` | (`base58`: `string`) => [`Field`](#classesfieldmd) |
| `toBase58` | (`field`: [`Field`](#classesfieldmd)) => `string` |

##### Defined in

[lib/encoding.ts:304](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/encoding.ts#L304)

___

#### StateHash

• `Const` **StateHash**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `fromBase58` | (`base58`: `string`) => [`Field`](#classesfieldmd) |
| `toBase58` | (`field`: [`Field`](#classesfieldmd)) => `string` |

##### Defined in

[lib/encoding.ts:316](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/encoding.ts#L316)

___

#### TokenId

• `Const` **TokenId**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `fromBase58` | (`base58`: `string`) => [`Field`](#classesfieldmd) |
| `toBase58` | (`field`: [`Field`](#classesfieldmd)) => `string` |

##### Defined in

[lib/encoding.ts:303](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/encoding.ts#L303)

### Functions

#### bytesFromFields

▸ **bytesFromFields**(`fields`): `Uint8Array`

##### Parameters

| Name | Type |
| :------ | :------ |
| `fields` | [`Field`](#classesfieldmd)[] |

##### Returns

`Uint8Array`

##### Defined in

[lib/encoding.ts:57](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/encoding.ts#L57)

___

#### bytesToFields

▸ **bytesToFields**(`bytes`): [`Field`](#classesfieldmd)[]

##### Parameters

| Name | Type |
| :------ | :------ |
| `bytes` | `Uint8Array` |

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[lib/encoding.ts:37](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/encoding.ts#L37)

___

#### stringFromFields

▸ **stringFromFields**(`fields`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `fields` | [`Field`](#classesfieldmd)[] |

##### Returns

`string`

##### Defined in

[lib/encoding.ts:30](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/encoding.ts#L30)

___

#### stringToFields

▸ **stringToFields**(`message`): [`Field`](#classesfieldmd)[]

##### Parameters

| Name | Type |
| :------ | :------ |
| `message` | `string` |

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[lib/encoding.ts:25](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/encoding.ts#L25)


<a name="modulesencryptionmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Encryption

## Namespace: Encryption

### Table of contents

#### Functions

- [decrypt](#decrypt)
- [encrypt](#encrypt)

### Functions

#### decrypt

▸ **decrypt**(`__namedParameters`, `privateKey`): [`Field`](#classesfieldmd)[]

##### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | `CipherText` |
| `privateKey` | [`PrivateKey`](#classesprivatekeymd) |

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[lib/encryption.ts:40](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/encryption.ts#L40)

___

#### encrypt

▸ **encrypt**(`message`, `otherPublicKey`): `Object`

##### Parameters

| Name | Type |
| :------ | :------ |
| `message` | [`Field`](#classesfieldmd)[] |
| `otherPublicKey` | [`PublicKey`](#classestypespublickeymd) |

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `cipherText` | [`Field`](#classesfieldmd)[] |
| `publicKey` | [`Group`](#classesgroupmd) |

##### Defined in

[lib/encryption.ts:12](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/encryption.ts#L12)


<a name="modulesexperimentalmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Experimental

## Namespace: Experimental

This module exposes APIs that are unstable, in the sense that the API surface is expected to change.
(Not unstable in the sense that they are less functional or tested than other parts.)

### Table of contents

#### Type Aliases

- [AsFieldsAndAux](#asfieldsandaux)

#### Variables

- [MerkleTree](#merkletree)
- [Reducer](#reducer)
- [jsLayout](#jslayout)

#### Functions

- [MerkleWitness](#merklewitness)
- [asFieldsAndAux](#asfieldsandaux-1)
- [createChildParty](#createchildparty)
- [memoizeWitness](#memoizewitness)
- [packToFields](#packtofields)

### Type Aliases

#### AsFieldsAndAux

Ƭ **AsFieldsAndAux**<`T`, `TJson`\>: `AsFieldsAndAux_`<`T`, `TJson`\>

##### Type parameters

| Name |
| :------ |
| `T` |
| `TJson` |

##### Defined in

[index.ts:93](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/index.ts#L93)

### Variables

#### MerkleTree

• **MerkleTree**: typeof `MerkleTree` = `Experimental_.MerkleTree`

##### Defined in

[index.ts:91](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/index.ts#L91)

___

#### Reducer

• **Reducer**: <T, A\>(`reducer`: { `actionType`: `T`  }) => `ReducerReturn`<`A`\> & { `initialActionsHash`: [`Field`](#classesfieldmd)  } = `Experimental_.Reducer`

##### Defined in

[index.ts:85](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/index.ts#L85)

___

#### jsLayout

• **jsLayout**: `Object` = `Experimental_.jsLayout`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `Parties` | { `docEntries`: { `feePayer`: ``null`` = null; `memo`: ``null`` = null; `otherParties`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `feePayer`: { `docEntries`: { `authorization`: ``null`` = null; `body`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `authorization`: { `type`: `string` = 'string' } ; `body`: { `docEntries`: { `fee`: ``null`` = null; `nonce`: ``null`` = null; `publicKey`: ``null`` = null; `validUntil`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `fee`: { `type`: `string` = 'UInt64' } ; `nonce`: { `type`: `string` = 'UInt32' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `validUntil`: { `inner`: { `type`: `string` = 'UInt32' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'FeePayerPartyBody'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'ZkappPartyFeePayer'; `type`: `string` = 'object' } ; `memo`: { `type`: `string` = 'string' } ; `otherParties`: { `inner`: { `docEntries`: { `authorization`: ``null`` = null; `body`: ``null`` = null } ; `docs`: `string` = 'A party to a zkApp transaction'; `entries`: { `authorization`: { `docEntries`: { `proof`: ``null`` = null; `signature`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `proof`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } ; `signature`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'Control'; `type`: `string` = 'object' } ; `body`: { `docEntries`: { `balanceChange`: ``null`` = null; `callData`: ``null`` = null; `callDepth`: ``null`` = null; `caller`: ``null`` = null; `events`: ``null`` = null; `incrementNonce`: ``null`` = null; `preconditions`: ``null`` = null; `publicKey`: ``null`` = null; `sequenceEvents`: ``null`` = null; `tokenId`: ``null`` = null; `update`: ``null`` = null; `useFullCommitment`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balanceChange`: { `docEntries`: { `magnitude`: ``null`` = null; `sgn`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `magnitude`: { `type`: `string` = 'UInt64' } ; `sgn`: { `type`: `string` = 'Sign' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceChange'; `type`: `string` = 'object' } ; `callData`: { `type`: `string` = 'Field' } ; `callDepth`: { `type`: `string` = 'number' } ; `caller`: { `type`: `string` = 'TokenId' } ; `events`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `incrementNonce`: { `type`: `string` = 'Bool' } ; `preconditions`: { `docEntries`: { `account`: ``null`` = null; `network`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `account`: { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } ; `network`: { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'Preconditions'; `type`: `string` = 'object' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `sequenceEvents`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `tokenId`: { `type`: `string` = 'TokenId' } ; `update`: { `docEntries`: { `appState`: ``null`` = null; `delegate`: ``null`` = null; `permissions`: ``null`` = null; `timing`: ``null`` = null; `tokenSymbol`: ``null`` = null; `verificationKey`: ``null`` = null; `votingFor`: ``null`` = null; `zkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `appState`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `permissions`: { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `timing`: { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `tokenSymbol`: { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `verificationKey`: { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `votingFor`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `zkappUri`: { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyUpdate'; `type`: `string` = 'object' } ; `useFullCommitment`: { `type`: `string` = 'Bool' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyBody'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'ZkappParty'; `type`: `string` = 'object' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'Parties'; `type`: `string` = 'object' } |
| `Parties.docEntries` | { `feePayer`: ``null`` = null; `memo`: ``null`` = null; `otherParties`: ``null`` = null } |
| `Parties.docEntries.feePayer` | ``null`` |
| `Parties.docEntries.memo` | ``null`` |
| `Parties.docEntries.otherParties` | ``null`` |
| `Parties.docs` | ``null`` |
| `Parties.entries` | { `feePayer`: { `docEntries`: { `authorization`: ``null`` = null; `body`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `authorization`: { `type`: `string` = 'string' } ; `body`: { `docEntries`: { `fee`: ``null`` = null; `nonce`: ``null`` = null; `publicKey`: ``null`` = null; `validUntil`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `fee`: { `type`: `string` = 'UInt64' } ; `nonce`: { `type`: `string` = 'UInt32' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `validUntil`: { `inner`: { `type`: `string` = 'UInt32' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'FeePayerPartyBody'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'ZkappPartyFeePayer'; `type`: `string` = 'object' } ; `memo`: { `type`: `string` = 'string' } ; `otherParties`: { `inner`: { `docEntries`: { `authorization`: ``null`` = null; `body`: ``null`` = null } ; `docs`: `string` = 'A party to a zkApp transaction'; `entries`: { `authorization`: { `docEntries`: { `proof`: ``null`` = null; `signature`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `proof`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } ; `signature`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'Control'; `type`: `string` = 'object' } ; `body`: { `docEntries`: { `balanceChange`: ``null`` = null; `callData`: ``null`` = null; `callDepth`: ``null`` = null; `caller`: ``null`` = null; `events`: ``null`` = null; `incrementNonce`: ``null`` = null; `preconditions`: ``null`` = null; `publicKey`: ``null`` = null; `sequenceEvents`: ``null`` = null; `tokenId`: ``null`` = null; `update`: ``null`` = null; `useFullCommitment`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balanceChange`: { `docEntries`: { `magnitude`: ``null`` = null; `sgn`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `magnitude`: { `type`: `string` = 'UInt64' } ; `sgn`: { `type`: `string` = 'Sign' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceChange'; `type`: `string` = 'object' } ; `callData`: { `type`: `string` = 'Field' } ; `callDepth`: { `type`: `string` = 'number' } ; `caller`: { `type`: `string` = 'TokenId' } ; `events`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `incrementNonce`: { `type`: `string` = 'Bool' } ; `preconditions`: { `docEntries`: { `account`: ``null`` = null; `network`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `account`: { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } ; `network`: { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'Preconditions'; `type`: `string` = 'object' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `sequenceEvents`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `tokenId`: { `type`: `string` = 'TokenId' } ; `update`: { `docEntries`: { `appState`: ``null`` = null; `delegate`: ``null`` = null; `permissions`: ``null`` = null; `timing`: ``null`` = null; `tokenSymbol`: ``null`` = null; `verificationKey`: ``null`` = null; `votingFor`: ``null`` = null; `zkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `appState`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `permissions`: { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `timing`: { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `tokenSymbol`: { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `verificationKey`: { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `votingFor`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `zkappUri`: { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyUpdate'; `type`: `string` = 'object' } ; `useFullCommitment`: { `type`: `string` = 'Bool' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyBody'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'ZkappParty'; `type`: `string` = 'object' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' }  } |
| `Parties.entries.feePayer` | { `docEntries`: { `authorization`: ``null`` = null; `body`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `authorization`: { `type`: `string` = 'string' } ; `body`: { `docEntries`: { `fee`: ``null`` = null; `nonce`: ``null`` = null; `publicKey`: ``null`` = null; `validUntil`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `fee`: { `type`: `string` = 'UInt64' } ; `nonce`: { `type`: `string` = 'UInt32' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `validUntil`: { `inner`: { `type`: `string` = 'UInt32' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'FeePayerPartyBody'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'ZkappPartyFeePayer'; `type`: `string` = 'object' } |
| `Parties.entries.feePayer.docEntries` | { `authorization`: ``null`` = null; `body`: ``null`` = null } |
| `Parties.entries.feePayer.docEntries.authorization` | ``null`` |
| `Parties.entries.feePayer.docEntries.body` | ``null`` |
| `Parties.entries.feePayer.docs` | ``null`` |
| `Parties.entries.feePayer.entries` | { `authorization`: { `type`: `string` = 'string' } ; `body`: { `docEntries`: { `fee`: ``null`` = null; `nonce`: ``null`` = null; `publicKey`: ``null`` = null; `validUntil`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `fee`: { `type`: `string` = 'UInt64' } ; `nonce`: { `type`: `string` = 'UInt32' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `validUntil`: { `inner`: { `type`: `string` = 'UInt32' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'FeePayerPartyBody'; `type`: `string` = 'object' }  } |
| `Parties.entries.feePayer.entries.authorization` | { `type`: `string` = 'string' } |
| `Parties.entries.feePayer.entries.authorization.type` | `string` |
| `Parties.entries.feePayer.entries.body` | { `docEntries`: { `fee`: ``null`` = null; `nonce`: ``null`` = null; `publicKey`: ``null`` = null; `validUntil`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `fee`: { `type`: `string` = 'UInt64' } ; `nonce`: { `type`: `string` = 'UInt32' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `validUntil`: { `inner`: { `type`: `string` = 'UInt32' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'FeePayerPartyBody'; `type`: `string` = 'object' } |
| `Parties.entries.feePayer.entries.body.docEntries` | { `fee`: ``null`` = null; `nonce`: ``null`` = null; `publicKey`: ``null`` = null; `validUntil`: ``null`` = null } |
| `Parties.entries.feePayer.entries.body.docEntries.fee` | ``null`` |
| `Parties.entries.feePayer.entries.body.docEntries.nonce` | ``null`` |
| `Parties.entries.feePayer.entries.body.docEntries.publicKey` | ``null`` |
| `Parties.entries.feePayer.entries.body.docEntries.validUntil` | ``null`` |
| `Parties.entries.feePayer.entries.body.docs` | ``null`` |
| `Parties.entries.feePayer.entries.body.entries` | { `fee`: { `type`: `string` = 'UInt64' } ; `nonce`: { `type`: `string` = 'UInt32' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `validUntil`: { `inner`: { `type`: `string` = 'UInt32' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } |
| `Parties.entries.feePayer.entries.body.entries.fee` | { `type`: `string` = 'UInt64' } |
| `Parties.entries.feePayer.entries.body.entries.fee.type` | `string` |
| `Parties.entries.feePayer.entries.body.entries.nonce` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.feePayer.entries.body.entries.nonce.type` | `string` |
| `Parties.entries.feePayer.entries.body.entries.publicKey` | { `type`: `string` = 'PublicKey' } |
| `Parties.entries.feePayer.entries.body.entries.publicKey.type` | `string` |
| `Parties.entries.feePayer.entries.body.entries.validUntil` | { `inner`: { `type`: `string` = 'UInt32' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } |
| `Parties.entries.feePayer.entries.body.entries.validUntil.inner` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.feePayer.entries.body.entries.validUntil.inner.type` | `string` |
| `Parties.entries.feePayer.entries.body.entries.validUntil.optionType` | `string` |
| `Parties.entries.feePayer.entries.body.entries.validUntil.type` | `string` |
| `Parties.entries.feePayer.entries.body.keys` | `string`[] |
| `Parties.entries.feePayer.entries.body.name` | `string` |
| `Parties.entries.feePayer.entries.body.type` | `string` |
| `Parties.entries.feePayer.keys` | `string`[] |
| `Parties.entries.feePayer.name` | `string` |
| `Parties.entries.feePayer.type` | `string` |
| `Parties.entries.memo` | { `type`: `string` = 'string' } |
| `Parties.entries.memo.type` | `string` |
| `Parties.entries.otherParties` | { `inner`: { `docEntries`: { `authorization`: ``null`` = null; `body`: ``null`` = null } ; `docs`: `string` = 'A party to a zkApp transaction'; `entries`: { `authorization`: { `docEntries`: { `proof`: ``null`` = null; `signature`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `proof`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } ; `signature`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'Control'; `type`: `string` = 'object' } ; `body`: { `docEntries`: { `balanceChange`: ``null`` = null; `callData`: ``null`` = null; `callDepth`: ``null`` = null; `caller`: ``null`` = null; `events`: ``null`` = null; `incrementNonce`: ``null`` = null; `preconditions`: ``null`` = null; `publicKey`: ``null`` = null; `sequenceEvents`: ``null`` = null; `tokenId`: ``null`` = null; `update`: ``null`` = null; `useFullCommitment`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balanceChange`: { `docEntries`: { `magnitude`: ``null`` = null; `sgn`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `magnitude`: { `type`: `string` = 'UInt64' } ; `sgn`: { `type`: `string` = 'Sign' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceChange'; `type`: `string` = 'object' } ; `callData`: { `type`: `string` = 'Field' } ; `callDepth`: { `type`: `string` = 'number' } ; `caller`: { `type`: `string` = 'TokenId' } ; `events`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `incrementNonce`: { `type`: `string` = 'Bool' } ; `preconditions`: { `docEntries`: { `account`: ``null`` = null; `network`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `account`: { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } ; `network`: { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'Preconditions'; `type`: `string` = 'object' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `sequenceEvents`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `tokenId`: { `type`: `string` = 'TokenId' } ; `update`: { `docEntries`: { `appState`: ``null`` = null; `delegate`: ``null`` = null; `permissions`: ``null`` = null; `timing`: ``null`` = null; `tokenSymbol`: ``null`` = null; `verificationKey`: ``null`` = null; `votingFor`: ``null`` = null; `zkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `appState`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `permissions`: { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `timing`: { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `tokenSymbol`: { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `verificationKey`: { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `votingFor`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `zkappUri`: { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyUpdate'; `type`: `string` = 'object' } ; `useFullCommitment`: { `type`: `string` = 'Bool' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyBody'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'ZkappParty'; `type`: `string` = 'object' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Parties.entries.otherParties.inner` | { `docEntries`: { `authorization`: ``null`` = null; `body`: ``null`` = null } ; `docs`: `string` = 'A party to a zkApp transaction'; `entries`: { `authorization`: { `docEntries`: { `proof`: ``null`` = null; `signature`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `proof`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } ; `signature`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'Control'; `type`: `string` = 'object' } ; `body`: { `docEntries`: { `balanceChange`: ``null`` = null; `callData`: ``null`` = null; `callDepth`: ``null`` = null; `caller`: ``null`` = null; `events`: ``null`` = null; `incrementNonce`: ``null`` = null; `preconditions`: ``null`` = null; `publicKey`: ``null`` = null; `sequenceEvents`: ``null`` = null; `tokenId`: ``null`` = null; `update`: ``null`` = null; `useFullCommitment`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balanceChange`: { `docEntries`: { `magnitude`: ``null`` = null; `sgn`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `magnitude`: { `type`: `string` = 'UInt64' } ; `sgn`: { `type`: `string` = 'Sign' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceChange'; `type`: `string` = 'object' } ; `callData`: { `type`: `string` = 'Field' } ; `callDepth`: { `type`: `string` = 'number' } ; `caller`: { `type`: `string` = 'TokenId' } ; `events`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `incrementNonce`: { `type`: `string` = 'Bool' } ; `preconditions`: { `docEntries`: { `account`: ``null`` = null; `network`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `account`: { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } ; `network`: { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'Preconditions'; `type`: `string` = 'object' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `sequenceEvents`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `tokenId`: { `type`: `string` = 'TokenId' } ; `update`: { `docEntries`: { `appState`: ``null`` = null; `delegate`: ``null`` = null; `permissions`: ``null`` = null; `timing`: ``null`` = null; `tokenSymbol`: ``null`` = null; `verificationKey`: ``null`` = null; `votingFor`: ``null`` = null; `zkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `appState`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `permissions`: { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `timing`: { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `tokenSymbol`: { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `verificationKey`: { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `votingFor`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `zkappUri`: { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyUpdate'; `type`: `string` = 'object' } ; `useFullCommitment`: { `type`: `string` = 'Bool' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyBody'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'ZkappParty'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.docEntries` | { `authorization`: ``null`` = null; `body`: ``null`` = null } |
| `Parties.entries.otherParties.inner.docEntries.authorization` | ``null`` |
| `Parties.entries.otherParties.inner.docEntries.body` | ``null`` |
| `Parties.entries.otherParties.inner.docs` | `string` |
| `Parties.entries.otherParties.inner.entries` | { `authorization`: { `docEntries`: { `proof`: ``null`` = null; `signature`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `proof`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } ; `signature`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'Control'; `type`: `string` = 'object' } ; `body`: { `docEntries`: { `balanceChange`: ``null`` = null; `callData`: ``null`` = null; `callDepth`: ``null`` = null; `caller`: ``null`` = null; `events`: ``null`` = null; `incrementNonce`: ``null`` = null; `preconditions`: ``null`` = null; `publicKey`: ``null`` = null; `sequenceEvents`: ``null`` = null; `tokenId`: ``null`` = null; `update`: ``null`` = null; `useFullCommitment`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balanceChange`: { `docEntries`: { `magnitude`: ``null`` = null; `sgn`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `magnitude`: { `type`: `string` = 'UInt64' } ; `sgn`: { `type`: `string` = 'Sign' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceChange'; `type`: `string` = 'object' } ; `callData`: { `type`: `string` = 'Field' } ; `callDepth`: { `type`: `string` = 'number' } ; `caller`: { `type`: `string` = 'TokenId' } ; `events`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `incrementNonce`: { `type`: `string` = 'Bool' } ; `preconditions`: { `docEntries`: { `account`: ``null`` = null; `network`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `account`: { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } ; `network`: { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'Preconditions'; `type`: `string` = 'object' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `sequenceEvents`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `tokenId`: { `type`: `string` = 'TokenId' } ; `update`: { `docEntries`: { `appState`: ``null`` = null; `delegate`: ``null`` = null; `permissions`: ``null`` = null; `timing`: ``null`` = null; `tokenSymbol`: ``null`` = null; `verificationKey`: ``null`` = null; `votingFor`: ``null`` = null; `zkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `appState`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `permissions`: { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `timing`: { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `tokenSymbol`: { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `verificationKey`: { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `votingFor`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `zkappUri`: { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyUpdate'; `type`: `string` = 'object' } ; `useFullCommitment`: { `type`: `string` = 'Bool' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyBody'; `type`: `string` = 'object' }  } |
| `Parties.entries.otherParties.inner.entries.authorization` | { `docEntries`: { `proof`: ``null`` = null; `signature`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `proof`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } ; `signature`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'Control'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.authorization.docEntries` | { `proof`: ``null`` = null; `signature`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.authorization.docEntries.proof` | ``null`` |
| `Parties.entries.otherParties.inner.entries.authorization.docEntries.signature` | ``null`` |
| `Parties.entries.otherParties.inner.entries.authorization.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.authorization.entries` | { `proof`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } ; `signature`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } |
| `Parties.entries.otherParties.inner.entries.authorization.entries.proof` | { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.authorization.entries.proof.inner` | { `type`: `string` = 'string' } |
| `Parties.entries.otherParties.inner.entries.authorization.entries.proof.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.authorization.entries.proof.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.authorization.entries.proof.type` | `string` |
| `Parties.entries.otherParties.inner.entries.authorization.entries.signature` | { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.authorization.entries.signature.inner` | { `type`: `string` = 'string' } |
| `Parties.entries.otherParties.inner.entries.authorization.entries.signature.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.authorization.entries.signature.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.authorization.entries.signature.type` | `string` |
| `Parties.entries.otherParties.inner.entries.authorization.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.authorization.name` | `string` |
| `Parties.entries.otherParties.inner.entries.authorization.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body` | { `docEntries`: { `balanceChange`: ``null`` = null; `callData`: ``null`` = null; `callDepth`: ``null`` = null; `caller`: ``null`` = null; `events`: ``null`` = null; `incrementNonce`: ``null`` = null; `preconditions`: ``null`` = null; `publicKey`: ``null`` = null; `sequenceEvents`: ``null`` = null; `tokenId`: ``null`` = null; `update`: ``null`` = null; `useFullCommitment`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balanceChange`: { `docEntries`: { `magnitude`: ``null`` = null; `sgn`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `magnitude`: { `type`: `string` = 'UInt64' } ; `sgn`: { `type`: `string` = 'Sign' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceChange'; `type`: `string` = 'object' } ; `callData`: { `type`: `string` = 'Field' } ; `callDepth`: { `type`: `string` = 'number' } ; `caller`: { `type`: `string` = 'TokenId' } ; `events`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `incrementNonce`: { `type`: `string` = 'Bool' } ; `preconditions`: { `docEntries`: { `account`: ``null`` = null; `network`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `account`: { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } ; `network`: { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'Preconditions'; `type`: `string` = 'object' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `sequenceEvents`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `tokenId`: { `type`: `string` = 'TokenId' } ; `update`: { `docEntries`: { `appState`: ``null`` = null; `delegate`: ``null`` = null; `permissions`: ``null`` = null; `timing`: ``null`` = null; `tokenSymbol`: ``null`` = null; `verificationKey`: ``null`` = null; `votingFor`: ``null`` = null; `zkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `appState`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `permissions`: { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `timing`: { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `tokenSymbol`: { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `verificationKey`: { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `votingFor`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `zkappUri`: { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyUpdate'; `type`: `string` = 'object' } ; `useFullCommitment`: { `type`: `string` = 'Bool' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyBody'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.docEntries` | { `balanceChange`: ``null`` = null; `callData`: ``null`` = null; `callDepth`: ``null`` = null; `caller`: ``null`` = null; `events`: ``null`` = null; `incrementNonce`: ``null`` = null; `preconditions`: ``null`` = null; `publicKey`: ``null`` = null; `sequenceEvents`: ``null`` = null; `tokenId`: ``null`` = null; `update`: ``null`` = null; `useFullCommitment`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.docEntries.balanceChange` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.docEntries.callData` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.docEntries.callDepth` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.docEntries.caller` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.docEntries.events` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.docEntries.incrementNonce` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.docEntries.preconditions` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.docEntries.publicKey` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.docEntries.sequenceEvents` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.docEntries.tokenId` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.docEntries.update` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.docEntries.useFullCommitment` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries` | { `balanceChange`: { `docEntries`: { `magnitude`: ``null`` = null; `sgn`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `magnitude`: { `type`: `string` = 'UInt64' } ; `sgn`: { `type`: `string` = 'Sign' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceChange'; `type`: `string` = 'object' } ; `callData`: { `type`: `string` = 'Field' } ; `callDepth`: { `type`: `string` = 'number' } ; `caller`: { `type`: `string` = 'TokenId' } ; `events`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `incrementNonce`: { `type`: `string` = 'Bool' } ; `preconditions`: { `docEntries`: { `account`: ``null`` = null; `network`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `account`: { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } ; `network`: { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'Preconditions'; `type`: `string` = 'object' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `sequenceEvents`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `tokenId`: { `type`: `string` = 'TokenId' } ; `update`: { `docEntries`: { `appState`: ``null`` = null; `delegate`: ``null`` = null; `permissions`: ``null`` = null; `timing`: ``null`` = null; `tokenSymbol`: ``null`` = null; `verificationKey`: ``null`` = null; `votingFor`: ``null`` = null; `zkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `appState`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `permissions`: { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `timing`: { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `tokenSymbol`: { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `verificationKey`: { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `votingFor`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `zkappUri`: { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyUpdate'; `type`: `string` = 'object' } ; `useFullCommitment`: { `type`: `string` = 'Bool' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.balanceChange` | { `docEntries`: { `magnitude`: ``null`` = null; `sgn`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `magnitude`: { `type`: `string` = 'UInt64' } ; `sgn`: { `type`: `string` = 'Sign' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceChange'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.balanceChange.docEntries` | { `magnitude`: ``null`` = null; `sgn`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.balanceChange.docEntries.magnitude` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.balanceChange.docEntries.sgn` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.balanceChange.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.balanceChange.entries` | { `magnitude`: { `type`: `string` = 'UInt64' } ; `sgn`: { `type`: `string` = 'Sign' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.balanceChange.entries.magnitude` | { `type`: `string` = 'UInt64' } |
| `Parties.entries.otherParties.inner.entries.body.entries.balanceChange.entries.magnitude.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.balanceChange.entries.sgn` | { `type`: `string` = 'Sign' } |
| `Parties.entries.otherParties.inner.entries.body.entries.balanceChange.entries.sgn.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.balanceChange.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.balanceChange.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.balanceChange.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.callData` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.callData.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.callDepth` | { `type`: `string` = 'number' } |
| `Parties.entries.otherParties.inner.entries.body.entries.callDepth.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.caller` | { `type`: `string` = 'TokenId' } |
| `Parties.entries.otherParties.inner.entries.body.entries.caller.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.events` | { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType` | { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.docEntries` | { `data`: ``null`` = null; `hash`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.docEntries.data` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.docEntries.hash` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.entries` | { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.entries.data` | { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.entries.data.inner` | { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.entries.data.inner.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.entries.data.inner.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.entries.data.inner.staticLength` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.entries.data.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.entries.data.staticLength` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.entries.data.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.entries.hash` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.entries.hash.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedType.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.checkedTypeName` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.inner` | { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Parties.entries.otherParties.inner.entries.body.entries.events.inner.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.events.inner.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.inner.staticLength` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.staticLength` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.events.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.incrementNonce` | { `type`: `string` = 'Bool' } |
| `Parties.entries.otherParties.inner.entries.body.entries.incrementNonce.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions` | { `docEntries`: { `account`: ``null`` = null; `network`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `account`: { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } ; `network`: { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'Preconditions'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.docEntries` | { `account`: ``null`` = null; `network`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.docEntries.account` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.docEntries.network` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries` | { `account`: { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } ; `network`: { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account` | { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.docEntries` | { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.docEntries.balance` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.docEntries.delegate` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.docEntries.isNew` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.docEntries.nonce` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.docEntries.provedState` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.docEntries.receiptChainHash` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.docEntries.sequenceState` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.docEntries.state` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries` | { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance.inner.docEntries.lower` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance.inner.docEntries.upper` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance.inner.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance.inner.entries` | { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance.inner.entries.lower` | { `type`: `string` = 'UInt64' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance.inner.entries.lower.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance.inner.entries.upper` | { `type`: `string` = 'UInt64' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance.inner.entries.upper.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance.inner.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.balance.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.delegate` | { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.delegate.inner` | { `type`: `string` = 'PublicKey' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.delegate.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.delegate.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.delegate.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.isNew` | { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.isNew.inner` | { `type`: `string` = 'Bool' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.isNew.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.isNew.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.isNew.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce.inner.docEntries.lower` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce.inner.docEntries.upper` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce.inner.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce.inner.entries` | { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce.inner.entries.lower` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce.inner.entries.lower.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce.inner.entries.upper` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce.inner.entries.upper.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce.inner.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.nonce.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.provedState` | { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.provedState.inner` | { `type`: `string` = 'Bool' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.provedState.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.provedState.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.provedState.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.receiptChainHash` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.receiptChainHash.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.receiptChainHash.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.receiptChainHash.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.receiptChainHash.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.sequenceState` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.sequenceState.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.sequenceState.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.sequenceState.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.sequenceState.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.state` | { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.state.inner` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.state.inner.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.state.inner.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.state.inner.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.state.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.state.staticLength` | `number` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.entries.state.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.account.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network` | { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.docEntries` | { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.docEntries.blockchainLength` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.docEntries.globalSlotSinceGenesis` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.docEntries.globalSlotSinceHardFork` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.docEntries.minWindowDensity` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.docEntries.nextEpochData` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.docEntries.snarkedLedgerHash` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.docEntries.stakingEpochData` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.docEntries.timestamp` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.docEntries.totalCurrency` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries` | { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.docEntries.lower` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.docEntries.upper` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.entries` | { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.entries.lower` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.entries.lower.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.entries.upper` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.entries.upper.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.blockchainLength.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.docEntries.lower` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.docEntries.upper` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.entries` | { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.entries.lower` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.entries.lower.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.entries.upper` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.entries.upper.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.docEntries.lower` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.docEntries.upper` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.entries` | { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.entries.lower` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.entries.lower.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.entries.upper` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.entries.upper.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.docEntries.lower` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.docEntries.upper` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.entries` | { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.entries.lower` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.entries.lower.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.entries.upper` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.entries.upper.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData` | { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.docEntries` | { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.docEntries.epochLength` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.docEntries.ledger` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.docEntries.lockCheckpoint` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.docEntries.seed` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.docEntries.startCheckpoint` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries` | { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.docEntries.lower` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.docEntries.upper` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.entries` | { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.entries.lower` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.entries.lower.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.entries.upper` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.entries.upper.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger` | { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.docEntries` | { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.docEntries.hash` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.docEntries.totalCurrency` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries` | { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.hash` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.hash.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.hash.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.hash.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.hash.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.docEntries.lower` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.docEntries.upper` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.entries` | { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.entries.lower` | { `type`: `string` = 'UInt64' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.entries.lower.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.entries.upper` | { `type`: `string` = 'UInt64' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.entries.upper.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.lockCheckpoint` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.lockCheckpoint.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.lockCheckpoint.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.lockCheckpoint.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.lockCheckpoint.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.seed` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.seed.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.seed.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.seed.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.seed.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.startCheckpoint` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.startCheckpoint.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.startCheckpoint.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.startCheckpoint.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.startCheckpoint.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.nextEpochData.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.snarkedLedgerHash` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.snarkedLedgerHash.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.snarkedLedgerHash.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.snarkedLedgerHash.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.snarkedLedgerHash.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData` | { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.docEntries` | { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.docEntries.epochLength` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.docEntries.ledger` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.docEntries.lockCheckpoint` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.docEntries.seed` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.docEntries.startCheckpoint` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries` | { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.docEntries.lower` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.docEntries.upper` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.entries` | { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.entries.lower` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.entries.lower.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.entries.upper` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.entries.upper.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger` | { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.docEntries` | { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.docEntries.hash` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.docEntries.totalCurrency` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries` | { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.hash` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.hash.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.hash.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.hash.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.hash.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.docEntries.lower` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.docEntries.upper` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.entries` | { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.entries.lower` | { `type`: `string` = 'UInt64' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.entries.lower.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.entries.upper` | { `type`: `string` = 'UInt64' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.entries.upper.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.lockCheckpoint` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.lockCheckpoint.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.lockCheckpoint.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.lockCheckpoint.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.lockCheckpoint.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.seed` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.seed.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.seed.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.seed.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.seed.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.startCheckpoint` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.startCheckpoint.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.startCheckpoint.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.startCheckpoint.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.startCheckpoint.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.docEntries.lower` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.docEntries.upper` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.entries` | { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.entries.lower` | { `type`: `string` = 'UInt64' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.entries.lower.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.entries.upper` | { `type`: `string` = 'UInt64' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.entries.upper.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.timestamp.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.docEntries.lower` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.docEntries.upper` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.entries` | { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.entries.lower` | { `type`: `string` = 'UInt64' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.entries.lower.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.entries.upper` | { `type`: `string` = 'UInt64' } |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.entries.upper.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.entries.totalCurrency.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.entries.network.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.preconditions.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.publicKey` | { `type`: `string` = 'PublicKey' } |
| `Parties.entries.otherParties.inner.entries.body.entries.publicKey.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents` | { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType` | { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.docEntries` | { `data`: ``null`` = null; `hash`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.docEntries.data` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.docEntries.hash` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.entries` | { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.entries.data` | { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.entries.data.inner` | { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.entries.data.inner.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.entries.data.inner.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.entries.data.inner.staticLength` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.entries.data.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.entries.data.staticLength` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.entries.data.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.entries.hash` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.entries.hash.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedType.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.checkedTypeName` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.inner` | { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.inner.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.inner.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.inner.staticLength` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.staticLength` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.sequenceEvents.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.tokenId` | { `type`: `string` = 'TokenId' } |
| `Parties.entries.otherParties.inner.entries.body.entries.tokenId.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update` | { `docEntries`: { `appState`: ``null`` = null; `delegate`: ``null`` = null; `permissions`: ``null`` = null; `timing`: ``null`` = null; `tokenSymbol`: ``null`` = null; `verificationKey`: ``null`` = null; `votingFor`: ``null`` = null; `zkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `appState`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `permissions`: { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `timing`: { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `tokenSymbol`: { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `verificationKey`: { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `votingFor`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `zkappUri`: { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyUpdate'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.docEntries` | { `appState`: ``null`` = null; `delegate`: ``null`` = null; `permissions`: ``null`` = null; `timing`: ``null`` = null; `tokenSymbol`: ``null`` = null; `verificationKey`: ``null`` = null; `votingFor`: ``null`` = null; `zkappUri`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.docEntries.appState` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.docEntries.delegate` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.docEntries.permissions` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.docEntries.timing` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.docEntries.tokenSymbol` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.docEntries.verificationKey` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.docEntries.votingFor` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.docEntries.zkappUri` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries` | { `appState`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `permissions`: { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `timing`: { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `tokenSymbol`: { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `verificationKey`: { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `votingFor`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `zkappUri`: { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.appState` | { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.appState.inner` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.appState.inner.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.appState.inner.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.appState.inner.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.appState.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.appState.staticLength` | `number` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.appState.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.delegate` | { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.delegate.inner` | { `type`: `string` = 'PublicKey' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.delegate.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.delegate.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.delegate.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions` | { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner` | { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.docEntries` | { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.docEntries.editSequenceState` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.docEntries.editState` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.docEntries.incrementNonce` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.docEntries.receive` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.docEntries.send` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.docEntries.setDelegate` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.docEntries.setPermissions` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.docEntries.setTokenSymbol` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.docEntries.setVerificationKey` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.docEntries.setVotingFor` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.docEntries.setZkappUri` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries` | { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.editSequenceState` | { `type`: `string` = 'AuthRequired' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.editSequenceState.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.editState` | { `type`: `string` = 'AuthRequired' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.editState.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.incrementNonce` | { `type`: `string` = 'AuthRequired' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.incrementNonce.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.receive` | { `type`: `string` = 'AuthRequired' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.receive.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.send` | { `type`: `string` = 'AuthRequired' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.send.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.setDelegate` | { `type`: `string` = 'AuthRequired' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.setDelegate.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.setPermissions` | { `type`: `string` = 'AuthRequired' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.setPermissions.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.setTokenSymbol` | { `type`: `string` = 'AuthRequired' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.setTokenSymbol.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.setVerificationKey` | { `type`: `string` = 'AuthRequired' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.setVerificationKey.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.setVotingFor` | { `type`: `string` = 'AuthRequired' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.setVotingFor.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.setZkappUri` | { `type`: `string` = 'AuthRequired' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.entries.setZkappUri.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.permissions.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing` | { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner` | { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.docEntries` | { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.docEntries.cliffAmount` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.docEntries.cliffTime` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.docEntries.initialMinimumBalance` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.docEntries.vestingIncrement` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.docEntries.vestingPeriod` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.entries` | { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.entries.cliffAmount` | { `type`: `string` = 'UInt64' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.entries.cliffAmount.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.entries.cliffTime` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.entries.cliffTime.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.entries.initialMinimumBalance` | { `type`: `string` = 'UInt64' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.entries.initialMinimumBalance.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.entries.vestingIncrement` | { `type`: `string` = 'UInt64' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.entries.vestingIncrement.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.entries.vestingPeriod` | { `type`: `string` = 'UInt32' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.entries.vestingPeriod.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.timing.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.tokenSymbol` | { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.tokenSymbol.inner` | { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.tokenSymbol.inner.checkedType` | { `type`: `string` = 'TokenSymbol' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.tokenSymbol.inner.checkedType.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.tokenSymbol.inner.checkedTypeName` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.tokenSymbol.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.tokenSymbol.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.tokenSymbol.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey` | { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey.inner` | { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey.inner.docEntries` | { `data`: ``null`` = null; `hash`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey.inner.docEntries.data` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey.inner.docEntries.hash` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey.inner.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey.inner.entries` | { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey.inner.entries.data` | { `type`: `string` = 'string' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey.inner.entries.data.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey.inner.entries.hash` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey.inner.entries.hash.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey.inner.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.verificationKey.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.votingFor` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.votingFor.inner` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.votingFor.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.votingFor.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.votingFor.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri` | { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner` | { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner.checkedType` | { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner.checkedType.docEntries` | { `data`: ``null`` = null; `hash`: ``null`` = null } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner.checkedType.docEntries.data` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner.checkedType.docEntries.hash` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner.checkedType.docs` | ``null`` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner.checkedType.entries` | { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner.checkedType.entries.data` | { `type`: `string` = 'string' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner.checkedType.entries.data.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner.checkedType.entries.hash` | { `type`: `string` = 'Field' } |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner.checkedType.entries.hash.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner.checkedType.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner.checkedType.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner.checkedType.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner.checkedTypeName` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.inner.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.optionType` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.entries.zkappUri.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.entries.update.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.update.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.entries.useFullCommitment` | { `type`: `string` = 'Bool' } |
| `Parties.entries.otherParties.inner.entries.body.entries.useFullCommitment.type` | `string` |
| `Parties.entries.otherParties.inner.entries.body.keys` | `string`[] |
| `Parties.entries.otherParties.inner.entries.body.name` | `string` |
| `Parties.entries.otherParties.inner.entries.body.type` | `string` |
| `Parties.entries.otherParties.inner.keys` | `string`[] |
| `Parties.entries.otherParties.inner.name` | `string` |
| `Parties.entries.otherParties.inner.type` | `string` |
| `Parties.entries.otherParties.staticLength` | ``null`` |
| `Parties.entries.otherParties.type` | `string` |
| `Parties.keys` | `string`[] |
| `Parties.name` | `string` |
| `Parties.type` | `string` |
| `Party` | { `docEntries`: { `authorization`: ``null`` = null; `body`: ``null`` = null } ; `docs`: `string` = 'A party to a zkApp transaction'; `entries`: { `authorization`: { `docEntries`: { `proof`: ``null`` = null; `signature`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `proof`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } ; `signature`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'Control'; `type`: `string` = 'object' } ; `body`: { `docEntries`: { `balanceChange`: ``null`` = null; `callData`: ``null`` = null; `callDepth`: ``null`` = null; `caller`: ``null`` = null; `events`: ``null`` = null; `incrementNonce`: ``null`` = null; `preconditions`: ``null`` = null; `publicKey`: ``null`` = null; `sequenceEvents`: ``null`` = null; `tokenId`: ``null`` = null; `update`: ``null`` = null; `useFullCommitment`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balanceChange`: { `docEntries`: { `magnitude`: ``null`` = null; `sgn`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `magnitude`: { `type`: `string` = 'UInt64' } ; `sgn`: { `type`: `string` = 'Sign' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceChange'; `type`: `string` = 'object' } ; `callData`: { `type`: `string` = 'Field' } ; `callDepth`: { `type`: `string` = 'number' } ; `caller`: { `type`: `string` = 'TokenId' } ; `events`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `incrementNonce`: { `type`: `string` = 'Bool' } ; `preconditions`: { `docEntries`: { `account`: ``null`` = null; `network`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `account`: { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } ; `network`: { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'Preconditions'; `type`: `string` = 'object' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `sequenceEvents`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `tokenId`: { `type`: `string` = 'TokenId' } ; `update`: { `docEntries`: { `appState`: ``null`` = null; `delegate`: ``null`` = null; `permissions`: ``null`` = null; `timing`: ``null`` = null; `tokenSymbol`: ``null`` = null; `verificationKey`: ``null`` = null; `votingFor`: ``null`` = null; `zkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `appState`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `permissions`: { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `timing`: { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `tokenSymbol`: { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `verificationKey`: { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `votingFor`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `zkappUri`: { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyUpdate'; `type`: `string` = 'object' } ; `useFullCommitment`: { `type`: `string` = 'Bool' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyBody'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'ZkappParty'; `type`: `string` = 'object' } |
| `Party.docEntries` | { `authorization`: ``null`` = null; `body`: ``null`` = null } |
| `Party.docEntries.authorization` | ``null`` |
| `Party.docEntries.body` | ``null`` |
| `Party.docs` | `string` |
| `Party.entries` | { `authorization`: { `docEntries`: { `proof`: ``null`` = null; `signature`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `proof`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } ; `signature`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'Control'; `type`: `string` = 'object' } ; `body`: { `docEntries`: { `balanceChange`: ``null`` = null; `callData`: ``null`` = null; `callDepth`: ``null`` = null; `caller`: ``null`` = null; `events`: ``null`` = null; `incrementNonce`: ``null`` = null; `preconditions`: ``null`` = null; `publicKey`: ``null`` = null; `sequenceEvents`: ``null`` = null; `tokenId`: ``null`` = null; `update`: ``null`` = null; `useFullCommitment`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balanceChange`: { `docEntries`: { `magnitude`: ``null`` = null; `sgn`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `magnitude`: { `type`: `string` = 'UInt64' } ; `sgn`: { `type`: `string` = 'Sign' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceChange'; `type`: `string` = 'object' } ; `callData`: { `type`: `string` = 'Field' } ; `callDepth`: { `type`: `string` = 'number' } ; `caller`: { `type`: `string` = 'TokenId' } ; `events`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `incrementNonce`: { `type`: `string` = 'Bool' } ; `preconditions`: { `docEntries`: { `account`: ``null`` = null; `network`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `account`: { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } ; `network`: { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'Preconditions'; `type`: `string` = 'object' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `sequenceEvents`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `tokenId`: { `type`: `string` = 'TokenId' } ; `update`: { `docEntries`: { `appState`: ``null`` = null; `delegate`: ``null`` = null; `permissions`: ``null`` = null; `timing`: ``null`` = null; `tokenSymbol`: ``null`` = null; `verificationKey`: ``null`` = null; `votingFor`: ``null`` = null; `zkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `appState`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `permissions`: { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `timing`: { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `tokenSymbol`: { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `verificationKey`: { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `votingFor`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `zkappUri`: { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyUpdate'; `type`: `string` = 'object' } ; `useFullCommitment`: { `type`: `string` = 'Bool' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyBody'; `type`: `string` = 'object' }  } |
| `Party.entries.authorization` | { `docEntries`: { `proof`: ``null`` = null; `signature`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `proof`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } ; `signature`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'Control'; `type`: `string` = 'object' } |
| `Party.entries.authorization.docEntries` | { `proof`: ``null`` = null; `signature`: ``null`` = null } |
| `Party.entries.authorization.docEntries.proof` | ``null`` |
| `Party.entries.authorization.docEntries.signature` | ``null`` |
| `Party.entries.authorization.docs` | ``null`` |
| `Party.entries.authorization.entries` | { `proof`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } ; `signature`: { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' }  } |
| `Party.entries.authorization.entries.proof` | { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } |
| `Party.entries.authorization.entries.proof.inner` | { `type`: `string` = 'string' } |
| `Party.entries.authorization.entries.proof.inner.type` | `string` |
| `Party.entries.authorization.entries.proof.optionType` | `string` |
| `Party.entries.authorization.entries.proof.type` | `string` |
| `Party.entries.authorization.entries.signature` | { `inner`: { `type`: `string` = 'string' } ; `optionType`: `string` = 'orUndefined'; `type`: `string` = 'option' } |
| `Party.entries.authorization.entries.signature.inner` | { `type`: `string` = 'string' } |
| `Party.entries.authorization.entries.signature.inner.type` | `string` |
| `Party.entries.authorization.entries.signature.optionType` | `string` |
| `Party.entries.authorization.entries.signature.type` | `string` |
| `Party.entries.authorization.keys` | `string`[] |
| `Party.entries.authorization.name` | `string` |
| `Party.entries.authorization.type` | `string` |
| `Party.entries.body` | { `docEntries`: { `balanceChange`: ``null`` = null; `callData`: ``null`` = null; `callDepth`: ``null`` = null; `caller`: ``null`` = null; `events`: ``null`` = null; `incrementNonce`: ``null`` = null; `preconditions`: ``null`` = null; `publicKey`: ``null`` = null; `sequenceEvents`: ``null`` = null; `tokenId`: ``null`` = null; `update`: ``null`` = null; `useFullCommitment`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balanceChange`: { `docEntries`: { `magnitude`: ``null`` = null; `sgn`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `magnitude`: { `type`: `string` = 'UInt64' } ; `sgn`: { `type`: `string` = 'Sign' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceChange'; `type`: `string` = 'object' } ; `callData`: { `type`: `string` = 'Field' } ; `callDepth`: { `type`: `string` = 'number' } ; `caller`: { `type`: `string` = 'TokenId' } ; `events`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `incrementNonce`: { `type`: `string` = 'Bool' } ; `preconditions`: { `docEntries`: { `account`: ``null`` = null; `network`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `account`: { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } ; `network`: { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'Preconditions'; `type`: `string` = 'object' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `sequenceEvents`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `tokenId`: { `type`: `string` = 'TokenId' } ; `update`: { `docEntries`: { `appState`: ``null`` = null; `delegate`: ``null`` = null; `permissions`: ``null`` = null; `timing`: ``null`` = null; `tokenSymbol`: ``null`` = null; `verificationKey`: ``null`` = null; `votingFor`: ``null`` = null; `zkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `appState`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `permissions`: { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `timing`: { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `tokenSymbol`: { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `verificationKey`: { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `votingFor`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `zkappUri`: { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyUpdate'; `type`: `string` = 'object' } ; `useFullCommitment`: { `type`: `string` = 'Bool' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyBody'; `type`: `string` = 'object' } |
| `Party.entries.body.docEntries` | { `balanceChange`: ``null`` = null; `callData`: ``null`` = null; `callDepth`: ``null`` = null; `caller`: ``null`` = null; `events`: ``null`` = null; `incrementNonce`: ``null`` = null; `preconditions`: ``null`` = null; `publicKey`: ``null`` = null; `sequenceEvents`: ``null`` = null; `tokenId`: ``null`` = null; `update`: ``null`` = null; `useFullCommitment`: ``null`` = null } |
| `Party.entries.body.docEntries.balanceChange` | ``null`` |
| `Party.entries.body.docEntries.callData` | ``null`` |
| `Party.entries.body.docEntries.callDepth` | ``null`` |
| `Party.entries.body.docEntries.caller` | ``null`` |
| `Party.entries.body.docEntries.events` | ``null`` |
| `Party.entries.body.docEntries.incrementNonce` | ``null`` |
| `Party.entries.body.docEntries.preconditions` | ``null`` |
| `Party.entries.body.docEntries.publicKey` | ``null`` |
| `Party.entries.body.docEntries.sequenceEvents` | ``null`` |
| `Party.entries.body.docEntries.tokenId` | ``null`` |
| `Party.entries.body.docEntries.update` | ``null`` |
| `Party.entries.body.docEntries.useFullCommitment` | ``null`` |
| `Party.entries.body.docs` | ``null`` |
| `Party.entries.body.entries` | { `balanceChange`: { `docEntries`: { `magnitude`: ``null`` = null; `sgn`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `magnitude`: { `type`: `string` = 'UInt64' } ; `sgn`: { `type`: `string` = 'Sign' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceChange'; `type`: `string` = 'object' } ; `callData`: { `type`: `string` = 'Field' } ; `callDepth`: { `type`: `string` = 'number' } ; `caller`: { `type`: `string` = 'TokenId' } ; `events`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `incrementNonce`: { `type`: `string` = 'Bool' } ; `preconditions`: { `docEntries`: { `account`: ``null`` = null; `network`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `account`: { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } ; `network`: { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'Preconditions'; `type`: `string` = 'object' } ; `publicKey`: { `type`: `string` = 'PublicKey' } ; `sequenceEvents`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `tokenId`: { `type`: `string` = 'TokenId' } ; `update`: { `docEntries`: { `appState`: ``null`` = null; `delegate`: ``null`` = null; `permissions`: ``null`` = null; `timing`: ``null`` = null; `tokenSymbol`: ``null`` = null; `verificationKey`: ``null`` = null; `votingFor`: ``null`` = null; `zkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `appState`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `permissions`: { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `timing`: { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `tokenSymbol`: { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `verificationKey`: { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `votingFor`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `zkappUri`: { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyUpdate'; `type`: `string` = 'object' } ; `useFullCommitment`: { `type`: `string` = 'Bool' }  } |
| `Party.entries.body.entries.balanceChange` | { `docEntries`: { `magnitude`: ``null`` = null; `sgn`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `magnitude`: { `type`: `string` = 'UInt64' } ; `sgn`: { `type`: `string` = 'Sign' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceChange'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.balanceChange.docEntries` | { `magnitude`: ``null`` = null; `sgn`: ``null`` = null } |
| `Party.entries.body.entries.balanceChange.docEntries.magnitude` | ``null`` |
| `Party.entries.body.entries.balanceChange.docEntries.sgn` | ``null`` |
| `Party.entries.body.entries.balanceChange.docs` | ``null`` |
| `Party.entries.body.entries.balanceChange.entries` | { `magnitude`: { `type`: `string` = 'UInt64' } ; `sgn`: { `type`: `string` = 'Sign' }  } |
| `Party.entries.body.entries.balanceChange.entries.magnitude` | { `type`: `string` = 'UInt64' } |
| `Party.entries.body.entries.balanceChange.entries.magnitude.type` | `string` |
| `Party.entries.body.entries.balanceChange.entries.sgn` | { `type`: `string` = 'Sign' } |
| `Party.entries.body.entries.balanceChange.entries.sgn.type` | `string` |
| `Party.entries.body.entries.balanceChange.keys` | `string`[] |
| `Party.entries.body.entries.balanceChange.name` | `string` |
| `Party.entries.body.entries.balanceChange.type` | `string` |
| `Party.entries.body.entries.callData` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.callData.type` | `string` |
| `Party.entries.body.entries.callDepth` | { `type`: `string` = 'number' } |
| `Party.entries.body.entries.callDepth.type` | `string` |
| `Party.entries.body.entries.caller` | { `type`: `string` = 'TokenId' } |
| `Party.entries.body.entries.caller.type` | `string` |
| `Party.entries.body.entries.events` | { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Party.entries.body.entries.events.checkedType` | { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.events.checkedType.docEntries` | { `data`: ``null`` = null; `hash`: ``null`` = null } |
| `Party.entries.body.entries.events.checkedType.docEntries.data` | ``null`` |
| `Party.entries.body.entries.events.checkedType.docEntries.hash` | ``null`` |
| `Party.entries.body.entries.events.checkedType.docs` | ``null`` |
| `Party.entries.body.entries.events.checkedType.entries` | { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } |
| `Party.entries.body.entries.events.checkedType.entries.data` | { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Party.entries.body.entries.events.checkedType.entries.data.inner` | { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Party.entries.body.entries.events.checkedType.entries.data.inner.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.events.checkedType.entries.data.inner.inner.type` | `string` |
| `Party.entries.body.entries.events.checkedType.entries.data.inner.staticLength` | ``null`` |
| `Party.entries.body.entries.events.checkedType.entries.data.inner.type` | `string` |
| `Party.entries.body.entries.events.checkedType.entries.data.staticLength` | ``null`` |
| `Party.entries.body.entries.events.checkedType.entries.data.type` | `string` |
| `Party.entries.body.entries.events.checkedType.entries.hash` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.events.checkedType.entries.hash.type` | `string` |
| `Party.entries.body.entries.events.checkedType.keys` | `string`[] |
| `Party.entries.body.entries.events.checkedType.name` | `string` |
| `Party.entries.body.entries.events.checkedType.type` | `string` |
| `Party.entries.body.entries.events.checkedTypeName` | `string` |
| `Party.entries.body.entries.events.inner` | { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Party.entries.body.entries.events.inner.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.events.inner.inner.type` | `string` |
| `Party.entries.body.entries.events.inner.staticLength` | ``null`` |
| `Party.entries.body.entries.events.inner.type` | `string` |
| `Party.entries.body.entries.events.staticLength` | ``null`` |
| `Party.entries.body.entries.events.type` | `string` |
| `Party.entries.body.entries.incrementNonce` | { `type`: `string` = 'Bool' } |
| `Party.entries.body.entries.incrementNonce.type` | `string` |
| `Party.entries.body.entries.preconditions` | { `docEntries`: { `account`: ``null`` = null; `network`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `account`: { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } ; `network`: { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' }  } ; `keys`: `string`[] ; `name`: `string` = 'Preconditions'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.docEntries` | { `account`: ``null`` = null; `network`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.docEntries.account` | ``null`` |
| `Party.entries.body.entries.preconditions.docEntries.network` | ``null`` |
| `Party.entries.body.entries.preconditions.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries` | { `account`: { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } ; `network`: { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' }  } |
| `Party.entries.body.entries.preconditions.entries.account` | { `docEntries`: { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } ; `keys`: `string`[] ; `name`: `string` = 'AccountPrecondition'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.account.docEntries` | { `balance`: ``null`` = null; `delegate`: ``null`` = null; `isNew`: ``null`` = null; `nonce`: ``null`` = null; `provedState`: ``null`` = null; `receiptChainHash`: ``null`` = null; `sequenceState`: ``null`` = null; `state`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.account.docEntries.balance` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.account.docEntries.delegate` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.account.docEntries.isNew` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.account.docEntries.nonce` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.account.docEntries.provedState` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.account.docEntries.receiptChainHash` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.account.docEntries.sequenceState` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.account.docEntries.state` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.account.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.account.entries` | { `balance`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `isNew`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nonce`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `provedState`: { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `receiptChainHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `sequenceState`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `state`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' }  } |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BalanceInterval'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance.inner.docEntries.lower` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance.inner.docEntries.upper` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance.inner.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance.inner.entries` | { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance.inner.entries.lower` | { `type`: `string` = 'UInt64' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance.inner.entries.lower.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance.inner.entries.upper` | { `type`: `string` = 'UInt64' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance.inner.entries.upper.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance.inner.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance.inner.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.balance.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.delegate` | { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.delegate.inner` | { `type`: `string` = 'PublicKey' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.delegate.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.delegate.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.delegate.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.isNew` | { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.isNew.inner` | { `type`: `string` = 'Bool' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.isNew.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.isNew.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.isNew.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'NonceInterval'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce.inner.docEntries.lower` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce.inner.docEntries.upper` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce.inner.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce.inner.entries` | { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce.inner.entries.lower` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce.inner.entries.lower.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce.inner.entries.upper` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce.inner.entries.upper.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce.inner.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce.inner.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.nonce.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.provedState` | { `inner`: { `type`: `string` = 'Bool' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.provedState.inner` | { `type`: `string` = 'Bool' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.provedState.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.provedState.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.provedState.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.receiptChainHash` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.receiptChainHash.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.receiptChainHash.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.receiptChainHash.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.receiptChainHash.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.sequenceState` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.sequenceState.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.sequenceState.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.sequenceState.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.sequenceState.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.state` | { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.state.inner` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.state.inner.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.preconditions.entries.account.entries.state.inner.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.state.inner.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.state.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.entries.state.staticLength` | `number` |
| `Party.entries.body.entries.preconditions.entries.account.entries.state.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.account.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.account.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network` | { `docEntries`: { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'NetworkPrecondition'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.network.docEntries` | { `blockchainLength`: ``null`` = null; `globalSlotSinceGenesis`: ``null`` = null; `globalSlotSinceHardFork`: ``null`` = null; `minWindowDensity`: ``null`` = null; `nextEpochData`: ``null`` = null; `snarkedLedgerHash`: ``null`` = null; `stakingEpochData`: ``null`` = null; `timestamp`: ``null`` = null; `totalCurrency`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.network.docEntries.blockchainLength` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.docEntries.globalSlotSinceGenesis` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.docEntries.globalSlotSinceHardFork` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.docEntries.minWindowDensity` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.docEntries.nextEpochData` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.docEntries.snarkedLedgerHash` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.docEntries.stakingEpochData` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.docEntries.timestamp` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.docEntries.totalCurrency` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries` | { `blockchainLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceGenesis`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `globalSlotSinceHardFork`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `minWindowDensity`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `nextEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `snarkedLedgerHash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `stakingEpochData`: { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } ; `timestamp`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.docEntries.lower` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.docEntries.upper` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.entries` | { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.entries.lower` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.entries.lower.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.entries.upper` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.entries.upper.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.blockchainLength.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.docEntries.lower` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.docEntries.upper` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.entries` | { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.entries.lower` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.entries.lower.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.entries.upper` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.entries.upper.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceGenesis.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'GlobalSlotInterval'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.docEntries.lower` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.docEntries.upper` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.entries` | { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.entries.lower` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.entries.lower.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.entries.upper` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.entries.upper.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.globalSlotSinceHardFork.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.docEntries.lower` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.docEntries.upper` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.entries` | { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.entries.lower` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.entries.lower.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.entries.upper` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.entries.upper.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.minWindowDensity.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData` | { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.docEntries` | { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.docEntries.epochLength` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.docEntries.ledger` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.docEntries.lockCheckpoint` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.docEntries.seed` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.docEntries.startCheckpoint` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries` | { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.docEntries.lower` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.docEntries.upper` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.entries` | { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.entries.lower` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.entries.lower.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.entries.upper` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.entries.upper.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.epochLength.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger` | { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.docEntries` | { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.docEntries.hash` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.docEntries.totalCurrency` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries` | { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.hash` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.hash.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.hash.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.hash.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.hash.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.docEntries.lower` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.docEntries.upper` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.entries` | { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.entries.lower` | { `type`: `string` = 'UInt64' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.entries.lower.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.entries.upper` | { `type`: `string` = 'UInt64' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.entries.upper.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.entries.totalCurrency.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.ledger.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.lockCheckpoint` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.lockCheckpoint.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.lockCheckpoint.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.lockCheckpoint.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.lockCheckpoint.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.seed` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.seed.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.seed.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.seed.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.seed.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.startCheckpoint` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.startCheckpoint.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.startCheckpoint.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.startCheckpoint.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.entries.startCheckpoint.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.nextEpochData.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.snarkedLedgerHash` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.snarkedLedgerHash.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.snarkedLedgerHash.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.snarkedLedgerHash.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.snarkedLedgerHash.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData` | { `docEntries`: { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochDataPrecondition'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.docEntries` | { `epochLength`: ``null`` = null; `ledger`: ``null`` = null; `lockCheckpoint`: ``null`` = null; `seed`: ``null`` = null; `startCheckpoint`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.docEntries.epochLength` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.docEntries.ledger` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.docEntries.lockCheckpoint` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.docEntries.seed` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.docEntries.startCheckpoint` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries` | { `epochLength`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `ledger`: { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } ; `lockCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `seed`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `startCheckpoint`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'LengthInterval'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.docEntries.lower` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.docEntries.upper` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.entries` | { `lower`: { `type`: `string` = 'UInt32' } ; `upper`: { `type`: `string` = 'UInt32' }  } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.entries.lower` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.entries.lower.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.entries.upper` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.entries.upper.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.epochLength.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger` | { `docEntries`: { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'EpochLedgerPrecondition'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.docEntries` | { `hash`: ``null`` = null; `totalCurrency`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.docEntries.hash` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.docEntries.totalCurrency` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries` | { `hash`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `totalCurrency`: { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.hash` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.hash.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.hash.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.hash.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.hash.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.docEntries.lower` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.docEntries.upper` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.entries` | { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.entries.lower` | { `type`: `string` = 'UInt64' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.entries.lower.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.entries.upper` | { `type`: `string` = 'UInt64' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.entries.upper.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.entries.totalCurrency.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.ledger.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.lockCheckpoint` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.lockCheckpoint.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.lockCheckpoint.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.lockCheckpoint.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.lockCheckpoint.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.seed` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.seed.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.seed.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.seed.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.seed.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.startCheckpoint` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.startCheckpoint.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.startCheckpoint.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.startCheckpoint.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.entries.startCheckpoint.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.stakingEpochData.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'BlockTimeInterval'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.docEntries.lower` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.docEntries.upper` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.entries` | { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.entries.lower` | { `type`: `string` = 'UInt64' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.entries.lower.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.entries.upper` | { `type`: `string` = 'UInt64' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.entries.upper.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.timestamp.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency` | { `inner`: { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner` | { `docEntries`: { `lower`: ``null`` = null; `upper`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } ; `keys`: `string`[] ; `name`: `string` = 'CurrencyAmountInterval'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.docEntries` | { `lower`: ``null`` = null; `upper`: ``null`` = null } |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.docEntries.lower` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.docEntries.upper` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.docs` | ``null`` |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.entries` | { `lower`: { `type`: `string` = 'UInt64' } ; `upper`: { `type`: `string` = 'UInt64' }  } |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.entries.lower` | { `type`: `string` = 'UInt64' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.entries.lower.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.entries.upper` | { `type`: `string` = 'UInt64' } |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.entries.upper.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency.inner.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency.optionType` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.entries.totalCurrency.type` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.entries.network.name` | `string` |
| `Party.entries.body.entries.preconditions.entries.network.type` | `string` |
| `Party.entries.body.entries.preconditions.keys` | `string`[] |
| `Party.entries.body.entries.preconditions.name` | `string` |
| `Party.entries.body.entries.preconditions.type` | `string` |
| `Party.entries.body.entries.publicKey` | { `type`: `string` = 'PublicKey' } |
| `Party.entries.body.entries.publicKey.type` | `string` |
| `Party.entries.body.entries.sequenceEvents` | { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'Events'; `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Party.entries.body.entries.sequenceEvents.checkedType` | { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.sequenceEvents.checkedType.docEntries` | { `data`: ``null`` = null; `hash`: ``null`` = null } |
| `Party.entries.body.entries.sequenceEvents.checkedType.docEntries.data` | ``null`` |
| `Party.entries.body.entries.sequenceEvents.checkedType.docEntries.hash` | ``null`` |
| `Party.entries.body.entries.sequenceEvents.checkedType.docs` | ``null`` |
| `Party.entries.body.entries.sequenceEvents.checkedType.entries` | { `data`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `hash`: { `type`: `string` = 'Field' }  } |
| `Party.entries.body.entries.sequenceEvents.checkedType.entries.data` | { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Party.entries.body.entries.sequenceEvents.checkedType.entries.data.inner` | { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Party.entries.body.entries.sequenceEvents.checkedType.entries.data.inner.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.sequenceEvents.checkedType.entries.data.inner.inner.type` | `string` |
| `Party.entries.body.entries.sequenceEvents.checkedType.entries.data.inner.staticLength` | ``null`` |
| `Party.entries.body.entries.sequenceEvents.checkedType.entries.data.inner.type` | `string` |
| `Party.entries.body.entries.sequenceEvents.checkedType.entries.data.staticLength` | ``null`` |
| `Party.entries.body.entries.sequenceEvents.checkedType.entries.data.type` | `string` |
| `Party.entries.body.entries.sequenceEvents.checkedType.entries.hash` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.sequenceEvents.checkedType.entries.hash.type` | `string` |
| `Party.entries.body.entries.sequenceEvents.checkedType.keys` | `string`[] |
| `Party.entries.body.entries.sequenceEvents.checkedType.name` | `string` |
| `Party.entries.body.entries.sequenceEvents.checkedType.type` | `string` |
| `Party.entries.body.entries.sequenceEvents.checkedTypeName` | `string` |
| `Party.entries.body.entries.sequenceEvents.inner` | { `inner`: { `type`: `string` = 'Field' } ; `staticLength`: ``null`` = null; `type`: `string` = 'array' } |
| `Party.entries.body.entries.sequenceEvents.inner.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.sequenceEvents.inner.inner.type` | `string` |
| `Party.entries.body.entries.sequenceEvents.inner.staticLength` | ``null`` |
| `Party.entries.body.entries.sequenceEvents.inner.type` | `string` |
| `Party.entries.body.entries.sequenceEvents.staticLength` | ``null`` |
| `Party.entries.body.entries.sequenceEvents.type` | `string` |
| `Party.entries.body.entries.tokenId` | { `type`: `string` = 'TokenId' } |
| `Party.entries.body.entries.tokenId.type` | `string` |
| `Party.entries.body.entries.update` | { `docEntries`: { `appState`: ``null`` = null; `delegate`: ``null`` = null; `permissions`: ``null`` = null; `timing`: ``null`` = null; `tokenSymbol`: ``null`` = null; `verificationKey`: ``null`` = null; `votingFor`: ``null`` = null; `zkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `appState`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `permissions`: { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `timing`: { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `tokenSymbol`: { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `verificationKey`: { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `votingFor`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `zkappUri`: { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } ; `keys`: `string`[] ; `name`: `string` = 'PartyUpdate'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.update.docEntries` | { `appState`: ``null`` = null; `delegate`: ``null`` = null; `permissions`: ``null`` = null; `timing`: ``null`` = null; `tokenSymbol`: ``null`` = null; `verificationKey`: ``null`` = null; `votingFor`: ``null`` = null; `zkappUri`: ``null`` = null } |
| `Party.entries.body.entries.update.docEntries.appState` | ``null`` |
| `Party.entries.body.entries.update.docEntries.delegate` | ``null`` |
| `Party.entries.body.entries.update.docEntries.permissions` | ``null`` |
| `Party.entries.body.entries.update.docEntries.timing` | ``null`` |
| `Party.entries.body.entries.update.docEntries.tokenSymbol` | ``null`` |
| `Party.entries.body.entries.update.docEntries.verificationKey` | ``null`` |
| `Party.entries.body.entries.update.docEntries.votingFor` | ``null`` |
| `Party.entries.body.entries.update.docEntries.zkappUri` | ``null`` |
| `Party.entries.body.entries.update.docs` | ``null`` |
| `Party.entries.body.entries.update.entries` | { `appState`: { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } ; `delegate`: { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `permissions`: { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `timing`: { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `tokenSymbol`: { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `verificationKey`: { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `votingFor`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `zkappUri`: { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' }  } |
| `Party.entries.body.entries.update.entries.appState` | { `inner`: { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } ; `staticLength`: `number` = 8; `type`: `string` = 'array' } |
| `Party.entries.body.entries.update.entries.appState.inner` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.update.entries.appState.inner.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.update.entries.appState.inner.inner.type` | `string` |
| `Party.entries.body.entries.update.entries.appState.inner.optionType` | `string` |
| `Party.entries.body.entries.update.entries.appState.inner.type` | `string` |
| `Party.entries.body.entries.update.entries.appState.staticLength` | `number` |
| `Party.entries.body.entries.update.entries.appState.type` | `string` |
| `Party.entries.body.entries.update.entries.delegate` | { `inner`: { `type`: `string` = 'PublicKey' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.update.entries.delegate.inner` | { `type`: `string` = 'PublicKey' } |
| `Party.entries.body.entries.update.entries.delegate.inner.type` | `string` |
| `Party.entries.body.entries.update.entries.delegate.optionType` | `string` |
| `Party.entries.body.entries.update.entries.delegate.type` | `string` |
| `Party.entries.body.entries.update.entries.permissions` | { `inner`: { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.update.entries.permissions.inner` | { `docEntries`: { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } ; `keys`: `string`[] ; `name`: `string` = 'Permissions'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.update.entries.permissions.inner.docEntries` | { `editSequenceState`: ``null`` = null; `editState`: ``null`` = null; `incrementNonce`: ``null`` = null; `receive`: ``null`` = null; `send`: ``null`` = null; `setDelegate`: ``null`` = null; `setPermissions`: ``null`` = null; `setTokenSymbol`: ``null`` = null; `setVerificationKey`: ``null`` = null; `setVotingFor`: ``null`` = null; `setZkappUri`: ``null`` = null } |
| `Party.entries.body.entries.update.entries.permissions.inner.docEntries.editSequenceState` | ``null`` |
| `Party.entries.body.entries.update.entries.permissions.inner.docEntries.editState` | ``null`` |
| `Party.entries.body.entries.update.entries.permissions.inner.docEntries.incrementNonce` | ``null`` |
| `Party.entries.body.entries.update.entries.permissions.inner.docEntries.receive` | ``null`` |
| `Party.entries.body.entries.update.entries.permissions.inner.docEntries.send` | ``null`` |
| `Party.entries.body.entries.update.entries.permissions.inner.docEntries.setDelegate` | ``null`` |
| `Party.entries.body.entries.update.entries.permissions.inner.docEntries.setPermissions` | ``null`` |
| `Party.entries.body.entries.update.entries.permissions.inner.docEntries.setTokenSymbol` | ``null`` |
| `Party.entries.body.entries.update.entries.permissions.inner.docEntries.setVerificationKey` | ``null`` |
| `Party.entries.body.entries.update.entries.permissions.inner.docEntries.setVotingFor` | ``null`` |
| `Party.entries.body.entries.update.entries.permissions.inner.docEntries.setZkappUri` | ``null`` |
| `Party.entries.body.entries.update.entries.permissions.inner.docs` | ``null`` |
| `Party.entries.body.entries.update.entries.permissions.inner.entries` | { `editSequenceState`: { `type`: `string` = 'AuthRequired' } ; `editState`: { `type`: `string` = 'AuthRequired' } ; `incrementNonce`: { `type`: `string` = 'AuthRequired' } ; `receive`: { `type`: `string` = 'AuthRequired' } ; `send`: { `type`: `string` = 'AuthRequired' } ; `setDelegate`: { `type`: `string` = 'AuthRequired' } ; `setPermissions`: { `type`: `string` = 'AuthRequired' } ; `setTokenSymbol`: { `type`: `string` = 'AuthRequired' } ; `setVerificationKey`: { `type`: `string` = 'AuthRequired' } ; `setVotingFor`: { `type`: `string` = 'AuthRequired' } ; `setZkappUri`: { `type`: `string` = 'AuthRequired' }  } |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.editSequenceState` | { `type`: `string` = 'AuthRequired' } |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.editSequenceState.type` | `string` |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.editState` | { `type`: `string` = 'AuthRequired' } |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.editState.type` | `string` |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.incrementNonce` | { `type`: `string` = 'AuthRequired' } |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.incrementNonce.type` | `string` |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.receive` | { `type`: `string` = 'AuthRequired' } |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.receive.type` | `string` |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.send` | { `type`: `string` = 'AuthRequired' } |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.send.type` | `string` |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.setDelegate` | { `type`: `string` = 'AuthRequired' } |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.setDelegate.type` | `string` |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.setPermissions` | { `type`: `string` = 'AuthRequired' } |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.setPermissions.type` | `string` |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.setTokenSymbol` | { `type`: `string` = 'AuthRequired' } |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.setTokenSymbol.type` | `string` |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.setVerificationKey` | { `type`: `string` = 'AuthRequired' } |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.setVerificationKey.type` | `string` |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.setVotingFor` | { `type`: `string` = 'AuthRequired' } |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.setVotingFor.type` | `string` |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.setZkappUri` | { `type`: `string` = 'AuthRequired' } |
| `Party.entries.body.entries.update.entries.permissions.inner.entries.setZkappUri.type` | `string` |
| `Party.entries.body.entries.update.entries.permissions.inner.keys` | `string`[] |
| `Party.entries.body.entries.update.entries.permissions.inner.name` | `string` |
| `Party.entries.body.entries.update.entries.permissions.inner.type` | `string` |
| `Party.entries.body.entries.update.entries.permissions.optionType` | `string` |
| `Party.entries.body.entries.update.entries.permissions.type` | `string` |
| `Party.entries.body.entries.update.entries.timing` | { `inner`: { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.update.entries.timing.inner` | { `docEntries`: { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } ; `keys`: `string`[] ; `name`: `string` = 'Timing'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.update.entries.timing.inner.docEntries` | { `cliffAmount`: ``null`` = null; `cliffTime`: ``null`` = null; `initialMinimumBalance`: ``null`` = null; `vestingIncrement`: ``null`` = null; `vestingPeriod`: ``null`` = null } |
| `Party.entries.body.entries.update.entries.timing.inner.docEntries.cliffAmount` | ``null`` |
| `Party.entries.body.entries.update.entries.timing.inner.docEntries.cliffTime` | ``null`` |
| `Party.entries.body.entries.update.entries.timing.inner.docEntries.initialMinimumBalance` | ``null`` |
| `Party.entries.body.entries.update.entries.timing.inner.docEntries.vestingIncrement` | ``null`` |
| `Party.entries.body.entries.update.entries.timing.inner.docEntries.vestingPeriod` | ``null`` |
| `Party.entries.body.entries.update.entries.timing.inner.docs` | ``null`` |
| `Party.entries.body.entries.update.entries.timing.inner.entries` | { `cliffAmount`: { `type`: `string` = 'UInt64' } ; `cliffTime`: { `type`: `string` = 'UInt32' } ; `initialMinimumBalance`: { `type`: `string` = 'UInt64' } ; `vestingIncrement`: { `type`: `string` = 'UInt64' } ; `vestingPeriod`: { `type`: `string` = 'UInt32' }  } |
| `Party.entries.body.entries.update.entries.timing.inner.entries.cliffAmount` | { `type`: `string` = 'UInt64' } |
| `Party.entries.body.entries.update.entries.timing.inner.entries.cliffAmount.type` | `string` |
| `Party.entries.body.entries.update.entries.timing.inner.entries.cliffTime` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.update.entries.timing.inner.entries.cliffTime.type` | `string` |
| `Party.entries.body.entries.update.entries.timing.inner.entries.initialMinimumBalance` | { `type`: `string` = 'UInt64' } |
| `Party.entries.body.entries.update.entries.timing.inner.entries.initialMinimumBalance.type` | `string` |
| `Party.entries.body.entries.update.entries.timing.inner.entries.vestingIncrement` | { `type`: `string` = 'UInt64' } |
| `Party.entries.body.entries.update.entries.timing.inner.entries.vestingIncrement.type` | `string` |
| `Party.entries.body.entries.update.entries.timing.inner.entries.vestingPeriod` | { `type`: `string` = 'UInt32' } |
| `Party.entries.body.entries.update.entries.timing.inner.entries.vestingPeriod.type` | `string` |
| `Party.entries.body.entries.update.entries.timing.inner.keys` | `string`[] |
| `Party.entries.body.entries.update.entries.timing.inner.name` | `string` |
| `Party.entries.body.entries.update.entries.timing.inner.type` | `string` |
| `Party.entries.body.entries.update.entries.timing.optionType` | `string` |
| `Party.entries.body.entries.update.entries.timing.type` | `string` |
| `Party.entries.body.entries.update.entries.tokenSymbol` | { `inner`: { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.update.entries.tokenSymbol.inner` | { `checkedType`: { `type`: `string` = 'TokenSymbol' } ; `checkedTypeName`: `string` = 'TokenSymbol'; `type`: `string` = 'string' } |
| `Party.entries.body.entries.update.entries.tokenSymbol.inner.checkedType` | { `type`: `string` = 'TokenSymbol' } |
| `Party.entries.body.entries.update.entries.tokenSymbol.inner.checkedType.type` | `string` |
| `Party.entries.body.entries.update.entries.tokenSymbol.inner.checkedTypeName` | `string` |
| `Party.entries.body.entries.update.entries.tokenSymbol.inner.type` | `string` |
| `Party.entries.body.entries.update.entries.tokenSymbol.optionType` | `string` |
| `Party.entries.body.entries.update.entries.tokenSymbol.type` | `string` |
| `Party.entries.body.entries.update.entries.verificationKey` | { `inner`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.update.entries.verificationKey.inner` | { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'VerificationKeyWithHash'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.update.entries.verificationKey.inner.docEntries` | { `data`: ``null`` = null; `hash`: ``null`` = null } |
| `Party.entries.body.entries.update.entries.verificationKey.inner.docEntries.data` | ``null`` |
| `Party.entries.body.entries.update.entries.verificationKey.inner.docEntries.hash` | ``null`` |
| `Party.entries.body.entries.update.entries.verificationKey.inner.docs` | ``null`` |
| `Party.entries.body.entries.update.entries.verificationKey.inner.entries` | { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } |
| `Party.entries.body.entries.update.entries.verificationKey.inner.entries.data` | { `type`: `string` = 'string' } |
| `Party.entries.body.entries.update.entries.verificationKey.inner.entries.data.type` | `string` |
| `Party.entries.body.entries.update.entries.verificationKey.inner.entries.hash` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.update.entries.verificationKey.inner.entries.hash.type` | `string` |
| `Party.entries.body.entries.update.entries.verificationKey.inner.keys` | `string`[] |
| `Party.entries.body.entries.update.entries.verificationKey.inner.name` | `string` |
| `Party.entries.body.entries.update.entries.verificationKey.inner.type` | `string` |
| `Party.entries.body.entries.update.entries.verificationKey.optionType` | `string` |
| `Party.entries.body.entries.update.entries.verificationKey.type` | `string` |
| `Party.entries.body.entries.update.entries.votingFor` | { `inner`: { `type`: `string` = 'Field' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.update.entries.votingFor.inner` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.update.entries.votingFor.inner.type` | `string` |
| `Party.entries.body.entries.update.entries.votingFor.optionType` | `string` |
| `Party.entries.body.entries.update.entries.votingFor.type` | `string` |
| `Party.entries.body.entries.update.entries.zkappUri` | { `inner`: { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } ; `optionType`: `string` = 'flaggedOption'; `type`: `string` = 'option' } |
| `Party.entries.body.entries.update.entries.zkappUri.inner` | { `checkedType`: { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } ; `checkedTypeName`: `string` = 'StringWithHash'; `type`: `string` = 'string' } |
| `Party.entries.body.entries.update.entries.zkappUri.inner.checkedType` | { `docEntries`: { `data`: ``null`` = null; `hash`: ``null`` = null } ; `docs`: ``null`` = null; `entries`: { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } ; `keys`: `string`[] ; `name`: `string` = 'Events'; `type`: `string` = 'object' } |
| `Party.entries.body.entries.update.entries.zkappUri.inner.checkedType.docEntries` | { `data`: ``null`` = null; `hash`: ``null`` = null } |
| `Party.entries.body.entries.update.entries.zkappUri.inner.checkedType.docEntries.data` | ``null`` |
| `Party.entries.body.entries.update.entries.zkappUri.inner.checkedType.docEntries.hash` | ``null`` |
| `Party.entries.body.entries.update.entries.zkappUri.inner.checkedType.docs` | ``null`` |
| `Party.entries.body.entries.update.entries.zkappUri.inner.checkedType.entries` | { `data`: { `type`: `string` = 'string' } ; `hash`: { `type`: `string` = 'Field' }  } |
| `Party.entries.body.entries.update.entries.zkappUri.inner.checkedType.entries.data` | { `type`: `string` = 'string' } |
| `Party.entries.body.entries.update.entries.zkappUri.inner.checkedType.entries.data.type` | `string` |
| `Party.entries.body.entries.update.entries.zkappUri.inner.checkedType.entries.hash` | { `type`: `string` = 'Field' } |
| `Party.entries.body.entries.update.entries.zkappUri.inner.checkedType.entries.hash.type` | `string` |
| `Party.entries.body.entries.update.entries.zkappUri.inner.checkedType.keys` | `string`[] |
| `Party.entries.body.entries.update.entries.zkappUri.inner.checkedType.name` | `string` |
| `Party.entries.body.entries.update.entries.zkappUri.inner.checkedType.type` | `string` |
| `Party.entries.body.entries.update.entries.zkappUri.inner.checkedTypeName` | `string` |
| `Party.entries.body.entries.update.entries.zkappUri.inner.type` | `string` |
| `Party.entries.body.entries.update.entries.zkappUri.optionType` | `string` |
| `Party.entries.body.entries.update.entries.zkappUri.type` | `string` |
| `Party.entries.body.entries.update.keys` | `string`[] |
| `Party.entries.body.entries.update.name` | `string` |
| `Party.entries.body.entries.update.type` | `string` |
| `Party.entries.body.entries.useFullCommitment` | { `type`: `string` = 'Bool' } |
| `Party.entries.body.entries.useFullCommitment.type` | `string` |
| `Party.entries.body.keys` | `string`[] |
| `Party.entries.body.name` | `string` |
| `Party.entries.body.type` | `string` |
| `Party.keys` | `string`[] |
| `Party.name` | `string` |
| `Party.type` | `string` |

##### Defined in

[index.ts:88](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/index.ts#L88)

### Functions

#### MerkleWitness

▸ **MerkleWitness**(`height`): typeof `BaseMerkleWitness`

##### Parameters

| Name | Type |
| :------ | :------ |
| `height` | `number` |

##### Returns

typeof `BaseMerkleWitness`

##### Defined in

[index.ts:92](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/index.ts#L92)

___

#### asFieldsAndAux

▸ **asFieldsAndAux**<`T`, `JsonT`\>(`layout`): `Object`

##### Type parameters

| Name |
| :------ |
| `T` |
| `JsonT` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `layout` | `any` |

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `check` | (`value`: `T`) => `void` |
| `fromFields` | (`fields`: [`Field`](#classesfieldmd)[], `aux`: `any`[]) => `T` |
| `sizeInFields` | () => `number` |
| `toAuxiliary` | (`value?`: `T`) => `any`[] |
| `toFields` | (`value`: `T`) => [`Field`](#classesfieldmd)[] |
| `toInput` | (`value`: `T`) => `HashInput` |
| `toJSON` | (`value`: `T`) => `JsonT` |
| `witness` | (`f`: () => `T`) => `T` |

##### Defined in

[index.ts:89](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/index.ts#L89)

___

#### createChildParty

▸ **createChildParty**(`parent`, `childAddress`, `options?`): [`Party`](#classespartymd)

##### Parameters

| Name | Type |
| :------ | :------ |
| `parent` | [`Party`](#classespartymd) |
| `childAddress` | [`PublicKey`](#classestypespublickeymd) |
| `options?` | `Object` |
| `options.caller?` | [`Field`](#classesfieldmd) |
| `options.tokenId?` | [`Field`](#classesfieldmd) |
| `options.useFullCommitment?` | [`Bool`](#classesboolmd) |

##### Returns

[`Party`](#classespartymd)

##### Defined in

[index.ts:86](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/index.ts#L86)

___

#### memoizeWitness

▸ **memoizeWitness**<`T`\>(`type`, `compute`): `T`

##### Type parameters

| Name |
| :------ |
| `T` |

##### Parameters

| Name | Type |
| :------ | :------ |
| `type` | [`AsFieldElements`](#interfacesasfieldelementsmd)<`T`\> |
| `compute` | () => `T` |

##### Returns

`T`

##### Defined in

[index.ts:87](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/index.ts#L87)

___

#### packToFields

▸ **packToFields**(`__namedParameters`): [`Field`](#classesfieldmd)[]

##### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | `HashInput` |

##### Returns

[`Field`](#classesfieldmd)[]

##### Defined in

[index.ts:90](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/index.ts#L90)


<a name="modulesminamd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Mina

## Namespace: Mina

### Table of contents

#### Type Aliases

- [CurrentTransaction](#currenttransaction)
- [FeePayerSpec](#feepayerspec)

#### Variables

- [currentTransaction](#currenttransaction-1)

#### Functions

- [BerkeleyQANet](#berkeleyqanet)
- [LocalBlockchain](#localblockchain)
- [accountCreationFee](#accountcreationfee)
- [createTransaction](#createtransaction)
- [currentSlot](#currentslot)
- [fetchEvents](#fetchevents)
- [getAccount](#getaccount)
- [getBalance](#getbalance)
- [getNetworkState](#getnetworkstate)
- [hasAccount](#hasaccount)
- [sendTransaction](#sendtransaction)
- [setActiveInstance](#setactiveinstance)
- [transaction](#transaction)

### Type Aliases

#### CurrentTransaction

Ƭ **CurrentTransaction**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `fetchMode` | `FetchMode` |
| `isFinalRunOutsideCircuit` | `boolean` |
| `parties` | [`Party`](#classespartymd)[] |
| `sender?` | [`PrivateKey`](#classesprivatekeymd) |

##### Defined in

[lib/mina.ts:62](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L62)

___

#### FeePayerSpec

Ƭ **FeePayerSpec**: [`PrivateKey`](#classesprivatekeymd) \| { `fee?`: `number` \| `string` \| [`UInt64`](#classesuint64md) ; `feePayerKey`: [`PrivateKey`](#classesprivatekeymd) ; `memo?`: `string`  } \| `undefined`

##### Defined in

[lib/mina.ts:71](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L71)

### Variables

#### currentTransaction

• **currentTransaction**: `t`<[`CurrentTransaction`](#currenttransaction)\>

##### Defined in

[lib/mina.ts:69](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L69)

### Functions

#### BerkeleyQANet

▸ **BerkeleyQANet**(`graphqlEndpoint`): `Mina`

##### Parameters

| Name | Type |
| :------ | :------ |
| `graphqlEndpoint` | `string` |

##### Returns

`Mina`

##### Defined in

[lib/mina.ts:483](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L483)

___

#### LocalBlockchain

▸ **LocalBlockchain**(`__namedParameters?`): `MockMina`

A mock Mina blockchain running locally and useful for testing.

##### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | `Object` |
| `__namedParameters.accountCreationFee` | `undefined` \| `string` \| `number` |

##### Returns

`MockMina`

##### Defined in

[lib/mina.ts:222](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L222)

___

#### accountCreationFee

▸ **accountCreationFee**(): [`UInt64`](#classesuint64md)

##### Returns

[`UInt64`](#classesuint64md)

##### Defined in

[lib/mina.ts:618](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L618)

___

#### createTransaction

▸ **createTransaction**(`feePayer`, `f`, `__namedParameters?`): `Transaction`

##### Parameters

| Name | Type |
| :------ | :------ |
| `feePayer` | [`FeePayerSpec`](#feepayerspec) |
| `f` | () => `unknown` |
| `__namedParameters` | `Object` |
| `__namedParameters.fetchMode` | `undefined` \| `FetchMode` |
| `__namedParameters.isFinalRunOutsideCircuit` | `undefined` \| `boolean` |

##### Returns

`Transaction`

##### Defined in

[lib/mina.ts:84](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L84)

___

#### currentSlot

▸ **currentSlot**(): [`UInt32`](#classesuint32md)

##### Returns

[`UInt32`](#classesuint32md)

The current slot number, according to the active Mina instance.

##### Defined in

[lib/mina.ts:589](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L589)

___

#### fetchEvents

▸ **fetchEvents**(`publicKey`, `tokenId`): `Promise`<`any`\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | [`PublicKey`](#classestypespublickeymd) |
| `tokenId` | [`Field`](#classesfieldmd) |

##### Returns

`Promise`<`any`\>

A list of emitted events associated to the given public key.

##### Defined in

[lib/mina.ts:629](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L629)

___

#### getAccount

▸ **getAccount**(`publicKey`, `tokenId?`): `Account`

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | [`PublicKey`](#classestypespublickeymd) |
| `tokenId?` | [`Field`](#classesfieldmd) |

##### Returns

`Account`

The account data associated to the given public key.

##### Defined in

[lib/mina.ts:596](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L596)

___

#### getBalance

▸ **getBalance**(`publicKey`, `tokenId?`): [`UInt64`](#classesuint64md)

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | [`PublicKey`](#classestypespublickeymd) |
| `tokenId?` | [`Field`](#classesfieldmd) |

##### Returns

[`UInt64`](#classesuint64md)

The balance associated to the given public key.

##### Defined in

[lib/mina.ts:614](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L614)

___

#### getNetworkState

▸ **getNetworkState**(): `PreconditionBaseTypes`<{ `blockchainLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceGenesis`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceHardFork`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `minWindowDensity`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `nextEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `snarkedLedgerHash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `stakingEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `timestamp`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  }\>

##### Returns

`PreconditionBaseTypes`<{ `blockchainLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceGenesis`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceHardFork`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `minWindowDensity`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `nextEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `snarkedLedgerHash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `stakingEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `timestamp`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  }\>

Data associated with the current state of the Mina network.

##### Defined in

[lib/mina.ts:607](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L607)

___

#### hasAccount

▸ **hasAccount**(`publicKey`, `tokenId?`): `boolean`

##### Parameters

| Name | Type |
| :------ | :------ |
| `publicKey` | [`PublicKey`](#classestypespublickeymd) |
| `tokenId?` | [`Field`](#classesfieldmd) |

##### Returns

`boolean`

##### Defined in

[lib/mina.ts:600](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L600)

___

#### sendTransaction

▸ **sendTransaction**(`txn`): `TransactionId`

##### Parameters

| Name | Type |
| :------ | :------ |
| `txn` | `Transaction` |

##### Returns

`TransactionId`

##### Defined in

[lib/mina.ts:622](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L622)

___

#### setActiveInstance

▸ **setActiveInstance**(`m`): `void`

Set the currently used Mina instance.

##### Parameters

| Name | Type |
| :------ | :------ |
| `m` | `Mina` |

##### Returns

`void`

##### Defined in

[lib/mina.ts:551](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L551)

___

#### transaction

▸ **transaction**(`f`): `Promise`<`Transaction`\>

Construct a smart contract transaction. Within the callback passed to this function,
you can call into the methods of smart contracts.

```typescript
transaction(() => {
  myZkapp.update();
  someOtherZkapp.someOtherMethod();
})
```

##### Parameters

| Name | Type |
| :------ | :------ |
| `f` | () => `void` |

##### Returns

`Promise`<`Transaction`\>

A transaction that can subsequently be submitted to the chain.

##### Defined in

[lib/mina.ts:568](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L568)

▸ **transaction**(`sender`, `f`): `Promise`<`Transaction`\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `sender` | [`FeePayerSpec`](#feepayerspec) |
| `f` | () => `void` |

##### Returns

`Promise`<`Transaction`\>

##### Defined in

[lib/mina.ts:569](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/mina.ts#L569)


<a name="modulestypesjsonmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / [Types](#modulestypesmd) / Json

## Namespace: Json

[Types](#modulestypesmd).Json

### Table of contents

#### Type Aliases

- [AuthRequired](#authrequired)
- [Bool](#bool)
- [Field](#field)
- [Parties](#parties)
- [Party](#party)
- [PublicKey](#publickey)
- [Sign](#sign)
- [TokenId](#tokenid)
- [TypeMap](#typemap)
- [UInt32](#uint32)
- [UInt64](#uint64)

### Type Aliases

#### AuthRequired

Ƭ **AuthRequired**: ``"Signature"`` \| ``"Proof"`` \| ``"Either"`` \| ``"None"`` \| ``"Impossible"``

##### Defined in

[snarky/parties-leaves-json.ts:11](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves-json.ts#L11)

___

#### Bool

Ƭ **Bool**: `boolean`

##### Defined in

[snarky/parties-leaves-json.ts:6](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves-json.ts#L6)

___

#### Field

Ƭ **Field**: `string`

##### Defined in

[snarky/parties-leaves-json.ts:5](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves-json.ts#L5)

___

#### Parties

Ƭ **Parties**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `feePayer` | { `authorization`: `string` ; `body`: { `fee`: [`UInt64`](#uint64) ; `nonce`: [`UInt32`](#uint32) ; `publicKey`: [`PublicKey`](#publickey) ; `validUntil`: [`UInt32`](#uint32) \| ``null``  }  } |
| `feePayer.authorization` | `string` |
| `feePayer.body` | { `fee`: [`UInt64`](#uint64) ; `nonce`: [`UInt32`](#uint32) ; `publicKey`: [`PublicKey`](#publickey) ; `validUntil`: [`UInt32`](#uint32) \| ``null``  } |
| `feePayer.body.fee` | [`UInt64`](#uint64) |
| `feePayer.body.nonce` | [`UInt32`](#uint32) |
| `feePayer.body.publicKey` | [`PublicKey`](#publickey) |
| `feePayer.body.validUntil` | [`UInt32`](#uint32) \| ``null`` |
| `memo` | `string` |
| `otherParties` | { `authorization`: { `proof`: `string` \| ``null`` ; `signature`: `string` \| ``null``  } ; `body`: { `balanceChange`: { `magnitude`: [`UInt64`](#uint64) ; `sgn`: [`Sign`](#sign)  } ; `callData`: [`Field`](#field) ; `callDepth`: `number` ; `caller`: [`TokenId`](#tokenid) ; `events`: [`Field`](#field)[][] ; `incrementNonce`: [`Bool`](#bool) ; `preconditions`: { `account`: { `balance`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null`` ; `delegate`: [`PublicKey`](#publickey) \| ``null`` ; `isNew`: [`Bool`](#bool) \| ``null`` ; `nonce`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `provedState`: [`Bool`](#bool) \| ``null`` ; `receiptChainHash`: [`Field`](#field) \| ``null`` ; `sequenceState`: [`Field`](#field) \| ``null`` ; `state`: ([`Field`](#field) \| ``null``)[]  } ; `network`: { `blockchainLength`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `globalSlotSinceGenesis`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `globalSlotSinceHardFork`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `minWindowDensity`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `nextEpochData`: { `epochLength`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `ledger`: { `hash`: [`Field`](#field) \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  } ; `lockCheckpoint`: [`Field`](#field) \| ``null`` ; `seed`: [`Field`](#field) \| ``null`` ; `startCheckpoint`: [`Field`](#field) \| ``null``  } ; `snarkedLedgerHash`: [`Field`](#field) \| ``null`` ; `stakingEpochData`: { `epochLength`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `ledger`: { `hash`: [`Field`](#field) \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  } ; `lockCheckpoint`: [`Field`](#field) \| ``null`` ; `seed`: [`Field`](#field) \| ``null`` ; `startCheckpoint`: [`Field`](#field) \| ``null``  } ; `timestamp`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  }  } ; `publicKey`: [`PublicKey`](#publickey) ; `sequenceEvents`: [`Field`](#field)[][] ; `tokenId`: [`TokenId`](#tokenid) ; `update`: { `appState`: ([`Field`](#field) \| ``null``)[] ; `delegate`: [`PublicKey`](#publickey) \| ``null`` ; `permissions`: { `editSequenceState`: [`AuthRequired`](#authrequired) ; `editState`: [`AuthRequired`](#authrequired) ; `incrementNonce`: [`AuthRequired`](#authrequired) ; `receive`: [`AuthRequired`](#authrequired) ; `send`: [`AuthRequired`](#authrequired) ; `setDelegate`: [`AuthRequired`](#authrequired) ; `setPermissions`: [`AuthRequired`](#authrequired) ; `setTokenSymbol`: [`AuthRequired`](#authrequired) ; `setVerificationKey`: [`AuthRequired`](#authrequired) ; `setVotingFor`: [`AuthRequired`](#authrequired) ; `setZkappUri`: [`AuthRequired`](#authrequired)  } \| ``null`` ; `timing`: { `cliffAmount`: [`UInt64`](#uint64) ; `cliffTime`: [`UInt32`](#uint32) ; `initialMinimumBalance`: [`UInt64`](#uint64) ; `vestingIncrement`: [`UInt64`](#uint64) ; `vestingPeriod`: [`UInt32`](#uint32)  } \| ``null`` ; `tokenSymbol`: `string` \| ``null`` ; `verificationKey`: { `data`: `string` ; `hash`: [`Field`](#field)  } \| ``null`` ; `votingFor`: [`Field`](#field) \| ``null`` ; `zkappUri`: `string` \| ``null``  } ; `useFullCommitment`: [`Bool`](#bool)  }  }[] |

##### Defined in

[snarky/gen/parties-json.ts:17](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/gen/parties-json.ts#L17)

___

#### Party

Ƭ **Party**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `authorization` | { `proof`: `string` \| ``null`` ; `signature`: `string` \| ``null``  } |
| `authorization.proof` | `string` \| ``null`` |
| `authorization.signature` | `string` \| ``null`` |
| `body` | { `balanceChange`: { `magnitude`: [`UInt64`](#uint64) ; `sgn`: [`Sign`](#sign)  } ; `callData`: [`Field`](#field) ; `callDepth`: `number` ; `caller`: [`TokenId`](#tokenid) ; `events`: [`Field`](#field)[][] ; `incrementNonce`: [`Bool`](#bool) ; `preconditions`: { `account`: { `balance`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null`` ; `delegate`: [`PublicKey`](#publickey) \| ``null`` ; `isNew`: [`Bool`](#bool) \| ``null`` ; `nonce`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `provedState`: [`Bool`](#bool) \| ``null`` ; `receiptChainHash`: [`Field`](#field) \| ``null`` ; `sequenceState`: [`Field`](#field) \| ``null`` ; `state`: ([`Field`](#field) \| ``null``)[]  } ; `network`: { `blockchainLength`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `globalSlotSinceGenesis`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `globalSlotSinceHardFork`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `minWindowDensity`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `nextEpochData`: { `epochLength`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `ledger`: { `hash`: [`Field`](#field) \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  } ; `lockCheckpoint`: [`Field`](#field) \| ``null`` ; `seed`: [`Field`](#field) \| ``null`` ; `startCheckpoint`: [`Field`](#field) \| ``null``  } ; `snarkedLedgerHash`: [`Field`](#field) \| ``null`` ; `stakingEpochData`: { `epochLength`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `ledger`: { `hash`: [`Field`](#field) \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  } ; `lockCheckpoint`: [`Field`](#field) \| ``null`` ; `seed`: [`Field`](#field) \| ``null`` ; `startCheckpoint`: [`Field`](#field) \| ``null``  } ; `timestamp`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  }  } ; `publicKey`: [`PublicKey`](#publickey) ; `sequenceEvents`: [`Field`](#field)[][] ; `tokenId`: [`TokenId`](#tokenid) ; `update`: { `appState`: ([`Field`](#field) \| ``null``)[] ; `delegate`: [`PublicKey`](#publickey) \| ``null`` ; `permissions`: { `editSequenceState`: [`AuthRequired`](#authrequired) ; `editState`: [`AuthRequired`](#authrequired) ; `incrementNonce`: [`AuthRequired`](#authrequired) ; `receive`: [`AuthRequired`](#authrequired) ; `send`: [`AuthRequired`](#authrequired) ; `setDelegate`: [`AuthRequired`](#authrequired) ; `setPermissions`: [`AuthRequired`](#authrequired) ; `setTokenSymbol`: [`AuthRequired`](#authrequired) ; `setVerificationKey`: [`AuthRequired`](#authrequired) ; `setVotingFor`: [`AuthRequired`](#authrequired) ; `setZkappUri`: [`AuthRequired`](#authrequired)  } \| ``null`` ; `timing`: { `cliffAmount`: [`UInt64`](#uint64) ; `cliffTime`: [`UInt32`](#uint32) ; `initialMinimumBalance`: [`UInt64`](#uint64) ; `vestingIncrement`: [`UInt64`](#uint64) ; `vestingPeriod`: [`UInt32`](#uint32)  } \| ``null`` ; `tokenSymbol`: `string` \| ``null`` ; `verificationKey`: { `data`: `string` ; `hash`: [`Field`](#field)  } \| ``null`` ; `votingFor`: [`Field`](#field) \| ``null`` ; `zkappUri`: `string` \| ``null``  } ; `useFullCommitment`: [`Bool`](#bool)  } |
| `body.balanceChange` | { `magnitude`: [`UInt64`](#uint64) ; `sgn`: [`Sign`](#sign)  } |
| `body.balanceChange.magnitude` | [`UInt64`](#uint64) |
| `body.balanceChange.sgn` | [`Sign`](#sign) |
| `body.callData` | [`Field`](#field) |
| `body.callDepth` | `number` |
| `body.caller` | [`TokenId`](#tokenid) |
| `body.events` | [`Field`](#field)[][] |
| `body.incrementNonce` | [`Bool`](#bool) |
| `body.preconditions` | { `account`: { `balance`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null`` ; `delegate`: [`PublicKey`](#publickey) \| ``null`` ; `isNew`: [`Bool`](#bool) \| ``null`` ; `nonce`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `provedState`: [`Bool`](#bool) \| ``null`` ; `receiptChainHash`: [`Field`](#field) \| ``null`` ; `sequenceState`: [`Field`](#field) \| ``null`` ; `state`: ([`Field`](#field) \| ``null``)[]  } ; `network`: { `blockchainLength`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `globalSlotSinceGenesis`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `globalSlotSinceHardFork`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `minWindowDensity`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `nextEpochData`: { `epochLength`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `ledger`: { `hash`: [`Field`](#field) \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  } ; `lockCheckpoint`: [`Field`](#field) \| ``null`` ; `seed`: [`Field`](#field) \| ``null`` ; `startCheckpoint`: [`Field`](#field) \| ``null``  } ; `snarkedLedgerHash`: [`Field`](#field) \| ``null`` ; `stakingEpochData`: { `epochLength`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `ledger`: { `hash`: [`Field`](#field) \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  } ; `lockCheckpoint`: [`Field`](#field) \| ``null`` ; `seed`: [`Field`](#field) \| ``null`` ; `startCheckpoint`: [`Field`](#field) \| ``null``  } ; `timestamp`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  }  } |
| `body.preconditions.account` | { `balance`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null`` ; `delegate`: [`PublicKey`](#publickey) \| ``null`` ; `isNew`: [`Bool`](#bool) \| ``null`` ; `nonce`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `provedState`: [`Bool`](#bool) \| ``null`` ; `receiptChainHash`: [`Field`](#field) \| ``null`` ; `sequenceState`: [`Field`](#field) \| ``null`` ; `state`: ([`Field`](#field) \| ``null``)[]  } |
| `body.preconditions.account.balance` | { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null`` |
| `body.preconditions.account.delegate` | [`PublicKey`](#publickey) \| ``null`` |
| `body.preconditions.account.isNew` | [`Bool`](#bool) \| ``null`` |
| `body.preconditions.account.nonce` | { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` |
| `body.preconditions.account.provedState` | [`Bool`](#bool) \| ``null`` |
| `body.preconditions.account.receiptChainHash` | [`Field`](#field) \| ``null`` |
| `body.preconditions.account.sequenceState` | [`Field`](#field) \| ``null`` |
| `body.preconditions.account.state` | ([`Field`](#field) \| ``null``)[] |
| `body.preconditions.network` | { `blockchainLength`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `globalSlotSinceGenesis`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `globalSlotSinceHardFork`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `minWindowDensity`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `nextEpochData`: { `epochLength`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `ledger`: { `hash`: [`Field`](#field) \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  } ; `lockCheckpoint`: [`Field`](#field) \| ``null`` ; `seed`: [`Field`](#field) \| ``null`` ; `startCheckpoint`: [`Field`](#field) \| ``null``  } ; `snarkedLedgerHash`: [`Field`](#field) \| ``null`` ; `stakingEpochData`: { `epochLength`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `ledger`: { `hash`: [`Field`](#field) \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  } ; `lockCheckpoint`: [`Field`](#field) \| ``null`` ; `seed`: [`Field`](#field) \| ``null`` ; `startCheckpoint`: [`Field`](#field) \| ``null``  } ; `timestamp`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  } |
| `body.preconditions.network.blockchainLength` | { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` |
| `body.preconditions.network.globalSlotSinceGenesis` | { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` |
| `body.preconditions.network.globalSlotSinceHardFork` | { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` |
| `body.preconditions.network.minWindowDensity` | { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` |
| `body.preconditions.network.nextEpochData` | { `epochLength`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `ledger`: { `hash`: [`Field`](#field) \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  } ; `lockCheckpoint`: [`Field`](#field) \| ``null`` ; `seed`: [`Field`](#field) \| ``null`` ; `startCheckpoint`: [`Field`](#field) \| ``null``  } |
| `body.preconditions.network.nextEpochData.epochLength` | { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` |
| `body.preconditions.network.nextEpochData.ledger` | { `hash`: [`Field`](#field) \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  } |
| `body.preconditions.network.nextEpochData.ledger.hash` | [`Field`](#field) \| ``null`` |
| `body.preconditions.network.nextEpochData.ledger.totalCurrency` | { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null`` |
| `body.preconditions.network.nextEpochData.lockCheckpoint` | [`Field`](#field) \| ``null`` |
| `body.preconditions.network.nextEpochData.seed` | [`Field`](#field) \| ``null`` |
| `body.preconditions.network.nextEpochData.startCheckpoint` | [`Field`](#field) \| ``null`` |
| `body.preconditions.network.snarkedLedgerHash` | [`Field`](#field) \| ``null`` |
| `body.preconditions.network.stakingEpochData` | { `epochLength`: { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` ; `ledger`: { `hash`: [`Field`](#field) \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  } ; `lockCheckpoint`: [`Field`](#field) \| ``null`` ; `seed`: [`Field`](#field) \| ``null`` ; `startCheckpoint`: [`Field`](#field) \| ``null``  } |
| `body.preconditions.network.stakingEpochData.epochLength` | { `lower`: [`UInt32`](#uint32) ; `upper`: [`UInt32`](#uint32)  } \| ``null`` |
| `body.preconditions.network.stakingEpochData.ledger` | { `hash`: [`Field`](#field) \| ``null`` ; `totalCurrency`: { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null``  } |
| `body.preconditions.network.stakingEpochData.ledger.hash` | [`Field`](#field) \| ``null`` |
| `body.preconditions.network.stakingEpochData.ledger.totalCurrency` | { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null`` |
| `body.preconditions.network.stakingEpochData.lockCheckpoint` | [`Field`](#field) \| ``null`` |
| `body.preconditions.network.stakingEpochData.seed` | [`Field`](#field) \| ``null`` |
| `body.preconditions.network.stakingEpochData.startCheckpoint` | [`Field`](#field) \| ``null`` |
| `body.preconditions.network.timestamp` | { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null`` |
| `body.preconditions.network.totalCurrency` | { `lower`: [`UInt64`](#uint64) ; `upper`: [`UInt64`](#uint64)  } \| ``null`` |
| `body.publicKey` | [`PublicKey`](#publickey) |
| `body.sequenceEvents` | [`Field`](#field)[][] |
| `body.tokenId` | [`TokenId`](#tokenid) |
| `body.update` | { `appState`: ([`Field`](#field) \| ``null``)[] ; `delegate`: [`PublicKey`](#publickey) \| ``null`` ; `permissions`: { `editSequenceState`: [`AuthRequired`](#authrequired) ; `editState`: [`AuthRequired`](#authrequired) ; `incrementNonce`: [`AuthRequired`](#authrequired) ; `receive`: [`AuthRequired`](#authrequired) ; `send`: [`AuthRequired`](#authrequired) ; `setDelegate`: [`AuthRequired`](#authrequired) ; `setPermissions`: [`AuthRequired`](#authrequired) ; `setTokenSymbol`: [`AuthRequired`](#authrequired) ; `setVerificationKey`: [`AuthRequired`](#authrequired) ; `setVotingFor`: [`AuthRequired`](#authrequired) ; `setZkappUri`: [`AuthRequired`](#authrequired)  } \| ``null`` ; `timing`: { `cliffAmount`: [`UInt64`](#uint64) ; `cliffTime`: [`UInt32`](#uint32) ; `initialMinimumBalance`: [`UInt64`](#uint64) ; `vestingIncrement`: [`UInt64`](#uint64) ; `vestingPeriod`: [`UInt32`](#uint32)  } \| ``null`` ; `tokenSymbol`: `string` \| ``null`` ; `verificationKey`: { `data`: `string` ; `hash`: [`Field`](#field)  } \| ``null`` ; `votingFor`: [`Field`](#field) \| ``null`` ; `zkappUri`: `string` \| ``null``  } |
| `body.update.appState` | ([`Field`](#field) \| ``null``)[] |
| `body.update.delegate` | [`PublicKey`](#publickey) \| ``null`` |
| `body.update.permissions` | { `editSequenceState`: [`AuthRequired`](#authrequired) ; `editState`: [`AuthRequired`](#authrequired) ; `incrementNonce`: [`AuthRequired`](#authrequired) ; `receive`: [`AuthRequired`](#authrequired) ; `send`: [`AuthRequired`](#authrequired) ; `setDelegate`: [`AuthRequired`](#authrequired) ; `setPermissions`: [`AuthRequired`](#authrequired) ; `setTokenSymbol`: [`AuthRequired`](#authrequired) ; `setVerificationKey`: [`AuthRequired`](#authrequired) ; `setVotingFor`: [`AuthRequired`](#authrequired) ; `setZkappUri`: [`AuthRequired`](#authrequired)  } \| ``null`` |
| `body.update.timing` | { `cliffAmount`: [`UInt64`](#uint64) ; `cliffTime`: [`UInt32`](#uint32) ; `initialMinimumBalance`: [`UInt64`](#uint64) ; `vestingIncrement`: [`UInt64`](#uint64) ; `vestingPeriod`: [`UInt32`](#uint32)  } \| ``null`` |
| `body.update.tokenSymbol` | `string` \| ``null`` |
| `body.update.verificationKey` | { `data`: `string` ; `hash`: [`Field`](#field)  } \| ``null`` |
| `body.update.votingFor` | [`Field`](#field) \| ``null`` |
| `body.update.zkappUri` | `string` \| ``null`` |
| `body.useFullCommitment` | [`Bool`](#bool) |

##### Defined in

[snarky/gen/parties-json.ts:159](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/gen/parties-json.ts#L159)

___

#### PublicKey

Ƭ **PublicKey**: `string`

##### Defined in

[snarky/parties-leaves-json.ts:9](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves-json.ts#L9)

___

#### Sign

Ƭ **Sign**: ``"Positive"`` \| ``"Negative"``

##### Defined in

[snarky/parties-leaves-json.ts:10](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves-json.ts#L10)

___

#### TokenId

Ƭ **TokenId**: [`Field`](#field)

##### Defined in

[snarky/parties-leaves-json.ts:12](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves-json.ts#L12)

___

#### TypeMap

Ƭ **TypeMap**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `AuthRequired` | [`AuthRequired`](#authrequired) |
| `Bool` | [`Bool`](#bool) |
| `Field` | [`Field`](#field) |
| `PublicKey` | [`PublicKey`](#publickey) |
| `Sign` | [`Sign`](#sign) |
| `TokenId` | [`TokenId`](#tokenid) |
| `UInt32` | [`UInt32`](#uint32) |
| `UInt64` | [`UInt64`](#uint64) |
| `null` | ``null`` |
| `number` | `number` |
| `string` | `string` |
| `undefined` | ``null`` |

##### Defined in

[snarky/parties-leaves-json.ts:15](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves-json.ts#L15)

___

#### UInt32

Ƭ **UInt32**: `string`

##### Defined in

[snarky/parties-leaves-json.ts:8](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves-json.ts#L8)

___

#### UInt64

Ƭ **UInt64**: `string`

##### Defined in

[snarky/parties-leaves-json.ts:7](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves-json.ts#L7)


<a name="modulestypesmd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / Types

## Namespace: Types

### Table of contents

#### References

- [Bool](#bool)
- [Field](#field)
- [Sign](#sign)
- [UInt32](#uint32)
- [UInt64](#uint64)

#### Namespaces

- [Json](#modulestypesjsonmd)

#### Classes

- [PublicKey](#classestypespublickeymd)

#### Type Aliases

- [AuthRequired](#authrequired)
- [Parties](#parties)
- [Party](#party)
- [TokenId](#tokenid)
- [TokenSymbol](#tokensymbol)
- [TypeMap](#typemap)

#### Variables

- [AuthRequired](#authrequired-1)
- [Events](#events)
- [Parties](#parties-1)
- [Party](#party-1)
- [SequenceEvents](#sequenceevents)
- [StringWithHash](#stringwithhash)
- [TokenId](#tokenid-1)
- [TokenSymbol](#tokensymbol-1)
- [TypeMap](#typemap-1)
- [customTypes](#customtypes)

### References

#### Bool

Re-exports [Bool](#classesboolmd)

___

#### Field

Re-exports [Field](#classesfieldmd)

___

#### Sign

Re-exports [Sign](#classessignmd)

___

#### UInt32

Re-exports [UInt32](#classesuint32md)

___

#### UInt64

Re-exports [UInt64](#classesuint64md)

### Type Aliases

#### AuthRequired

Ƭ **AuthRequired**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `constant` | [`Bool`](#classesboolmd) |
| `signatureNecessary` | [`Bool`](#classesboolmd) |
| `signatureSufficient` | [`Bool`](#classesboolmd) |

##### Defined in

[snarky/parties-leaves.ts:20](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves.ts#L20)

___

#### Parties

Ƭ **Parties**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `feePayer` | { `authorization`: `string` ; `body`: { `fee`: [`UInt64`](#classesuint64md) ; `nonce`: [`UInt32`](#classesuint32md) ; `publicKey`: [`PublicKey`](#classestypespublickeymd) ; `validUntil?`: [`UInt32`](#classesuint32md)  }  } |
| `feePayer.authorization` | `string` |
| `feePayer.body` | { `fee`: [`UInt64`](#classesuint64md) ; `nonce`: [`UInt32`](#classesuint32md) ; `publicKey`: [`PublicKey`](#classestypespublickeymd) ; `validUntil?`: [`UInt32`](#classesuint32md)  } |
| `feePayer.body.fee` | [`UInt64`](#classesuint64md) |
| `feePayer.body.nonce` | [`UInt32`](#classesuint32md) |
| `feePayer.body.publicKey` | [`PublicKey`](#classestypespublickeymd) |
| `feePayer.body.validUntil?` | [`UInt32`](#classesuint32md) |
| `memo` | `string` |
| `otherParties` | { `authorization`: { `proof?`: `string` ; `signature?`: `string`  } ; `body`: { `balanceChange`: { `magnitude`: [`UInt64`](#classesuint64md) ; `sgn`: [`Sign`](#classessignmd)  } ; `callData`: [`Field`](#classesfieldmd) ; `callDepth`: `number` ; `caller`: [`TokenId`](#tokenid-1) ; `events`: { `data`: [`Field`](#classesfieldmd)[][] ; `hash`: [`Field`](#classesfieldmd)  } ; `incrementNonce`: [`Bool`](#classesboolmd) ; `preconditions`: { `account`: { `balance`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } ; `delegate`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`PublicKey`](#classestypespublickeymd)  } ; `isNew`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Bool`](#classesboolmd)  } ; `nonce`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `provedState`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Bool`](#classesboolmd)  } ; `receiptChainHash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `sequenceState`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `state`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }[]  } ; `network`: { `blockchainLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceGenesis`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceHardFork`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `minWindowDensity`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `nextEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `snarkedLedgerHash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `stakingEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `timestamp`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  }  } ; `publicKey`: [`PublicKey`](#classestypespublickeymd) ; `sequenceEvents`: { `data`: [`Field`](#classesfieldmd)[][] ; `hash`: [`Field`](#classesfieldmd)  } ; `tokenId`: [`TokenId`](#tokenid-1) ; `update`: { `appState`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }[] ; `delegate`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`PublicKey`](#classestypespublickeymd)  } ; `permissions`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `editSequenceState`: [`AuthRequired`](#authrequired-1) ; `editState`: [`AuthRequired`](#authrequired-1) ; `incrementNonce`: [`AuthRequired`](#authrequired-1) ; `receive`: [`AuthRequired`](#authrequired-1) ; `send`: [`AuthRequired`](#authrequired-1) ; `setDelegate`: [`AuthRequired`](#authrequired-1) ; `setPermissions`: [`AuthRequired`](#authrequired-1) ; `setTokenSymbol`: [`AuthRequired`](#authrequired-1) ; `setVerificationKey`: [`AuthRequired`](#authrequired-1) ; `setVotingFor`: [`AuthRequired`](#authrequired-1) ; `setZkappUri`: [`AuthRequired`](#authrequired-1)  }  } ; `timing`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `cliffAmount`: [`UInt64`](#classesuint64md) ; `cliffTime`: [`UInt32`](#classesuint32md) ; `initialMinimumBalance`: [`UInt64`](#classesuint64md) ; `vestingIncrement`: [`UInt64`](#classesuint64md) ; `vestingPeriod`: [`UInt32`](#classesuint32md)  }  } ; `tokenSymbol`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`TokenSymbol`](#tokensymbol-1)  } ; `verificationKey`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `data`: `string` ; `hash`: [`Field`](#classesfieldmd)  }  } ; `votingFor`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `zkappUri`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `data`: `string` ; `hash`: [`Field`](#classesfieldmd)  }  }  } ; `useFullCommitment`: [`Bool`](#classesboolmd)  }  }[] |

##### Defined in

[snarky/gen/parties.ts:43](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/gen/parties.ts#L43)

___

#### Party

Ƭ **Party**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `authorization` | { `proof?`: `string` ; `signature?`: `string`  } |
| `authorization.proof?` | `string` |
| `authorization.signature?` | `string` |
| `body` | { `balanceChange`: { `magnitude`: [`UInt64`](#classesuint64md) ; `sgn`: [`Sign`](#classessignmd)  } ; `callData`: [`Field`](#classesfieldmd) ; `callDepth`: `number` ; `caller`: [`TokenId`](#tokenid-1) ; `events`: { `data`: [`Field`](#classesfieldmd)[][] ; `hash`: [`Field`](#classesfieldmd)  } ; `incrementNonce`: [`Bool`](#classesboolmd) ; `preconditions`: { `account`: { `balance`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } ; `delegate`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`PublicKey`](#classestypespublickeymd)  } ; `isNew`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Bool`](#classesboolmd)  } ; `nonce`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `provedState`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Bool`](#classesboolmd)  } ; `receiptChainHash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `sequenceState`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `state`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }[]  } ; `network`: { `blockchainLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceGenesis`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceHardFork`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `minWindowDensity`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `nextEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `snarkedLedgerHash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `stakingEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `timestamp`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  }  } ; `publicKey`: [`PublicKey`](#classestypespublickeymd) ; `sequenceEvents`: { `data`: [`Field`](#classesfieldmd)[][] ; `hash`: [`Field`](#classesfieldmd)  } ; `tokenId`: [`TokenId`](#tokenid-1) ; `update`: { `appState`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }[] ; `delegate`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`PublicKey`](#classestypespublickeymd)  } ; `permissions`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `editSequenceState`: [`AuthRequired`](#authrequired-1) ; `editState`: [`AuthRequired`](#authrequired-1) ; `incrementNonce`: [`AuthRequired`](#authrequired-1) ; `receive`: [`AuthRequired`](#authrequired-1) ; `send`: [`AuthRequired`](#authrequired-1) ; `setDelegate`: [`AuthRequired`](#authrequired-1) ; `setPermissions`: [`AuthRequired`](#authrequired-1) ; `setTokenSymbol`: [`AuthRequired`](#authrequired-1) ; `setVerificationKey`: [`AuthRequired`](#authrequired-1) ; `setVotingFor`: [`AuthRequired`](#authrequired-1) ; `setZkappUri`: [`AuthRequired`](#authrequired-1)  }  } ; `timing`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `cliffAmount`: [`UInt64`](#classesuint64md) ; `cliffTime`: [`UInt32`](#classesuint32md) ; `initialMinimumBalance`: [`UInt64`](#classesuint64md) ; `vestingIncrement`: [`UInt64`](#classesuint64md) ; `vestingPeriod`: [`UInt32`](#classesuint32md)  }  } ; `tokenSymbol`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`TokenSymbol`](#tokensymbol-1)  } ; `verificationKey`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `data`: `string` ; `hash`: [`Field`](#classesfieldmd)  }  } ; `votingFor`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `zkappUri`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `data`: `string` ; `hash`: [`Field`](#classesfieldmd)  }  }  } ; `useFullCommitment`: [`Bool`](#classesboolmd)  } |
| `body.balanceChange` | { `magnitude`: [`UInt64`](#classesuint64md) ; `sgn`: [`Sign`](#classessignmd)  } |
| `body.balanceChange.magnitude` | [`UInt64`](#classesuint64md) |
| `body.balanceChange.sgn` | [`Sign`](#classessignmd) |
| `body.callData` | [`Field`](#classesfieldmd) |
| `body.callDepth` | `number` |
| `body.caller` | [`TokenId`](#tokenid-1) |
| `body.events` | { `data`: [`Field`](#classesfieldmd)[][] ; `hash`: [`Field`](#classesfieldmd)  } |
| `body.events.data` | [`Field`](#classesfieldmd)[][] |
| `body.events.hash` | [`Field`](#classesfieldmd) |
| `body.incrementNonce` | [`Bool`](#classesboolmd) |
| `body.preconditions` | { `account`: { `balance`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } ; `delegate`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`PublicKey`](#classestypespublickeymd)  } ; `isNew`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Bool`](#classesboolmd)  } ; `nonce`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `provedState`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Bool`](#classesboolmd)  } ; `receiptChainHash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `sequenceState`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `state`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }[]  } ; `network`: { `blockchainLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceGenesis`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceHardFork`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `minWindowDensity`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `nextEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `snarkedLedgerHash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `stakingEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `timestamp`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  }  } |
| `body.preconditions.account` | { `balance`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } ; `delegate`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`PublicKey`](#classestypespublickeymd)  } ; `isNew`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Bool`](#classesboolmd)  } ; `nonce`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `provedState`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Bool`](#classesboolmd)  } ; `receiptChainHash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `sequenceState`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `state`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }[]  } |
| `body.preconditions.account.balance` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } |
| `body.preconditions.account.balance.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.account.balance.value` | { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  } |
| `body.preconditions.account.balance.value.lower` | [`UInt64`](#classesuint64md) |
| `body.preconditions.account.balance.value.upper` | [`UInt64`](#classesuint64md) |
| `body.preconditions.account.delegate` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`PublicKey`](#classestypespublickeymd)  } |
| `body.preconditions.account.delegate.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.account.delegate.value` | [`PublicKey`](#classestypespublickeymd) |
| `body.preconditions.account.isNew` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Bool`](#classesboolmd)  } |
| `body.preconditions.account.isNew.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.account.isNew.value` | [`Bool`](#classesboolmd) |
| `body.preconditions.account.nonce` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } |
| `body.preconditions.account.nonce.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.account.nonce.value` | { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  } |
| `body.preconditions.account.nonce.value.lower` | [`UInt32`](#classesuint32md) |
| `body.preconditions.account.nonce.value.upper` | [`UInt32`](#classesuint32md) |
| `body.preconditions.account.provedState` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Bool`](#classesboolmd)  } |
| `body.preconditions.account.provedState.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.account.provedState.value` | [`Bool`](#classesboolmd) |
| `body.preconditions.account.receiptChainHash` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } |
| `body.preconditions.account.receiptChainHash.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.account.receiptChainHash.value` | [`Field`](#classesfieldmd) |
| `body.preconditions.account.sequenceState` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } |
| `body.preconditions.account.sequenceState.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.account.sequenceState.value` | [`Field`](#classesfieldmd) |
| `body.preconditions.account.state` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }[] |
| `body.preconditions.network` | { `blockchainLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceGenesis`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `globalSlotSinceHardFork`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `minWindowDensity`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `nextEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `snarkedLedgerHash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `stakingEpochData`: { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } ; `timestamp`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } |
| `body.preconditions.network.blockchainLength` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } |
| `body.preconditions.network.blockchainLength.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.blockchainLength.value` | { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  } |
| `body.preconditions.network.blockchainLength.value.lower` | [`UInt32`](#classesuint32md) |
| `body.preconditions.network.blockchainLength.value.upper` | [`UInt32`](#classesuint32md) |
| `body.preconditions.network.globalSlotSinceGenesis` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } |
| `body.preconditions.network.globalSlotSinceGenesis.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.globalSlotSinceGenesis.value` | { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  } |
| `body.preconditions.network.globalSlotSinceGenesis.value.lower` | [`UInt32`](#classesuint32md) |
| `body.preconditions.network.globalSlotSinceGenesis.value.upper` | [`UInt32`](#classesuint32md) |
| `body.preconditions.network.globalSlotSinceHardFork` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } |
| `body.preconditions.network.globalSlotSinceHardFork.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.globalSlotSinceHardFork.value` | { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  } |
| `body.preconditions.network.globalSlotSinceHardFork.value.lower` | [`UInt32`](#classesuint32md) |
| `body.preconditions.network.globalSlotSinceHardFork.value.upper` | [`UInt32`](#classesuint32md) |
| `body.preconditions.network.minWindowDensity` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } |
| `body.preconditions.network.minWindowDensity.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.minWindowDensity.value` | { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  } |
| `body.preconditions.network.minWindowDensity.value.lower` | [`UInt32`](#classesuint32md) |
| `body.preconditions.network.minWindowDensity.value.upper` | [`UInt32`](#classesuint32md) |
| `body.preconditions.network.nextEpochData` | { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } |
| `body.preconditions.network.nextEpochData.epochLength` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } |
| `body.preconditions.network.nextEpochData.epochLength.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.nextEpochData.epochLength.value` | { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  } |
| `body.preconditions.network.nextEpochData.epochLength.value.lower` | [`UInt32`](#classesuint32md) |
| `body.preconditions.network.nextEpochData.epochLength.value.upper` | [`UInt32`](#classesuint32md) |
| `body.preconditions.network.nextEpochData.ledger` | { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } |
| `body.preconditions.network.nextEpochData.ledger.hash` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } |
| `body.preconditions.network.nextEpochData.ledger.hash.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.nextEpochData.ledger.hash.value` | [`Field`](#classesfieldmd) |
| `body.preconditions.network.nextEpochData.ledger.totalCurrency` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } |
| `body.preconditions.network.nextEpochData.ledger.totalCurrency.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.nextEpochData.ledger.totalCurrency.value` | { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  } |
| `body.preconditions.network.nextEpochData.ledger.totalCurrency.value.lower` | [`UInt64`](#classesuint64md) |
| `body.preconditions.network.nextEpochData.ledger.totalCurrency.value.upper` | [`UInt64`](#classesuint64md) |
| `body.preconditions.network.nextEpochData.lockCheckpoint` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } |
| `body.preconditions.network.nextEpochData.lockCheckpoint.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.nextEpochData.lockCheckpoint.value` | [`Field`](#classesfieldmd) |
| `body.preconditions.network.nextEpochData.seed` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } |
| `body.preconditions.network.nextEpochData.seed.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.nextEpochData.seed.value` | [`Field`](#classesfieldmd) |
| `body.preconditions.network.nextEpochData.startCheckpoint` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } |
| `body.preconditions.network.nextEpochData.startCheckpoint.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.nextEpochData.startCheckpoint.value` | [`Field`](#classesfieldmd) |
| `body.preconditions.network.snarkedLedgerHash` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } |
| `body.preconditions.network.snarkedLedgerHash.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.snarkedLedgerHash.value` | [`Field`](#classesfieldmd) |
| `body.preconditions.network.stakingEpochData` | { `epochLength`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } ; `ledger`: { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } ; `lockCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `seed`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `startCheckpoint`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }  } |
| `body.preconditions.network.stakingEpochData.epochLength` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  }  } |
| `body.preconditions.network.stakingEpochData.epochLength.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.stakingEpochData.epochLength.value` | { `lower`: [`UInt32`](#classesuint32md) ; `upper`: [`UInt32`](#classesuint32md)  } |
| `body.preconditions.network.stakingEpochData.epochLength.value.lower` | [`UInt32`](#classesuint32md) |
| `body.preconditions.network.stakingEpochData.epochLength.value.upper` | [`UInt32`](#classesuint32md) |
| `body.preconditions.network.stakingEpochData.ledger` | { `hash`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `totalCurrency`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  }  } |
| `body.preconditions.network.stakingEpochData.ledger.hash` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } |
| `body.preconditions.network.stakingEpochData.ledger.hash.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.stakingEpochData.ledger.hash.value` | [`Field`](#classesfieldmd) |
| `body.preconditions.network.stakingEpochData.ledger.totalCurrency` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } |
| `body.preconditions.network.stakingEpochData.ledger.totalCurrency.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.stakingEpochData.ledger.totalCurrency.value` | { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  } |
| `body.preconditions.network.stakingEpochData.ledger.totalCurrency.value.lower` | [`UInt64`](#classesuint64md) |
| `body.preconditions.network.stakingEpochData.ledger.totalCurrency.value.upper` | [`UInt64`](#classesuint64md) |
| `body.preconditions.network.stakingEpochData.lockCheckpoint` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } |
| `body.preconditions.network.stakingEpochData.lockCheckpoint.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.stakingEpochData.lockCheckpoint.value` | [`Field`](#classesfieldmd) |
| `body.preconditions.network.stakingEpochData.seed` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } |
| `body.preconditions.network.stakingEpochData.seed.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.stakingEpochData.seed.value` | [`Field`](#classesfieldmd) |
| `body.preconditions.network.stakingEpochData.startCheckpoint` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } |
| `body.preconditions.network.stakingEpochData.startCheckpoint.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.stakingEpochData.startCheckpoint.value` | [`Field`](#classesfieldmd) |
| `body.preconditions.network.timestamp` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } |
| `body.preconditions.network.timestamp.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.timestamp.value` | { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  } |
| `body.preconditions.network.timestamp.value.lower` | [`UInt64`](#classesuint64md) |
| `body.preconditions.network.timestamp.value.upper` | [`UInt64`](#classesuint64md) |
| `body.preconditions.network.totalCurrency` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  }  } |
| `body.preconditions.network.totalCurrency.isSome` | [`Bool`](#classesboolmd) |
| `body.preconditions.network.totalCurrency.value` | { `lower`: [`UInt64`](#classesuint64md) ; `upper`: [`UInt64`](#classesuint64md)  } |
| `body.preconditions.network.totalCurrency.value.lower` | [`UInt64`](#classesuint64md) |
| `body.preconditions.network.totalCurrency.value.upper` | [`UInt64`](#classesuint64md) |
| `body.publicKey` | [`PublicKey`](#classestypespublickeymd) |
| `body.sequenceEvents` | { `data`: [`Field`](#classesfieldmd)[][] ; `hash`: [`Field`](#classesfieldmd)  } |
| `body.sequenceEvents.data` | [`Field`](#classesfieldmd)[][] |
| `body.sequenceEvents.hash` | [`Field`](#classesfieldmd) |
| `body.tokenId` | [`TokenId`](#tokenid-1) |
| `body.update` | { `appState`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }[] ; `delegate`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`PublicKey`](#classestypespublickeymd)  } ; `permissions`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `editSequenceState`: [`AuthRequired`](#authrequired-1) ; `editState`: [`AuthRequired`](#authrequired-1) ; `incrementNonce`: [`AuthRequired`](#authrequired-1) ; `receive`: [`AuthRequired`](#authrequired-1) ; `send`: [`AuthRequired`](#authrequired-1) ; `setDelegate`: [`AuthRequired`](#authrequired-1) ; `setPermissions`: [`AuthRequired`](#authrequired-1) ; `setTokenSymbol`: [`AuthRequired`](#authrequired-1) ; `setVerificationKey`: [`AuthRequired`](#authrequired-1) ; `setVotingFor`: [`AuthRequired`](#authrequired-1) ; `setZkappUri`: [`AuthRequired`](#authrequired-1)  }  } ; `timing`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `cliffAmount`: [`UInt64`](#classesuint64md) ; `cliffTime`: [`UInt32`](#classesuint32md) ; `initialMinimumBalance`: [`UInt64`](#classesuint64md) ; `vestingIncrement`: [`UInt64`](#classesuint64md) ; `vestingPeriod`: [`UInt32`](#classesuint32md)  }  } ; `tokenSymbol`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`TokenSymbol`](#tokensymbol-1)  } ; `verificationKey`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `data`: `string` ; `hash`: [`Field`](#classesfieldmd)  }  } ; `votingFor`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } ; `zkappUri`: { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `data`: `string` ; `hash`: [`Field`](#classesfieldmd)  }  }  } |
| `body.update.appState` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  }[] |
| `body.update.delegate` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`PublicKey`](#classestypespublickeymd)  } |
| `body.update.delegate.isSome` | [`Bool`](#classesboolmd) |
| `body.update.delegate.value` | [`PublicKey`](#classestypespublickeymd) |
| `body.update.permissions` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `editSequenceState`: [`AuthRequired`](#authrequired-1) ; `editState`: [`AuthRequired`](#authrequired-1) ; `incrementNonce`: [`AuthRequired`](#authrequired-1) ; `receive`: [`AuthRequired`](#authrequired-1) ; `send`: [`AuthRequired`](#authrequired-1) ; `setDelegate`: [`AuthRequired`](#authrequired-1) ; `setPermissions`: [`AuthRequired`](#authrequired-1) ; `setTokenSymbol`: [`AuthRequired`](#authrequired-1) ; `setVerificationKey`: [`AuthRequired`](#authrequired-1) ; `setVotingFor`: [`AuthRequired`](#authrequired-1) ; `setZkappUri`: [`AuthRequired`](#authrequired-1)  }  } |
| `body.update.permissions.isSome` | [`Bool`](#classesboolmd) |
| `body.update.permissions.value` | { `editSequenceState`: [`AuthRequired`](#authrequired-1) ; `editState`: [`AuthRequired`](#authrequired-1) ; `incrementNonce`: [`AuthRequired`](#authrequired-1) ; `receive`: [`AuthRequired`](#authrequired-1) ; `send`: [`AuthRequired`](#authrequired-1) ; `setDelegate`: [`AuthRequired`](#authrequired-1) ; `setPermissions`: [`AuthRequired`](#authrequired-1) ; `setTokenSymbol`: [`AuthRequired`](#authrequired-1) ; `setVerificationKey`: [`AuthRequired`](#authrequired-1) ; `setVotingFor`: [`AuthRequired`](#authrequired-1) ; `setZkappUri`: [`AuthRequired`](#authrequired-1)  } |
| `body.update.permissions.value.editSequenceState` | [`AuthRequired`](#authrequired-1) |
| `body.update.permissions.value.editState` | [`AuthRequired`](#authrequired-1) |
| `body.update.permissions.value.incrementNonce` | [`AuthRequired`](#authrequired-1) |
| `body.update.permissions.value.receive` | [`AuthRequired`](#authrequired-1) |
| `body.update.permissions.value.send` | [`AuthRequired`](#authrequired-1) |
| `body.update.permissions.value.setDelegate` | [`AuthRequired`](#authrequired-1) |
| `body.update.permissions.value.setPermissions` | [`AuthRequired`](#authrequired-1) |
| `body.update.permissions.value.setTokenSymbol` | [`AuthRequired`](#authrequired-1) |
| `body.update.permissions.value.setVerificationKey` | [`AuthRequired`](#authrequired-1) |
| `body.update.permissions.value.setVotingFor` | [`AuthRequired`](#authrequired-1) |
| `body.update.permissions.value.setZkappUri` | [`AuthRequired`](#authrequired-1) |
| `body.update.timing` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `cliffAmount`: [`UInt64`](#classesuint64md) ; `cliffTime`: [`UInt32`](#classesuint32md) ; `initialMinimumBalance`: [`UInt64`](#classesuint64md) ; `vestingIncrement`: [`UInt64`](#classesuint64md) ; `vestingPeriod`: [`UInt32`](#classesuint32md)  }  } |
| `body.update.timing.isSome` | [`Bool`](#classesboolmd) |
| `body.update.timing.value` | { `cliffAmount`: [`UInt64`](#classesuint64md) ; `cliffTime`: [`UInt32`](#classesuint32md) ; `initialMinimumBalance`: [`UInt64`](#classesuint64md) ; `vestingIncrement`: [`UInt64`](#classesuint64md) ; `vestingPeriod`: [`UInt32`](#classesuint32md)  } |
| `body.update.timing.value.cliffAmount` | [`UInt64`](#classesuint64md) |
| `body.update.timing.value.cliffTime` | [`UInt32`](#classesuint32md) |
| `body.update.timing.value.initialMinimumBalance` | [`UInt64`](#classesuint64md) |
| `body.update.timing.value.vestingIncrement` | [`UInt64`](#classesuint64md) |
| `body.update.timing.value.vestingPeriod` | [`UInt32`](#classesuint32md) |
| `body.update.tokenSymbol` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`TokenSymbol`](#tokensymbol-1)  } |
| `body.update.tokenSymbol.isSome` | [`Bool`](#classesboolmd) |
| `body.update.tokenSymbol.value` | [`TokenSymbol`](#tokensymbol-1) |
| `body.update.verificationKey` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `data`: `string` ; `hash`: [`Field`](#classesfieldmd)  }  } |
| `body.update.verificationKey.isSome` | [`Bool`](#classesboolmd) |
| `body.update.verificationKey.value` | { `data`: `string` ; `hash`: [`Field`](#classesfieldmd)  } |
| `body.update.verificationKey.value.data` | `string` |
| `body.update.verificationKey.value.hash` | [`Field`](#classesfieldmd) |
| `body.update.votingFor` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: [`Field`](#classesfieldmd)  } |
| `body.update.votingFor.isSome` | [`Bool`](#classesboolmd) |
| `body.update.votingFor.value` | [`Field`](#classesfieldmd) |
| `body.update.zkappUri` | { `isSome`: [`Bool`](#classesboolmd) ; `value`: { `data`: `string` ; `hash`: [`Field`](#classesfieldmd)  }  } |
| `body.update.zkappUri.isSome` | [`Bool`](#classesboolmd) |
| `body.update.zkappUri.value` | { `data`: `string` ; `hash`: [`Field`](#classesfieldmd)  } |
| `body.update.zkappUri.value.data` | `string` |
| `body.update.zkappUri.value.hash` | [`Field`](#classesfieldmd) |
| `body.useFullCommitment` | [`Bool`](#classesboolmd) |

##### Defined in

[snarky/gen/parties.ts:247](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/gen/parties.ts#L247)

___

#### TokenId

Ƭ **TokenId**: [`Field`](#classesfieldmd)

##### Defined in

[snarky/parties-leaves.ts:25](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves.ts#L25)

___

#### TokenSymbol

Ƭ **TokenSymbol**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `field` | [`Field`](#classesfieldmd) |
| `symbol` | `string` |

##### Defined in

[lib/hash.ts:133](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/hash.ts#L133)

___

#### TypeMap

Ƭ **TypeMap**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `AuthRequired` | [`AuthRequired`](#authrequired-1) |
| `Bool` | [`Bool`](#classesboolmd) |
| `Field` | [`Field`](#classesfieldmd) |
| `PublicKey` | [`PublicKey`](#classestypespublickeymd) |
| `Sign` | [`Sign`](#classessignmd) |
| `TokenId` | [`TokenId`](#tokenid-1) |
| `UInt32` | [`UInt32`](#classesuint32md) |
| `UInt64` | [`UInt64`](#classesuint64md) |
| `null` | ``null`` |
| `number` | `number` |
| `string` | `string` |
| `undefined` | `undefined` |

##### Defined in

[snarky/parties-leaves.ts:28](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves.ts#L28)

### Variables

#### AuthRequired

• **AuthRequired**: `AsFieldsExtended`<[`AuthRequired`](#authrequired-1)\>

##### Defined in

[snarky/parties-leaves.ts:64](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves.ts#L64)

___

#### Events

• `Const` **Events**: `AsFieldsAndAux`<`DataAsHash`<[`Field`](#classesfieldmd)[][]\>, `string`[][]\>

##### Defined in

[snarky/parties-leaves.ts:128](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves.ts#L128)

___

#### Parties

• **Parties**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `check` | (`value`: [`Parties`](#parties-1)) => `void` |
| `fromFields` | (`fields`: [`Field`](#classesfieldmd)[], `aux`: `any`[]) => [`Parties`](#parties-1) |
| `sizeInFields` | () => `number` |
| `toAuxiliary` | (`value?`: [`Parties`](#parties-1)) => `any`[] |
| `toFields` | (`value`: [`Parties`](#parties-1)) => [`Field`](#classesfieldmd)[] |
| `toInput` | (`value`: [`Parties`](#parties-1)) => `HashInput` |
| `toJSON` | (`value`: [`Parties`](#parties-1)) => [`Parties`](#parties) |
| `witness` | (`f`: () => [`Parties`](#parties-1)) => [`Parties`](#parties-1) |

##### Defined in

[snarky/gen/parties.ts:242](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/gen/parties.ts#L242)

___

#### Party

• **Party**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `check` | (`value`: [`Party`](#party-1)) => `void` |
| `fromFields` | (`fields`: [`Field`](#classesfieldmd)[], `aux`: `any`[]) => [`Party`](#party-1) |
| `sizeInFields` | () => `number` |
| `toAuxiliary` | (`value?`: [`Party`](#party-1)) => `any`[] |
| `toFields` | (`value`: [`Party`](#party-1)) => [`Field`](#classesfieldmd)[] |
| `toInput` | (`value`: [`Party`](#party-1)) => `HashInput` |
| `toJSON` | (`value`: [`Party`](#party-1)) => [`Party`](#party) |
| `witness` | (`f`: () => [`Party`](#party-1)) => [`Party`](#party-1) |

##### Defined in

[snarky/gen/parties.ts:434](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/gen/parties.ts#L434)

___

#### SequenceEvents

• `Const` **SequenceEvents**: `AsFieldsAndAux`<`DataAsHash`<[`Field`](#classesfieldmd)[][]\>, `string`[][]\>

##### Defined in

[snarky/parties-leaves.ts:152](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves.ts#L152)

___

#### StringWithHash

• `Const` **StringWithHash**: `AsFieldsAndAux`<`DataAsHash`<`string`\>, `string`\>

##### Defined in

[snarky/parties-leaves.ts:176](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves.ts#L176)

___

#### TokenId

• **TokenId**: `AsFieldsExtended`<[`Field`](#classesfieldmd)\>

##### Defined in

[snarky/parties-leaves.ts:57](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves.ts#L57)

___

#### TokenSymbol

• **TokenSymbol**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `empty` | { `field`: [`Field`](#classesfieldmd) = Field.zero; `symbol`: `string` = '' } |
| `empty.field` | [`Field`](#classesfieldmd) |
| `empty.symbol` | `string` |
| `check` | (`value`: [`TokenSymbol`](#tokensymbol-1)) => `void` |
| `from` | (`symbol`: `string`) => [`TokenSymbol`](#tokensymbol-1) |
| `fromFields` | (`fields`: [`Field`](#classesfieldmd)[], `aux`: `any`[]) => [`TokenSymbol`](#tokensymbol-1) |
| `sizeInFields` | () => `number` |
| `toAuxiliary` | (`value?`: [`TokenSymbol`](#tokensymbol-1)) => `any`[] |
| `toFields` | (`value`: [`TokenSymbol`](#tokensymbol-1)) => [`Field`](#classesfieldmd)[] |
| `toInput` | (`value`: [`TokenSymbol`](#tokensymbol-1)) => `HashInput` |
| `toJSON` | (`value`: [`TokenSymbol`](#tokensymbol-1)) => `string` |

##### Defined in

[lib/hash.ts:161](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/hash.ts#L161)

___

#### TypeMap

• **TypeMap**: `Object`

##### Type declaration

| Name | Type |
| :------ | :------ |
| `AuthRequired` | `AsFieldsAndAux`<[`AuthRequired`](#authrequired-1), [`AuthRequired`](#authrequired)\> |
| `Bool` | `AsFieldsAndAux`<[`Bool`](#classesboolmd), `boolean`\> |
| `Field` | `AsFieldsAndAux`<[`Field`](#classesfieldmd), `string`\> |
| `PublicKey` | `AsFieldsAndAux`<[`PublicKey`](#classestypespublickeymd), `string`\> |
| `Sign` | `AsFieldsAndAux`<[`Sign`](#classessignmd), [`Sign`](#sign)\> |
| `TokenId` | `AsFieldsAndAux`<[`Field`](#classesfieldmd), `string`\> |
| `UInt32` | `AsFieldsAndAux`<[`UInt32`](#classesuint32md), `string`\> |
| `UInt64` | `AsFieldsAndAux`<[`UInt64`](#classesuint64md), `string`\> |
| `null` | `AsFieldsAndAux`<``null``, ``null``\> |
| `number` | `AsFieldsAndAux`<`number`, `number`\> |
| `string` | `AsFieldsAndAux`<`string`, `string`\> |
| `undefined` | `AsFieldsAndAux`<`undefined`, ``null``\> |

##### Defined in

[snarky/parties-leaves.ts:93](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/parties-leaves.ts#L93)

___

#### customTypes

• **customTypes**: `CustomTypes`

##### Defined in

[snarky/gen/parties.ts:41](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/snarky/gen/parties.ts#L41)


<a name="moduleszkprogrammd"></a>

[snarkyjs](#readmemd) / [Exports](#modulesmd) / ZkProgram

## Namespace: ZkProgram

### Table of contents

#### Functions

- [Proof](#proof)

### Functions

#### Proof

▸ **Proof**<`PublicInputType`\>(`program`): typeof `ZkProgramProof`

##### Type parameters

| Name | Type |
| :------ | :------ |
| `PublicInputType` | extends [`AsFieldElements`](#interfacesasfieldelementsmd)<`any`, `PublicInputType`\> |

##### Parameters

| Name | Type |
| :------ | :------ |
| `program` | `Object` |
| `program.name` | `string` |
| `program.publicInputType` | `PublicInputType` |

##### Returns

typeof `ZkProgramProof`

##### Defined in

[lib/proof_system.ts:537](https://github.com/o1-labs/snarkyjs/blob/7320d0b/src/lib/proof_system.ts#L537)