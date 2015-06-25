# glsl-shader-name

[![stable](http://badges.github.io/stability-badges/dist/stable.svg)](http://github.com/badges/stability-badges)

Extract a shader's name from its source, as specified in
[@spite's ShaderEditorExtension](https://github.com/spite/ShaderEditorExtension/issues/10).

``` glsl
// in plaintext:
#define SHADER_NAME hello world

// or for non-ASCII characters using base64:
#define SHADER_NAME_B64 aGVsbG8gd29ybGQ=
```

This is a simple pattern for identifying otherwise anonymous
shaders in GLSL tooling.

## Usage

[![NPM](https://nodei.co/npm/glsl-shader-name.png)](https://nodei.co/npm/glsl-shader-name/)

### `name = shaderName(src)`

Retrieves the shader name from a GLSL source string `src`.
You may also pass in a list of tokens generated by
[glsl-tokenizer](https://github.com/stackgl/glsl-tokenizer).

## Contributing

See [stackgl/contributing](https://github.com/stackgl/contributing) for details.

## License

MIT. See [LICENSE.md](http://github.com/stackgl/glsl-shader-name/blob/master/LICENSE.md) for details.