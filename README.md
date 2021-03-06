# ESLint Configuration
This package aims at creating universal configurations for ESLint that restricts the coding standards as much as possible. It is inspired but various rules packages but compiles everything into only one, dependency-free package.

## Versions
- `@typescript-eslint/eslint-plugin` - 3.7.1
- `@typescript-eslint/eslint-plugin-tslint` - 3.7.1
- `@typescript-eslint/parser` - 3.7.1
- `codelyzer` - 5.2.3
- `eslint` - 7.6.0
- `eslint-plugin-node` - not implemented yet
- `prettier` - 2.0.5
- `tslint` - 6.1.3

## Rules Details
### Possible Errors
- `getter-return` - disabled - TypeScript
- `no-dupe-args` - disabled - TypeScript
- `no-dupe-keys` - disabled - TypeScript
- `no-extra-parens` - disabled - Prettier, TypeScript
- `no-extra-semi` - disabled - Prettier, TypeScript
- `no-func-assign` - disabled - TypeScript
- `no-import-assign` - disabled - TypeScript
- `no-loss-of-precision` - disabled - TypeScript
- `no-obj-calls` - disabled - TypeScript
- `no-setter-return` - disabled - TypeScript
- `no-unexpected-multiline` - disabled - Prettier
- `no-unreachable` - disabled - TypeScript
- `no-unsafe-negation` - disabled - TypeScript
- `valid-typeof` - disabled - TypeScript

### Best Practices
- `block-scoped-var` - disabled - `no-var`
- `class-methods-use-this` - disabled since we don't want to enforce static members in classes
- `curly` - disabled - Prettier
- `default-param-last` - disabled - TypeScript
- `default-case` - can be omitted locally with `// No Default`
- `dot-location` - disabled - Prettier
- `dot-notation` - disabled - TypeScript
- `no-empty-function` - disabled - TypeScript
- `no-eq-null` - disabled - `eqeqeq`
- `no-extra-label` - disabled - `no-labels`
- `no-floating-decimal` - disabled - Prettier
- `no-implicit-globals` - disabled - `no-var` and using ES6 modules
- `no-invalid-this` - disabled - Angular
- `no-magic-numbers` - disabled - TypeScript
- `no-multi-spaces` - disabled - Prettier
- `no-redeclare` - disabled - `no-var` and TypeScript
- `no-return-await` - disabled - TypeScript
- `no-restricted-properties` - disabled since we don't have anything to restrict
- `no-unused-expressions` - disabled - TypeScript
- `no-unused-labels` - disabled - `no-labels`
- `no-throw-literal` - disabled - TypeScrypt
- `no-warning-comments` - `FIXME` comments will fail builds
- `no-with` - disabled - `strict` and TypeScript
- `require-await` - disabled - TypeScript
- `require-unicode-regexp` - disabled since we don't want to enforce unicode flag in RegEx
- `vars-on-top` - disabled - `no-var`
- `wrap-iife` - disabled - Prettier

### Strict Mode
- `strict` - Strict mode is implied by default but disabled in TypeScript since we use `alwaysStrict` flag in `tsconfig.json`

### Variables
- `init-declarations` - disabled since we don't want to enforce variables initialization, TypeScript
- `no-label-var` - disabled - `no-labels`
- `no-restricted-globals` - disabled since we don't have anything to restrict
- `no-undef` - disabled - TypeScript
- `no-unused-vars` - disabled - `no-var`, ES6 and TypeScript
- `no-use-before-define` - disabled - `no-var`, ES6 and TypeScript

### Stylistic Issues
- `array-bracket-newline` - disabled - Prettier
- `array-bracket-spacing` - disabled - Prettier
- `array-element-newline` - disabled - Prettier
- `block-spacing` - disabled - Prettier
- `brace-style` - disabled - Prettier, TypeScript
- `camelcase` - disabled - TypeScript
- `comma-dangle` - disabled - Prettier
- `comma-spacing` - disabled - Prettier, TypeScript
- `comma-style` - disabled - Prettier
- `computed-property-spacing` - disabled - Prettier
- `consistent-this` - disabled since we use target clean contexts
- `eol-last` - disabled - Prettier
- `func-call-spacing`: disabled - Prettier, TypeScript
- `func-name-matching`: disabled - `func-names`
- `function-call-argument-newline` - disabled - Prettier
- `function-paren-newline` - disabled - Prettier
- `id-blacklist` - disabled since we don't have anything to blacklist
- `id-match` - this should be enabled
- `implicit-arrow-linebreak` - disabled - Prettier
- `indent` - disabled - Prettier, TypeScript
- `jsx-quotes` - disabled - Prettier
- `key-spacing` - disabled - Prettier
- `keyword-spacing` - disabled - Prettier, TypeScript
- `line-comment-position` - disabled since we allow line comments everywhere
- `linebreak-style` - disabled - Prettier
- `lines-around-comment` - disabled - Prettier
- `lines-between-class-members` - disabled - TypeScript
- `max-len` - disabled - Prettier
- `multiline-comment-style` - disabled since we allow both types of multiline comments
- `multiline-ternary` - disabled - Prettier
- `newline-per-chained-call` - disabled - Prettier
- `new-parens` - disabled - Prettier
- `no-array-constructor` - disabled - TypeScript
- `no-inline-comments` - disabled since we allow inline comments
- `no-mixed-operators` - disabled since we don't want to enforce unnecessary parens and Prettier
- `no-mixed-spaces-and-tabs` - disabled - `no-tabs` and Prettier
- `no-multiple-empty-lines` - disabled - Prettier
- `no-negated-condition` - disabled since we allow negated conditions
- `no-restricted-syntax` - disabled since we don't have anything to restrict
- `no-tabs` - disabled - Prettier
- `no-ternary` - disabled since we allow ternary operators
- `no-trailing-spaces` - disabled - Prettier
- `no-whitespace-before-property` - disabled - Prettier
- `nonblock-statement-body-position` - disabled - `curly` and Prettier
- `object-curly-newline` - disabled - Prettier
- `object-curly-spacing` - disabled - Prettier
- `object-property-newline` - disabled - Prettier
- `one-var-declaration-per-line` - disabled - Prettier
- `operator-linebreak` - disabled - Prettier
- `padded-blocks` - disabled - Prettier
- `padding-line-between-statements` - might need adjustments
- `quote-props` - disabled - Prettier
- `quotes` - disabled - Prettier, TypeScript
- `semi` - disabled - Prettier
- `semi-spacing` - disabled - Prettier
- `semi-style` - disabled - Prettier
- `sort-keys` - disabled since we don't want to sort object keys
- `sort-vars` - disabled since we don't want to sort variables
- `space-before-blocks` - disabled - Prettier
- `space-before-function-paren` - disabled - Prettier
- `space-in-parens` - disabled - Prettier
- `space-infix-ops` - disabled - Prettier
- `space-unary-ops` - disabled - Prettier
- `switch-colon-spacing` - disabled - Prettier
- `template-tag-spacing` - disabled - Prettier
- `unicode-bom` - disabled - Prettier
- `wrap-regex` - disabled since we don't want to wrap RegEx expressions and Prettier

