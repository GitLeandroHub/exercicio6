## Exercise Six

1. Fork & clone this project
2. Add new tests for `fn set_price` and `fn buy`
    - [./pallets/kitties/src/tests.rs](./pallets/kitties/src/tests.rs#L201)
    - Make sure you have covered happy paths, error paths and edge cases
3. Update test for `fn transfer` to check the updated behaviour regards to KittyPrices
    - [./pallets/kitties/src/tests.rs](./pallets/kitties/src/tests.rs#L167)
4. Run benchmark related commands and see if the output makes sense
    - `make benchmark`
    - `make benchmark-output`
    - `make benchmark-traits`