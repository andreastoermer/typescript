## TypeScript Compiler for Meteor

TypeScript files are compiled into ES5 and CommonJS modules by default.

Default compiler options as JSON:

```json
{
  "module": "commonjs",
  "target": "es5",
  "moduleResolution": "node",
  "experimentalDecorators": true,
  "emitDecoratorMetadata": true,
  "sourceMap": true
}
```

## Package Structure

This package uses (directly or indirectly) three other packages, which are worth to mention:

[typescript-compiler](https://github.com/barbatus/typescript-compiler) - exports a Meteor TypeScript compiler that implements Meteor compiler API. TypeScript compiler in its turn uses [meteor-typescript](https://github.com/barbatus/meteor-typescript) package’s API
to compile TypeScript source code incrementally on file changes.

[typescript-runtime](https://github.com/barbatus/typescript-runtime) - currently contains TypeScript helpers,
which allow to configure behavior of some parts of the compiled TypeScript code for special use cases. One of the use cases is usage with the old browsers.

## Credits

Thanks @barbatus for barbatus:typescript, which this package is based on, even as far as copying some parts.
Adornis doesn't claim any ownership of this code, we have merely taken over the repository after fruitless attempts to contact barbatus.
We love you, if you want to take this repo back, contact @yorrd.

## License

MIT
