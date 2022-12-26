# Lack of Import-mapped Completion Repro

- The `capi.dev` service implements intellisense in accordance with the [Deno LS intellisense API](https://deno.land/manual@v1.29.1/advanced/language_server/imports).
- The `import_map.json` redirects `capi/`-prefixed imports to their `https://capi.dev/@v0.1.0-beta.22/`-prefixed counterparts.
- We get import completions from `https://capi.dev/@v0.1.0-beta.22/`-prefixed imports
- We get no import completions from `capi/`-prefixed imports