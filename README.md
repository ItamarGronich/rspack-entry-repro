### Reproduction repo for the entry bug in Rspack

Rspack doesn't consider `resolve.extensions` when loading default entry

to reproduce just install and run `npm run dev` or `npm run build`

#### Expected behavior
Rspack should detect the `./src/index.tsx` file as the entry point.

#### Actual behavior
Rspack search for the `./src/index.js` file as the entry point but fails to find it.

probably need to consider `resolve.extensions` when loading default entry
