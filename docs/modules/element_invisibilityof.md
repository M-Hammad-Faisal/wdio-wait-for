[wdio-wait-for](../README.md) / [Modules](../modules.md) / element/invisibilityOf

# Module: element/invisibilityOf

## Table of contents

### Functions

- [invisibilityOf](element_invisibilityof.md#invisibilityof)

## Functions

### invisibilityOf

▸ **invisibilityOf**(`selector`: *string*): *function*

A condition for checking the element to be invisible

**`example`** 
browser.waitUntil(invisibilityOf('.header'));

#### Parameters:

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | *string* | The selector to check |

**Returns:** () => *Promise*<boolean\>

An expected condition that returns a promise
    representing whether the element is invisible.

Defined in: element/invisibilityOf.ts:13
