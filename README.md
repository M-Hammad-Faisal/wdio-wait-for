# WDIO-WAIT-FOR

> wdio-wait-for is a Node.js library for [WebdriverIO](http://webdriver.io/) that supplies a set of common conditions that provides functionalities to wait for certain conditions till a defined task is complete.
## [API](./docs/modules.md)

- [alertIsPresent](docs/modules/browser_alertispresent.md)
- [numberOfWindowsToBe​](docs/modules/browser_numberofwindowstobe_.md)
- [titleContains](docs/modules/browser_titlecontains.md)
- [titleIs](docs/modules/browser_titleis.md)
- [urlContains](docs/modules/browser_urlcontains.md)
- [urlIs](docs/modules/browser_urlis.md)
- [elementContainsText](docs/modules/element_elementcontainstext.md)
- [elementContainsValue](docs/modules/element_elementcontainsvalue.md)
- [elementToBeClickable](docs/modules/element_elementtobeclickable.md)
- [elementToBeEnabled](docs/modules/element_elementtobeenabled.md)
- [elementToBeInvisible](docs/modules/element_elementtobeinvisible.md)
- [elementToBeVisible](docs/modules/element_elementtobevisible.md)
- [numberOfElementsToBe](docs/modules/element_numberofelementstobe.md)
- [numberOfElementsToBeLessThan](docs/modules/element_numberofelementstobelessthan.md)
- [numberOfElementsToBeMoreThan​](docs/modules/element_numberofelementstobemorethan_.md)
- [sizeOfElementToBe](docs/modules/element_sizeofelementtobe.md)

## Examples

### Import
#### JavaScript

```javascript
// import all methods
const EC = require('wdio-wait-for');

browser.waitUntil(EC.alertIsPresent(), { timeout: 5000, timeoutMsg: 'Failed, after waiting for the alert to be present' })
```

```javascript
// import specific method
const { alertIsPresent } = require('wdio-wait-for');

browser.waitUntil(alertIsPresent(), { timeout: 5000, timeoutMsg: 'Failed, after waiting for the alert to be present' })
```

#### TypeScript

```typescript
// import all methods
import * as EC from 'wdio-wait-for';

browser.waitUntil(EC.elementToBeEnabled('input'), { timeout: 5000, timeoutMsg: 'Failed, after waiting for the element to be enabled' })
```

```typescript
// import specific method
import { elementToBeEnabled } from 'wdio-wait-for';

browser.waitUntil(elementToBeEnabled('input'), { timeout: 5000, timeoutMsg: 'Failed, after waiting for the element to be enabled' })
```
### Wait for alert
This code code snippet shows how to use conditions

```typescript
browser.waitUntil(alertIsPresent(), { timeout: 5000, timeoutMsg: 'Failed, after waiting for the alert to be present' })
```
### Wait for number of elements to be
This code code snippet shows how to use conditions

```typescript
browser.waitUntil(numberOfElementsToBe('.links', 2), { timeout: 5000, timeoutMsg: 'Failed, after waiting for the 2 elements' })
```

## License

wdio-wait-for is [MIT licensed](./LICENSE).


## Author
Yevhen Laichenkov <elaichenkov@gmail.com>