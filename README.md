# DBT Models for Airbyte

This directory contains the model used on the airbyte synchronization of the Hasura Database/

## Usage

To use this repo, a `profiles.yml` with the data warehouse credentials must be in the directory `$HOME/.dbt/` of the user, or its path has to be indicated with `--profile-dir`.


This directory requires the package [dbt-postgres](https://docs.getdbt.com/docs/core/connect-data-platform/postgres-setup).

The following commands can be used :

- To build the project : `dbt build`
- To run the project : `dbt run`
- To test the project: `dbt test`

### development

Each new models can be test on the `test` environment of  [infra-bi](https://github.com/status-im/infra-bi) by merging it into the `test` branch of this repo. Once the tests are conclusive, the `test` branch can me merge into the `prod` one.

## Resources:

- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [chat](https://community.getdbt.com/) on Slack for live discussions and support
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices
