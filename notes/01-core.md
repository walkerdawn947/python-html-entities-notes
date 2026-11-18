# Decode HTML entities: implementation

## What the example does

unescape decodes named and numeric references. Decoded output may contain markup and must be escaped again before insertion into HTML.

The public function is `solve(value)`. The JSON input contract can be seen in this concrete example:

```json
"Tom &amp; Ada"
```

Expected result:

```json
"Tom & Ada"
```

Run `python3 example.py` for the Python representation of the result. `solution.py` contains the full implementation and can also be imported by another script.

## Scope

The function implements exactly the behavior described above. It does not perform network or filesystem access. Python exceptions indicate unsupported input; the next lesson turns them into a command-line error response. Review the limitations before reusing it in an application.