### ECMAScript 6
- `arrow-body-style` - disabled - Prettier
- `arrow-parens` - disabled - Prettier
- `arrow-spacing` - disabled - Prettier
- `constructor-super` - disabled - TypeScript
- `generator-star-spacing` - disabled - Prettier
- `no-confusing-arrow` - disabled - Prettier
- `no-const-assign` - disabled - TypeScript
- `no-duple-class-members` - disabled - TypeScript
- `no-new-symbol` - disabled - TypeScript
- `no-restricted-exports` - disabled since there's nothing to restrict
- `no-this-before-super` - disabled - TypeScript
- `no-useless-constructor` - disabled since we use dependency injection and TypeScript
- `prefer-arrow-callback` - disabled - Prettier
- `rest-spread-spacing` - disabled - Prettier
- `sort-imports` - this needs to be adjusted in the future as for the moment the rule can't separate imports via blank lines
- `template-curly-spacing` - disabled - Prettier
- `yield-star-spacing` - disabled - Prettier

### TypeScript
- `@typescript-eslint/brace-style` - disabled - Prettier
- `@typescript-eslint/class-literal-property-style` - disabled since we don't want to enforce a particular style
- `@typescript-eslint/comma-spacing` - disabled - Prettier
- `@typescript-eslint/explicit-module-boundary-types` - disabled since types are enforced on a global level
- `@typescript-eslint/func-call-spacing` - disabled - Prettier
- `@typescript-eslint/indent` - disabled - Prettier
- `@typescript-eslint/init-declarations` - disabled since we don't want to enforce variables initialization
- `@typescript-eslint/keyword-spacing` - disabled - Prettier
- `@typescript-eslint/member-delimiter-style` - disabled - Prettier
- `@typescript-eslint/member-ordering` - this can be improved drastically
- `@typescript-eslint/no-explicit-any` - disabled since we allow any
- `@typescript-eslint/no-extra-parens` - disabled - Prettier
- `@typescript-eslint/no-extra-semi` - disabled - Prettier
- `@typescript-eslint/no-floating-promises` - disabled - Angular
- `@typescript-eslint/no-magic-numbers` - disabled as there are multiple edge cases where this can't be avoided and the code becomes extremely verbose
- `@typescript-eslint/no-unnecessary-condition` - disabled for regular mode, but enabled for strict mode
- `@typescript-eslint/no-unsafe-assignment` - disabled since we allow any
- `@typescript-eslint/no-unsafe-call` - disabled as it is too strict
- `@typescript-eslint/no-unsafe-member-access` - disabled as it is too strict
- `@typescript-eslint/no-unsafe-return` - disabled as it is too strict
- `@typescript-eslint/no-unused-vars` - disabled since this is reported by compiler
- `@typescript-eslint/no-unused-vars-experimental` - disabled since this is reported by compiler
- `@typescript-eslint/no-use-before-define` - disabled since this is reported by compiler
- `@typescript-eslint/no-useless-constructor` - disabled since we use dependency injection
- `@typescript-eslint/prefer-namespace-keyword` - disabled since we don't use namespace
- `@typescript-eslint/prefer-readonly-parameter-types` - disabled since it is very verbose
- `@typescript-eslint/prefer-ts-expect-error` - disabled - `ban-ts-comment`
- `@typescript-eslint/promise-function-async` - disabled - Angular
- `@typescript-eslint/quotes` - disabled - Prettier
- `@typescript-eslint/return-await` - disabled - NestJS
- `@typescript-eslint/semi` - disabled - Prettier
- `@typescript-eslint/space-before-function-paren` - disabled - Prettier
- `@typescript-eslint/type-annotation-spacing` - disabled - Prettier
- `@typescript-eslint/strict-boolean-expressions` - disabled since we want to allow short checks
- `@typescript-eslint/typedef` - this should be updated accordingly

## Inspired by:
- [eslint-config-prettier - 6.11.0](https://github.com/prettier/eslint-config-prettier)
