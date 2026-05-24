# snapval

> ⚡ Lightweight, type-safe validation library for JavaScript & TypeScript

[![npm version](https://img.shields.io/npm/v/snapval)](https://www.npmjs.com/package/snapval)
[![license](https://img.shields.io/npm/l/snapval)](./LICENSE)
[![types](https://img.shields.io/npm/types/snapval)](https://www.typescriptlang.org/)

---

## Features

- 🔒 Full TypeScript support with inferred types
- 🪶 Zero dependencies, ~2KB minified
- 🔗 Chainable, composable validators
- 💬 Customizable error messages

---

## Installation

```bash
npm install snapval
# or
yarn add snapval
# or
pnpm add snapval
```

---

## Usage

```ts
import { v } from 'snapval'

const schema = v.object({
  name: v.string().min(1),
  age:  v.number().min(0).max(120),
  email: v.string().email(),
})

const result = schema.parse({
  name: 'Alice',
  age: 30,
  email: 'alice@example.com',
})

console.log(result) // { name: 'Alice', age: 30, email: 'alice@example.com' }
```

### Safe parse (no throw)

```ts
const result = schema.safeParse(input)

if (result.success) {
  console.log(result.data)
} else {
  console.error(result.errors)
}
```

---

## API

| Validator | Methods |
|-----------|---------|
| `v.string()` | `.min(n)` `.max(n)` `.email()` `.url()` `.regex(r)` |
| `v.number()` | `.min(n)` `.max(n)` `.int()` `.positive()` |
| `v.boolean()` | — |
| `v.array(schema)` | `.min(n)` `.max(n)` |
| `v.object(shape)` | `.partial()` `.pick(keys)` |
| `v.union(schemas)` | — |
| `v.optional(schema)` | — |

---

## Requirements

- Node.js 16+
- TypeScript 4.7+ (optional)

---

## Contributing

```bash
git clone https://github.com/your-org/snapval
cd snapval
npm install
npm test
```

Pull requests are welcome! Please open an issue first for major changes.

---

## License

[MIT](./LICENSE)
