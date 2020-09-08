# Live Reload

Live Reload is a server watcher, written in Deno, for TypeScript and JavaScript
that will reload the server when it detects a change in
any TypeScript or JavaScript file.

## Usage

To use Live Reload, first have Deno installed, and then use a terminal and write:

```bash
deno run -A https://deno.land/x/live_reload@0.0.3/reload.ts --main=main.ts
```

Note that the argument for --main should be the main module for the server.
Also the main module can also be a .js file too.
