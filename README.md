## Getting Started

First, generate the static html output:

```bash
npm run build
```
# or
```bash
yarn build
```
# or
```bash
pnpm build
```
Once complete, we should see an /out directory. It contains the bundled version of our Next.js application as well as our manifest.json. Think of this directory as the source code of our extension.

We’ve now successfully prepared our Next.js application to be embedded within an extension! Our last step is to simply import it into the browser to test:

Firefox:
- Navigate to: about:debugging#/runtime/this-firefox
- Click the ‘Load Temporary Add-on…’ button.
- Select your manifest.json file.

To check the static html out in browser:
```bash
npx serve@latest out
```
