# ckb-tests

## How to update assets?

Example: update consensus/insufficient_reward.json

- Open file test/src/specs/consensus/insufficient_reward.rs in ckb
- Switch to the commented `run` function
- Run a single integration test: `make CKB_TEST_ARGS='insufficient_reward' integration`
- The new assets file is exported as `test/${backup}/ckb_integration_test.json`. Use it to overwrite consensus/insufficient_reward.json and send the PR to this repository.
