# Release Cycle

- Work
- When ready, checkout `master` and merge `dev`
- Create an annonated tag on `master`: `$ git tag -m x.y.z x.y.z`
- Push with tags `$ git push --follow-tags`
- CI will run and if all's well, a deployment will automatically be launched on [appveyor](https://ci.appveyor.com)
- Updating the version for vnext
  - Checkout `dev`
  - Update the version in "backend/build/version.props"
  - `$ git commit -am "chore: update version for vnext"`
  - `$ git push`
