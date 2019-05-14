# typescript-eslint-no-unnecessary-type-assertion-undefined
https://github.com/typescript-eslint/typescript-eslint/issues/529
## Steps
1. Run `npm install` or `yarn`
2. Run `npm run typecheck` or `yarn typecheck` -> no errors
3. Run `npm run lint` or `yarn lint`
```
D:\Projects\typescript-eslint-no-unnecessary-type-assertion-undefined\index.ts
  4:5  error  This assertion is unnecessary since the receiver accepts the original type of the expression  @typescript-eslint/no-unnecessary-type-assertion

✖ 1 problem (1 error, 0 warnings)
  1 error and 0 warnings potentially fixable with the `--fix` option.
```
4. Run `npm run fix` or `yarn fix`
5. Run `npm run typecheck` or `yarn typecheck`
```
index.ts:4:5 - error TS2345: Argument of type 'string | null' is not assignable to parameter of type 'string | undefined'.
  Type 'null' is not assignable to type 'string | undefined'.

4 foo(str);
      ~~~


Found 1 error.
```