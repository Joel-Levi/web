# @web/mocks

## 0.1.6

### Patch Changes

- 8cf9fcc1: Export types like Mock & handler as well via the `types.js` entrypoint.

  Example:

  ```js
  // in TS
  import { Mock } from '@web/mocks/types.js';

  // or in JsDoc

  /**
   * Gets mocks by given status
   * @param {number} status - response code status
   * @returns {import('@web/mocks/types.js').Mock[]}
   */
  export function getMocksByStatus(status) {}
  ```

## 0.1.5

### Patch Changes

- c2a9df28: fix: flatten mocks correctly

## 0.1.4

### Patch Changes

- fd7cb03e: fix: content type

## 0.1.3

### Patch Changes

- f2362bbf: Trigger pipeline

## 0.1.2

### Patch Changes

- e9c77e06: Version Packages

## 0.1.1

### Patch Changes

- 78f76396: Publish Types

## 0.1.0

### Minor Changes

- a2fb64aa: Adds support for node.js request mocking, as well as some breaking changes:

  1. Add support for request mocking in node js via `@web/mocks/node.js`
  2. rename `rest` to `http` -> not all requests/apis are RESTful, but all requests are http requests
  3. `withMocks()` to `withMocks` (no function call)
  4. move plugins from `node.js` to `plugins.js`
  5. separate `registerMockRoutes` from loading storybook code; when using `registerMockRoutes` in tests, we dont need to import storybook code
  6. remove `./msw.js`, moved into `browser.js` directly
  7. moved `storybook-decorator.js` to `@web/mocks/storybook/decorator.js`, this also leaves some space for the storybook UI addon (`@web/mocks/storybook/addon.js`), and if we decide to move the `storyFixture` (`@web/mocks/storybook/fixture.js`) in here as well

## 0.0.13

### Patch Changes

- 2062d628: chore: update sw

## 0.0.12

### Patch Changes

- 6d765f22: chore: bump msw and remove process.env shim

## 0.0.11

### Patch Changes

- e2189387: fix: default value for opts

## 0.0.10

### Patch Changes

- 1b8b7792: chore: add comment to injected code

## 0.0.9

### Patch Changes

- e2e0bf97: feat: request interceptor

## 0.0.8

### Patch Changes

- 626daf60: feat: bypass sw

## 0.0.7

### Patch Changes

- 1dcec76b: fix: mock rollup plugin

## 0.0.6

### Patch Changes

- 1354dd07: Docs/mocks
- b0d8a907: fix: type: module, and add missing file

## 0.0.5

### Patch Changes

- d952332b: docs: msw

## 0.0.4

### Patch Changes

- 7ef5114f: fix: missing file

## 0.0.3

### Patch Changes

- 6451a7f8: fix: publish correct files

## 0.0.2

### Patch Changes

- 7c27731b: feat: mocks
