# Live Reload

Live Reload is a server watcher, written in Deno, for TypeScript and JavaScript
that will reload the server when it detects a change in
any TypeScript or JavaScript file.

## Usage

To use Live Reload, first have Deno installed, and then use a terminal and write:

```bash
deno run --allow-read --allow-run https://deno.land/x/live_reload@0.0.3/reload.ts --main=main.ts
```

Note that the argument for --main should be the main module for the server.
Also the main module can also be a .js file too.

To restrict permissions, add command line arguments such as allow-net and allow-read.
For example, to restrict the Deno subprocess to only read and net access use:

```bash
deno run --allow-read --allow-run https://deno.land/x/live_reload@0.0.3/reload.ts --main=main.ts allow-net allow-read
```

The list of permission arguments are available [here](https://deno.land/manual/getting_started/permissions).

Note that arguments for permissions leave off the '--' at the beginning of the permission and
having no permisions is interpretted as having all permissions (-A).

To give no permissions use:

```bash
deno run --allow-read --allow-run https://deno.land/x/live_reload@0.0.3/reload.ts --main=main.ts allow-none
```
