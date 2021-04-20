[wdio-wait-for](../README.md) / [Modules](../modules.md) / element/elementToBeSelected

# Module: element/elementToBeSelected

## Table of contents

### Functions

- [elementToBeSelected](element_elementtobeselected.md#elementtobeselected)

## Functions

### elementToBeSelected

▸ **elementToBeSelected**(`selector`: *string*): *function*

A condition for checking an element is visible and selected

**`example`** 
browser.waitUntil(elementToBeSelected('.btn'));

#### Parameters:

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | *string* | The selector to check |

**Returns:** () => *Promise*<boolean\>

An expected condition that returns a promise
    representing whether the element is selected.

Defined in: element/elementToBeSelected.ts:13
