[![Test](https://github.com/snow-actions/composite-action-template/actions/workflows/test.yml/badge.svg)](https://github.com/snow-actions/composite-action-template/actions/workflows/test.yml)

# Create a Composite Action

Use this template to bootstrap the creation of a [composite action](https://docs.github.com/en/actions/creating-actions/creating-a-composite-action).:rocket:

This template includes tests, a validation workflow and versioning guidance.  

## Create an action from this template

Click the `Use this Template` and provide the new repo details for your action.

See the [documentation](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)

## Change action.yml

The action.yml defines the inputs and outputs for your action.

Update the action.yml with your name, description, inputs, outputs and branding for your action.

See the [documentation](https://help.github.com/en/articles/metadata-syntax-for-github-actions).

## Change the Code

The action.yml also defines the steps for your action.

Update the action.yml with your steps for your action.

## Test

Test is written in [test.yml](.github/workflows/test.yml).

You can use `test`, `[`, `[[` and `((` commands for asserting on bash.

Be aware that `[` and `[[` with single line need to be enclosed in `''` or `""` on YAML.

```yaml
- run: test "${GREET}" = "Hello World"
- run: '[ "${GREET}" = "Hello World" ]'
- run: '[[ "${GREET}" == "Hello World" ]'
- run: (( ${NUMBER} == 1 ))
```

## Validate

You can now validate the action by referencing `./` in a workflow in your repo (see [test.yml](.github/workflows/test.yml))

```yaml
- uses: ./
  with:
    who-to-greet: World
```

See the [actions tab](https://github.com/actions/composite-action-template/actions) for runs of this action! :rocket:

## Usage

After testing you can [create a v1 tag](https://github.com/actions/toolkit/blob/master/docs/action-versioning.md) to reference the stable and latest V1 action

## Other official action templates

- [actions/javascript-action](https://github.com/actions/javascript-action)
- [actions/typescript-action](https://github.com/actions/typescript-action)
- [actions/container-action](https://github.com/actions/container-action)
