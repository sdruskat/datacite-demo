# datacite-demo

HERMES demo repository for the DataCite webinar `DOIs for Research Software: Increasing Visibility, Connectivity, Citability`.

## Publication history

This repository has been published automatically with a GitHub Actions continuous integration workflow running `hermes`.

The way this has worked was:

1. A [commit](https://github.com/sdruskat/datacite-demo/commit/c23d4c63adb0f91546a5dbbf6ed684c6a223a500) was pushed to the `main` branch.
2. [`hermes`](https://github.com/hermes-hmc/workflow/) harvested and processed metadata from git history and the [CFF file](CITATION.cff), and created a [pull request for curating](https://github.com/sdruskat/datacite-demo/pull/7) these metadata.
3. The metadata was accepted for publication and the pull request was merged.
4. `hermes` then [made](https://github.com/sdruskat/datacite-demo/actions/runs/5066268290) the publication on Zenodo Sandbox (https://sandbox.zenodo.org/record/1205714) and postprocessed the metadata to update the `hermes` configuration.
5. It created a [second pull request to integrate the Zenodo Sandbox publication record id](https://github.com/sdruskat/datacite-demo/pull/8) in the HERMES configuration, so that future releases would be published under the same concept record.
