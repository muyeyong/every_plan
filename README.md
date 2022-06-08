# Create Daily plan Issue Action

automatic create daily plan issue for muyeyong/every-plan

## Inputs

## `token`

**Required** github token.

## Example usage

uses: muyeyong/create-daily-plan-issue-action@main

with:
token: 'github token'

```js
jobs:
  create_daily_plan_issue:
    runs-on: ubuntu-latest
    name: create daily plan issue
    steps:
      - name: Checkout
        uses: actions/checkout@v2
      - name: create daily plan issue action step
        uses: muyeyong/create-daily-plan-issue-action@main
        env:
          TOKEN: ${{ secrets.TOKEN }}
        with:
          token: ${{env.TOKEN}}
```
