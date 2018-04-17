<a name="store"></a>

## store : <code>object</code>
**Kind**: global namespace

* [store](#store) : <code>object</code>
    * [.each(callback)](#store.each)
    * [.expired(key)](#store.expired) ⇒
    * [.get(key)](#store.get) ⇒
    * [.del(key)](#store.del) ⇒
    * [.clear(key)](#store.clear) ⇒
    * [.clean(key)](#store.clean) ⇒
    * [.has(key)](#store.has) ⇒
    * [.size(unit)](#store.size) ⇒

<a name="store.each"></a>

### store.each(callback)
遍历 store

**Kind**: static method of [<code>store</code>](#store)

| Param | Type | Description |
| --- | --- | --- |
| callback | <code>function</code> | 参数为key, val(过期key的val在localstorage有                                                                                                                                                             值，但取值会为空) |

<a name="store.expired"></a>

### store.expired(key) ⇒
判断key是否过期，没有返回key的值，过期返回false

**Kind**: static method of [<code>store</code>](#store)
**Returns**: expired

| Param | Type |
| --- | --- |
| key | <code>string</code> |

<a name="store.get"></a>

### store.get(key) ⇒
通过key获取store的value值(不包含过期的)

**Kind**: static method of [<code>store</code>](#store)
**Returns**: vaule || object

| Param | Type | Description |
| --- | --- | --- |
| key | <code>string</code> | 可以为string或空，为空时取所有的localstorage |

<a name="store.del"></a>

### store.del(key) ⇒
删除store某个key及值

**Kind**: static method of [<code>store</code>](#store)
**Returns**: store

| Param | Type | Description |
| --- | --- | --- |
| key | <code>string</code> | string |

<a name="store.clear"></a>

### store.clear(key) ⇒
清除所有store存储

**Kind**: static method of [<code>store</code>](#store)
**Returns**: store

| Param | Type | Description |
| --- | --- | --- |
| key | <code>string</code> | string |

<a name="store.clean"></a>

### store.clean(key) ⇒
清除所有已过期的store存储, 运行时即执行

**Kind**: static method of [<code>store</code>](#store)
**Returns**: store

| Param | Type | Description |
| --- | --- | --- |
| key | <code>string</code> | string |

<a name="store.has"></a>

### store.has(key) ⇒
判断某key是否存在

**Kind**: static method of [<code>store</code>](#store)
**Returns**: boolean

| Param | Type | Description |
| --- | --- | --- |
| key | <code>string</code> | string |

<a name="store.size"></a>

### store.size(unit) ⇒
获取store已存储的大小

**Kind**: static method of [<code>store</code>](#store)
**Returns**: int

| Param | Type | Description |
| --- | --- | --- |
| unit | <code>string</code> | 单位默认返回bytes,可以为KB, MB; |


## Licence ##

The MIT License

Copyright (c) 2015 Joe github.com@ccjoe