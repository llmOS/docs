# OpenCopilot docs

This repository holds the MDX-formatted [OpenCopilot docs](https://docs.opencopilot.dev).

The below sections are starter instructions from the Mintlify starter [template](https://github.com/mintlify/starter).

### 👩‍💻 Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify) to preview the documentation changes locally. To install, use the following command

```
npm i -g mintlify
```

Run the following command at the root of your documentation (where mint.json is)

```
mintlify dev
```

### 😎 Publishing Changes

Changes will be deployed to production automatically after pushing to the default branch.

You can also preview changes using PRs, which generates a preview link of the docs.

#### Troubleshooting

- Mintlify dev isn't running - Run `mintlify install` it'll re-install dependencies.
- Page loads as a 404 - Make sure you are running in a folder with `mint.json`

### OpenAPI

1. Copy new `openapi.json` file into this repo
2. `npx @mintlify/scraping@latest openapi-file openapi.json -o api-reference`
3. Copy-and-replace the "navigation object suggestion" into `mint.json` file.