# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `esprima > invalid-syntax > migrated_0051`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: true
	directives: Array []
	filename: "esprima/invalid-syntax/migrated_0051/input.js"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "esprima/invalid-syntax/migrated_0051/input.js"
		end: Object {
			column: 0
			line: 2
		}
		start: Object {
			column: 0
			line: 1
		}
	}
	diagnostics: Array [
		Object {
			origins: Array [Object {category: "parse/js"}]
			description: Object {
				advice: Array []
				category: "parse/js"
				message: MARKUP {parts: Array [RAW_MARKUP {value: "Bad character escape sequence"}]}
			}
			location: Object {
				filename: "esprima/invalid-syntax/migrated_0051/input.js"
				mtime: undefined
				sourceText: undefined
				end: Object {
					column: 3
					line: 1
				}
				start: Object {
					column: 3
					line: 1
				}
			}
		}
	]
	body: Array [
		JSExpressionStatement {
			loc: Object {
				filename: "esprima/invalid-syntax/migrated_0051/input.js"
				end: Object {
					column: 6
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			expression: JSReferenceIdentifier {
				name: "\0"
				loc: Object {
					filename: "esprima/invalid-syntax/migrated_0051/input.js"
					identifierName: "\0"
					end: Object {
						column: 6
						line: 1
					}
					start: Object {
						column: 0
						line: 1
					}
				}
			}
		}
		JSExpressionStatement {
			loc: Object {
				filename: "esprima/invalid-syntax/migrated_0051/input.js"
				end: Object {
					column: 7
					line: 1
				}
				start: Object {
					column: 6
					line: 1
				}
			}
			expression: JSReferenceIdentifier {
				name: "INVALID_PLACEHOLDER"
				loc: Object {
					filename: "esprima/invalid-syntax/migrated_0051/input.js"
					end: Object {
						column: 7
						line: 1
					}
					start: Object {
						column: 6
						line: 1
					}
				}
			}
		}
	]
}
```

### `diagnostics`

```

 esprima/invalid-syntax/migrated_0051/input.js:1:3 parse/js ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Bad character escape sequence

    \u{FFZ}
       ^

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```
