# Telegraf Snipgram

Download this extension from the [Visual Studio Code Marketplace](https://marketplace.visualstudio.com/items/gramlify.telegraf-snipgram)

## Usage

Here's the full list of all the snippets:

### [tfs] Telegraf Starter

```ts
const { Telegraf } = require("telegraf");

const app = new Telegraf();

app.launch();

process.once("SIGINT", () => app.stop("SIGINT"));
process.once("SIGTERM", () => app.stop("SIGTERM"));
```

### [tfsm] Telegraf Starter ESM

```ts
import { Telegraf } from "telegraf";

const app = new Telegraf();

app.launch();

process.once("SIGINT", () => app.stop("SIGINT"));
process.once("SIGTERM", () => app.stop("SIGTERM"));
```

### [tfc] Telegraf Command

```ts
app.command("", (ctx) => {
  // your code here
});
```

### [tfca] Telegraf Command Asynchronous

```ts
app.command("", async (ctx) => {
  // your code here
});
```

### [tfn] Telegraf On Something

```ts
app.on("", (ctx) => {
  // your code here
});
```

### [tfna] Telegraf On Something Asynchronous

```ts
app.on("", async (ctx) => {
  // your code here
});
```

### [tfntxt] Telegraf On Text

```ts
app.on("text", (ctx) => {
  // your code here
});
```

### [tfntxta] Telegraf On Text Asynchronous

```ts
app.on("text", async (ctx) => {
  // your code here
});
```

### [tfncq] Telegraf On Callback Query

```ts
app.on("callback_query", (ctx) => {
  // your code here
});
```

### [tfncqa] Telegraf On Callback Query Asynchronous

```ts
app.on("callback_query", async (ctx) => {
  // your code here
});
```

### [tfniq] Telegraf On Inline Query

```ts
app.on("inline_query", (ctx) => {
  // your code here
});
```

### [tfniqa] Telegraf On Inline Query Asynchronous

```ts
app.on("inline_query", async (ctx) => {
  // your code here
});
```

### [tfbs] Telegraf Base Scene

```ts
const someScene = new Scenes.BaseScene<Scenes.SceneContext>("some");
someScene.enter((ctx) => {
  // your code here
});
```

### [tfbsa] Telegraf Base Scene Asynchronous

```ts
const someScene = new Scenes.BaseScene<Scenes.SceneContext>("some");
someScene.enter(async (ctx) => {
  // your code here
});
```

### [tfsbs] Telegraf Stage Base Scene

```ts
const stage = new Scenes.Stage<Scenes.SceneContext>([]);
```

### [tfsbst] Telegraf Stage Base Scene With TTL

```ts
const stage = new Scenes.Stage<Scenes.SceneContext>([], {
  ttl: 10,
});
```

### [tfws] Telegraf Wizard Scene
```ts
const someWizard = new Scenes.WizardScene(
  "some-wizard",
  (ctx) => {
    // your code here
  }
);
```

### [tfwsa] Telegraf Wizard Scene Asynchronous
```ts
const someWizard = new Scenes.WizardScene(
  "some-wizard",
  async (ctx) => {
    // your code here
  }
);
```

### [tfsws] Telegraf Stage Wizard Scene

```ts
const stage = new Scenes.Stage<Scenes.WizardContext>([], {
  default: "-wizard",
});
```

### [tfwsrn] Telegraf Return Wizard Scene Next

```ts
return ctx.wizard.next();
```

### [tc] [tfctx] Telegraf CTX

```ts
(ctx) => {
  // your code here
};
```

### [tca] [tfctxa] Telegraf CTX Asynchronous

```ts
async (ctx) => {
  // your code here
};
```
