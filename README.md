# jboss-fuse-6-tech-preview-s2i with artifactory curl

Simple extension to the jboss-fuse-6-tech-preview s2i which requires the following env vars to pull from the artifactory

- ARTIFACTORY_URL
- GROUP_ID
- ARTIFACT_ID
- ARTIFACT_VERSION
- ARTIFACT_EXTENSION

Constructs a url like:

`    DEPLOYABLE_FULL_PATH="${ARTIFACTORY_URL}/${GROUP_SECTION}/${ARTIFACT_ID}/${ARTIFACT_VERSION}/${DEPLOYABLE_NAME}" `

