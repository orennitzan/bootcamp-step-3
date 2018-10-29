# Risingstart bootcamp-step-3

## Requirements

1. Create one migration file per table (eg. 1-create-user.js, 2-create-repository.js 3-create-contribution.js) with the following skeleton:

   - up method has the logic for the migration, down is for reverting it.
   - The migrations are executed in transactions.
   - The files are executed in alphabetical orde.

2. Add a migrate-db script to the scripts in package.json and corresponding scripts/migrate-db.js file.

## Instalation and Execution

1. git clone <https://github.com/orennitzan/bootcamp-step-3.git>
2. Change directory to **bootcamp-step-3**
3. Run npm test. Expect to pass 2 new tests defined in models/github-api/api.test.js
4. Please note that in this file you will find 2 test that are based on nock and 4 (commented) tests that atually using github api service that should work too. Also note that nock tests are defined widh .persist() option in order to prevent them from failing the calls to the api itself. See: <https://github.com/nock/nock#persist> for more information.
