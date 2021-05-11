# Veturpack

A Vue project with minimal setup and dependencies for reproducing [vetur#2898](https://github.com/vuejs/vetur/issues/2898) and [vue-next#3760](https://github.com/vuejs/vue-next/issues/3760).

## Usage

- Install latest version of [Vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur)
- `git clone git@github.com:octref/veturpack.git`
- `cd veturpack`
- `yarn install`
- `code .`

## Things to Try

- Set `"strict": true` in the tsconfig that manages the vue file in question.
- Create a function callback signature type to use as a prop type
- Add a prop whose type is `Function` and default is `null`
- Augment the function type with a `PropType` that includes your custom callback signature and `null`
- Observe error

## License

MIT
