This is a forked esm, flatbundled version of https://github.com/schteppe/cannon.js for easier handling in module environments and tree shaking. Visit the original project for documentations and examples.

    yarn add cannon-es

```jsx
import { World } from 'cannon-es'

// ...
```

#### TO DO:

- Check for any removed `@todo` or `@deprecated` JSDoc comments in merged PR file changes
- Check for variables that were previously intentionally uninitialized in the constructor, but were updated in the TS conversion
- Fix Octree `as any` assertions
- Convert to static methods where possible? (memory savings)
- Convert to abstract classes where possible (Equation, Solver, etc.?)
- Ensure no prototypal methods were overwritten due to error:
  - `Property xxxxx has no initializer and is not definitely assigned in the constructor`
- Resolve `as any` type assertions where possible
- Remove use of defined assertion (!) where possible (profile performance to ensure no degradation)
- Correct & standardize JSDoc comments
- Test possible performance improvements by converting matrices to Maps (instead of Arrays)
