# Release process

1. Draft a new release and tag via the Github UI. If releasing against a particular commit (rather than HEAD), make sure to choose the commit in the Github UI, do not create a release on an existing tag. Travis CI doesn’t seem to react to releases created on existing tags.
1. Copy and paste relevant commits since the previous release into the release notes (find relevant commits by drafting a pull request, e.g. https://github.com/acquia/cli/compare/v1.3.0...master)
1. Pay special attention to issues with the "change record" label, these need to be called out in release notes.
1. Publish the release.
1. Ensure that Travis CI builds and attaches acli.phar as a release asset.
1. Update RELEASE.md with new version numbers.
