---
layout: default
title: CHANGELOG
nav_order: 80
---

Changelog
===

> This changelog **doesn't follow Semantic Versioning**.

- We upgrade the **major** version when adding a new preset that changes how Next apps are meant to be used/built, resulting in a non-trivial **redesign of the NRN base code**.
  - Such as the big SSG change in Next.js v9.3 release, which uses a completely different paradigm

This changelog is meant to provide a good overview of the biggest changes in the NRN project,
such as a preset release history, but it is not meant to warn about non-backward compatible changes within presets.

---

## Want to subscribe?

[Subscribe to the discussion](https://github.com/UnlyEd/next-right-now/discussions/166) to be notified when new releases are made, and participate in the discussion about what has changed!

---

## Changes across presets

### Most valuable changes

Here is a short list of the most valuable changes and new features.

- 2021-06-15
    - [NextJS 11](https://github.com/UnlyEd/next-right-now/pull/371)
- 2021-06-09
    - [Send network speed to Amplitude analytics and Sentry](https://github.com/UnlyEd/next-right-now/pull/358)
    - [Improve HTTP headers security by default](https://github.com/UnlyEd/next-right-now/pull/364)
    - [Use main, footer, nav and their ARIA equivalent for better a11y](https://github.com/UnlyEd/next-right-now/pull/365)
    - [Optimize .vercelignore configuration](https://github.com/UnlyEd/next-right-now/pull/366)
- 2021-05-29
    - [Fix 404 page generation + refactor all layouts SSG/SSR](https://github.com/UnlyEd/next-right-now/pull/346)
    - [Upgrade Cypress to v7](https://github.com/UnlyEd/next-right-now/pull/327)
- 2021-05-20
    - [Preload app-wide shared data](https://github.com/UnlyEd/next-right-now/pull/334)
    - [Pre-fetch all Locize translations as app-wide static data](https://github.com/UnlyEd/next-right-now/pull/337)
    - [Enable react strict mode](https://github.com/UnlyEd/next-right-now/pull/340)
- 2021-05-20
    - [Improve 404 page detection (covers more use-cases) + Don't serve pages under a locale that hasn't been enabled](https://github.com/UnlyEd/next-right-now/pull/333)
- 2021-05-13
    - [Fix - Display deployment's aliases on PR (regression from #296)](https://github.com/UnlyEd/next-right-now/pull/318)
- 2021-05-12
    - [Upgrade dependencies](https://github.com/UnlyEd/next-right-now/pull/328)
    - [Simplify layouts](https://github.com/UnlyEd/next-right-now/pull/330)
- 2021-05-10
    - [Rework of fonts](https://github.com/UnlyEd/next-right-now/pull/315)
    - [Optimise cookieConsent to avoid rendering on each page transition](https://github.com/UnlyEd/next-right-now/pull/319)
- 2021-05-09
    - [GHA - Replace Vercel bash deploy script by "deploy-on-vercel" github action](https://github.com/UnlyEd/next-right-now/pull/296)
    - [Replace @unly/utils-simple-logger and winston by @unly/simple-logger and chalk (reduces bundle size by 40Kb)](https://github.com/UnlyEd/next-right-now/pull/314)
    - [Upgrade to Next.js v10.2](https://github.com/UnlyEd/next-right-now/pull/313)
- 2021-01-24
    - [Feature - Automatically release Vercel deployments as GitHub deployments](https://github.com/UnlyEd/next-right-now/pull/280)
    - [Optimize GitHub Actions triggers](https://github.com/UnlyEd/next-right-now/pull/282)
- 2021-01-20
    - [(MAJOR) Massive folder structure refactoring (`v2-mst-aptd-at-lcz-sty`), using modular approach and module path aliases](https://github.com/UnlyEd/next-right-now/pull/264)
    - [(MAJOR) Massive folder structure refactoring (`v2-mst-aptd-gcms-lcz-sty`), using modular approach and module path aliases](https://github.com/UnlyEd/next-right-now/pull/275)
- 2021-01-17
    - [Add Storybook static site, hosted on Vercel](https://github.com/UnlyEd/next-right-now/pull/251)
- 2021-01-13
    - [Improve Sentry monitoring for all pages + improve bootstrap error handling and monitoring](https://github.com/UnlyEd/next-right-now/commit/7fd4523e59528dfaaf418b601a3830559360c9d4)
    - [Improve demo about error handling](https://github.com/UnlyEd/next-right-now/commit/d00f799c11ddf5cdc4cd17c56d5f0d19569d2629)
- 2021-01-11
    - [Implement restore-variable to clean our actions](https://github.com/UnlyEd/next-right-now/pull/239)
    - [Deps - Upgrade `v2-mst-aptd-at-lcz-sty` packages (January 2021)](https://github.com/UnlyEd/next-right-now/pull/245)
    - [Deps - Upgrade `v2-mst-aptd-gcms-lcz-sty` packages (January 2021)](https://github.com/UnlyEd/next-right-now/pull/246)
    - [Deps - Upgrade to Emotion v11 (from v10) [BREAKING CHANGES]](https://github.com/UnlyEd/next-right-now/pull/247)
- 2021-01-09
    - [Documentation update](https://github.com/UnlyEd/next-right-now/pull/238)
- 2020-12-30
    - [Handle GitHub private repositories](https://github.com/UnlyEd/next-right-now/pull/236)
    - [Invoke custom webhook url once a Vercel deployment is "completed"](https://github.com/UnlyEd/next-right-now/pull/235)
- 2020-12-22
    - [DevOps - Resolve app version from git tags, instead of package.json](https://github.com/UnlyEd/next-right-now/pull/234)
- 2020-12-19
    - [Await Vercel deployment to be ready before running E2E](https://github.com/UnlyEd/next-right-now/pull/221)
    - [Provide in api/status the git commit metadata (SHA/branch/tag) used to make a Vercel deployment](https://github.com/UnlyEd/next-right-now/pull/225)
    - [Add an action that releases automatically when a change lands on the main branches](https://github.com/UnlyEd/next-right-now/pull/227) + various fixes regarding auto-releasing (WIP)
        - From now on, Next Right Now automatically creates tags and releases. This was WIP at the time, but has been improved by the end of 2020.
- 2020-11-21
    - [Update documentation about ENV vars](https://github.com/UnlyEd/next-right-now/pull/215)
    - [Improve LightHouse performances](https://github.com/UnlyEd/next-right-now/pull/214)
    - [Migrated "now" and "Zeit" to "vercel"](https://github.com/UnlyEd/next-right-now/issues/181)
        - GitHub Actions now uses `vercel` CLI instead of `now` which will be deprecated by the end of 2020
    - [GHA - Update cypress-io/github-action from v1 to v2 to fix CI/CD due to ::set-env security issue](https://github.com/UnlyEd/next-right-now/pull/209)
        - This fixes a recurring crash for all GH Actions since `::set-env` support has been dropped by GitHub about a week ago (was mostly affecting Cypress Action)
- 2020-10-21
    - [GHA - Auto-alias custom domains](https://github.com/UnlyEd/next-right-now/pull/185)
- 2020-10-20
    - [GHA - Enable Cypress debug logs for CPU/Memory usage by default](https://github.com/UnlyEd/next-right-now/commit/383862e34d288f5a435b921fd4b1a2ba89b3254f)
    - Allow triggering workflows manually through [GitHub Actions page](https://github.com/UnlyEd/next-right-now/actions)
        - Wasn't possible before because there weren't any workflows [in the main branch](https://github.com/UnlyEd/next-right-now/tree/gh-pages/.github/workflows)
          (`gh-pages`) - See https://github.community/t/cant-trigger-workflow-manually/121740/53?u=vadorequest
- 2020-10-18
    - [Improve GHA - Do not crash Github build when Vercel aliasing fails](https://github.com/UnlyEd/next-right-now/pull/180)
- 2020-10-17
    - [Manual & remote (HTTP) deployments through GitHub UI/API](https://github.com/UnlyEd/next-right-now/pull/147)
- 2020-10-08
    - [Added new example with **optional `catch-all` routes**](https://github.com/UnlyEd/next-right-now/pull/162)
- 2020-09-08
    - [Upgraded deps of `v2-mst-aptd-at-lcz-sty` preset](https://github.com/UnlyEd/next-right-now/pull/163)
    - [Upgraded deps of `v2-mst-aptd-gcms-lcz-sty` preset](https://github.com/UnlyEd/next-right-now/pull/165)
- 2020-09-07
    - [Improved the NRN docs](https://github.com/UnlyEd/next-right-now/pull/160)
    - [Migrated all `v2` presets from `v9.4.4` to Next.js `v9.5.4-canary.4`](https://github.com/UnlyEd/next-right-now/pull/161)
- 2020-07-28
    - [GDPR - Add cookie consent UI](https://github.com/UnlyEd/next-right-now/pull/140)
- 2020-07-21
    - [GDPR - Disable Google Click ID being used by default](https://github.com/UnlyEd/next-right-now/pull/138)
- 2020-07-20
    - Documentation updates of CHANGELOG and ROADMAP pages
- 2020-07-16
    - [Change NRN app publication workflow](https://github.com/UnlyEd/next-right-now/pull/129) for all `v2` presets
- 2020-06-25
    - [Allow custom i18n translations per customer](https://github.com/UnlyEd/next-right-now/pull/118) for all `v2` presets
- 2020-06-16
    - [Allow converting Markdown to JSX at runtime](https://github.com/UnlyEd/next-right-now/pull/113) for all `v2-*-at` presets (Airtable)
- 2020-06-12
    - [Automatically run LightHouse on PR commits (CI)](https://github.com/UnlyEd/next-right-now/pull/103) for all `v2` presets
    - [Added "item preview" feature, allowing to preview a NRN record from Stacker CMS](https://github.com/UnlyEd/next-right-now/pull/105) for all `v2-*-at` presets (Airtable)
        - _This feature has been renamed "Quick preview" since then_
- 2020-06-08
    - [Add jest-runner-groups to run tests by group](https://github.com/UnlyEd/next-right-now/pull/91) for all `v2` presets
- 2020-06-06
    - [Add hybrid memory/disk cache storages to optimise Airtable API data fetching during server initial build](https://github.com/UnlyEd/next-right-now/pull/92) for all `v2` presets
        - This will eventually be moved out of NRN and released as a NPM package
- 2020-06-06
    - [Use .env instead of .env.build file](https://github.com/UnlyEd/next-right-now/pull/77) for all `v2` presets
- 2020-05-31
    - [Implement preview mode](https://github.com/UnlyEd/next-right-now/pull/70) for all `v2` presets
        - _This feature [has been changed since](https://github.com/UnlyEd/next-right-now/pull/129), to allow "Preview mode" to be used only for the staging environment_


### Changes workflow

> `v2-mst-aptd-at-lcz-sty` and `v2-mst-aptd-gcms-lcz-sty` are both kept up-to-date. Changes that aren't specific to one preset are applied to both.

To see an exhaustive list of changes (added across presets), check out the [merged PR](https://github.com/UnlyEd/next-right-now/pulls?q=is%3Apr+sort%3Aupdated-desc+is%3Amerged).

Most changes are merged through PRs, for easier reviews.

*I basically don't have the time to keep a documented version of what's included in each preset branch (too much work).*

*If you want to know what's included within each preset, the easiest way is to review which commits are included in those presets.*

---

## Presets releases

- 2020-07-16 (v2)
    - Released [`v2-mst-aptd-at-lcz-sty`](https://github.com/UnlyEd/next-right-now/tree/v2-mst-aptd-at-lcz-sty) preset - [PR](https://github.com/UnlyEd/next-right-now/pull/131)
        - Very similar to [`v2-mst-aptd-gcms-lcz-sty`](https://github.com/UnlyEd/next-right-now/tree/v2-mst-aptd-gcms-lcz-sty) preset
        - Brings a much better CMS vendor (Stacker) for manipulating database content
            - This replaces our [NRN-Admin OSS project](https://github.com/UnlyEd/next-right-now-admin) (based on React Admin) which hasn't yielded the expected result
        - Use GraphCMS vendor instead of Airtable vendor (database)
        - Features advanced use-cases with embedded previews from CMS to NRN app
            - Basically, allows to preview a record on Stacker CMS using iframes hosted on NRN app
        - Features advanced [Markdown to JSX runtime transform](https://github.com/UnlyEd/next-right-now/discussions/99) for storing React components within Airtable
    - Changed default preset from `v2-mst-aptd-gcms-lcz-sty` to `v2-mst-aptd-at-lcz-sty`
- 2020-02-30 (v2)
    - New major version v2 due to complete refactoring of the whole NRN app (due to Next 9.3/9.4 which completely changed the way to build apps and added the SSG rendering mode)
    - Released [`v2-mst-aptd-gcms-lcz-sty`](https://github.com/UnlyEd/next-right-now/tree/v2-mst-aptd-gcms-lcz-sty) preset
        - Uses Next v9.4+
        - Supports hybrid SSG/SSR rendering modes
        - New NRN demo and showcase many more examples - See [#45](https://github.com/UnlyEd/next-right-now/issues/45)
    - Changed default preset from `v1-ssr-mst-aptd-gcms-lcz-sty` to `v2-mst-aptd-gcms-lcz-sty`
- 2020-02-28 (v1)
    - New major version v1
    - Released [`v1-ssr-mst-aptd-gcms-lcz-sty`](https://github.com/UnlyEd/next-right-now/tree/v1-ssr-mst-aptd-gcms-lcz-sty) preset
        - Uses Next v9.3.4
        - Doesn't support SSG, only supports SSR

---

<div class="pagination-section space-even">
    <span class="fs-4" markdown="1">
    [TESTIMONIALS](./testimonials){: .btn .btn }
    </span>
    <span class="fs-4" markdown="1">
    [FAQ](./faq){: .btn .btn }
    </span>
    <span class="fs-4" markdown="1">
    [CONTRIBUTING](./contributing){: .btn .btn }
    </span>
</div>
