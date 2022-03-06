# Inline SQL

![python](docs/py_lint.png)

Highlight and lint inline SQL strings. Supported languages are **Python**, **Go**, **JavaScript**, **TypeScript**, **Ruby**, **Java**, **C#**.

Syntax highlighting works for strings starting with `--sql` or any of the `SELECT `, `INSERT `, `INTO `, `DELETE `, `UPDATE `, `CREATE TABLE `. Linting and diagnostics powered entirely by awesome [joereynolds/sql-lint](https://github.com/joereynolds/sql-lint) and works for multiline strings that start with `--sql`. Integration with real database is available and controlled through VSCode options:

```json
{
    "inlineSQL.enableDBIntegration": true,
    "inlineSQL.dbDriver": "postgres",
    "inlineSQL.dbHost": "localhost",
    "inlineSQL.dbPort": 5432,
    "inlineSQL.dbUser": "postgres",
    "inlineSQL.dbPassword": "postgres"
}
```

## Examples

**Python**

![python](docs/py_lint.png)

**JavaScript/TypeScript**

![js](docs/js_lint.png)

**Go**

![go](docs/go_lint.png)

![go](docs/go_lint2.png)


## More syntax highlighting examples

<table style="width:100%; border: none!important;">
  <tr>
    <td>Python</td>
    <td>JavaScript/TypeScript</td>
  </tr>
  <tr>
    <td><img src="docs/python.png" /></td>
    <td><img src="docs/js.png" /></td>
  </tr>
</table>

<table style="width:100%; border: none!important;">
  <tr>
    <td>Ruby</td>
    <td>Java</td>
  </tr>
  <tr>
    <td><img src="docs/ruby.png" /></td>
    <td><img src="docs/java.png" /></td>
  </tr>
</table>

<h3 style="text-align:center;">Go</h3>

![go example](docs/go.png)

Currently gopls semantic token highligting (option `gopls.ui.semanticTokens` -  off by default) overrides extention's syntax. If anyone knows how to fix this, please share.
