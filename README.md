# Welcome to the OpenSanctions crawler planning repository!

This is where we coordinate implementing crawlers - the open source code which takes data from various sources, converts it to our data model, and adds it to our database for use in screening and investigations.

We have a contracted team who helps us keep on top of demand and our data coverage goals. If you're [interested in joining, let us know](https://www.opensanctions.org/docs/company/jobs/crawler-team/)!

We also welcome volunteer open source contributions, but recommend that you first take a look at the project board and [chat with us](https://www.opensanctions.org/contact/) to discuss the most appropriate next crawler to add. We'll then handle the movements on the project board described below on your behalf.

## New data source suggestions

Suggestions for data sources can be added by [submitting an issue](https://github.com/opensanctions/crawler-planning/issues/new/choose) in this repository. But please have a quick little [search](https://github.com/opensanctions/crawler-planning/issues) to see if someone else has already suggested the same source.

We review submissions and queue them for addition if/when they meet our [data inclusion criterea](https://www.opensanctions.org/docs/criteria/).

## Getting started on the team

We will assign your first task on the [project board](https://github.com/orgs/opensanctions/projects/2) which we'll pick to be a nice introductory task.

Your next step is to dive into the [instructions to get started with zavod](https://zavod.opensanctions.org/), our ETL framework, and see if you can get a crawler working.

## Workflow

The **Todo column** is ordered in decreasing priority.

When you're ready to start your next task, take the next top card in the **Todo column** and move it to the **In Progress column**. Add yourself as an assignee, if we haven't already done so.

When you feel your new/modified crawler is ready for production, 
  - create a pull request to the [opensanctions](https://github.com/opensanctions/opensanctions) repository with your branch
  - [link your pull request to the card issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue)
  - move the card to the **In Review column**.

If it's ready
  - we'll add it to the appropriate collection
  - we'll merge it
  - we'll move it to the **Done column**
  - it will be deployed automatically, and run according to its schedule.

If some changes are needed, we'll comment on the pull request, and move it back to to the **In Progress column** for you to revise.

Please try to finish any work in progress before starting anything new.

## Kinds of crawlers, sources, or data

Crawlers generally bring one type of [target](https://www.opensanctions.org/docs/glossary/#targets) into our database, and tasks are annotated to indicate the type:

- `crime-list` - crime-linked entities
- `sanctions-list` - sanctioned entities
- `pep-list` - Politically exposed persons

Each kind of target should be [annotated according to our data model](https://www.opensanctions.org/docs/topics/).
