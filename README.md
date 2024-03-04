# Table of Contents

- [About Repo](#about-pr-viewer)

# About PR-viewer

At the time of this repo creation, there is not a way to see your pull requests across Github.

This PR viewer will bring in current logged in GitHub user's PRs across their organizations, metrics, searching by org, repo, etc.

## Dashboard Display Requirements

The following items are display requirements:

- organization name (and link)
- repo name (and link)
- PR# (and link)
- PR description
- PR status (e.g.: draft, waiting approval, closed, etc)
- reviewer(s)
- submission date
- submitted by (and link to their profile)
- last edited date
- last edited by (and link to their profile)
- issues tied to PR
- other linked PRs (shich show description when you hover)

# Acceptance Criteria

## Must Have

These are the basic items required for this project.

1. GitHub API integration to gather required information (see [dashboard Display Requirements](#dashboard-display-requirements)) on all repos from all orgs under the logged in user (POC will use a token that is manually provided upon accessing the site)

2. "Website" will be hosted via GuitHub pages. For POC (or until we have a way to authenticate the logged in user) there will be a place to paste the required API token.

3. Be able to filter from organization down to repos.

Need to determine what will happen on the site if the token is bad or user doesn't exist ... somehow ...

## Nice To Have

These items are not required for POC (proof of concept) but are a long term vision for this project.

1. Use single sign on or some similar technology that will confirm they are logged in locally on GitHub, which will allow for the automated pull of information

2. Be able to filter based on if logged in user created or is a reviewer

3. Metrics page:
   - number of PRs assigned
   - number of assigned vs total open per repo