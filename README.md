# Simplified

Able to recursively simplify nearly any Javascript type into something JSON plus undefined.

Promises are (recursively) chained into simplified promises.

Can unwrap promises recursively into fully simplified.

Lots of tools on simplified data, like various formats of display, comparison, hashing, etc..

Use `SimplifiedWalker` like a typesafe recursive `Array.map()` on simplified types.

## Usage

```typescript
import { simplify } from "@asmartbear/simplified"

const s = simplify({a:new MyClass(), b: new Set([1,2,3])})
const sp = await simplifiedAwait(...)
```

## Development

Build:

```bash
npm run build
```

Unit tests:

```bash
npm run test
```

Unit tests, refreshed live:

```bash
npm run watch
```

Prepare for release (e.g. run tests and bump version number):

```bash
npm run release
```

Publish to npm:

```bash
npm publish
```
