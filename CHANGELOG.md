# CHANGE LOG

## Version 1.0.6 (2023-3-23)

- switch to https://github.com/cookiecutter-openedx/tutor-contrib-s3

## Version 1.0.5 (2023-3-17)

THIS HAS BEEN YANKED.

- repin to github.com/hastexo/tutor-contrib-s3.git@v1.0.0. After unpinning, the boto3 problem resurfaced, about
a leading "/" appearing on OPENEDX_MEDIA_ROOT.
- bump openedx-actions/tutor-k8s-get-secret@v1.0.0

Note: tutor's treatment of this setting has varied over time.

- Here it was set, with a leading "/" [tutor/templates/apps/openedx/settings/partials/common_all.py](https://github.com/overhangio/tutor/blob/ca04b245f3a0f7b44e0ab4fb9da9e100e6c9b9d9/tutor/templates/apps/openedx/settings/partials/common_all.py)
- Whereas more recently in [version v15.3.2 this was removed](https://github.com/overhangio/tutor/blob/v15.3.2/tutor/templates/apps/openedx/settings/partials/common_lms.py)
- This repo originally addressed this problem in [pr 4](https://github.com/openedx-actions/tutor-plugin-enable-s3/pull/4) by explicitly setting the value OPENEDX_MEDIA_ROOT="openedx/media/", and this had worked effectively until last night.

## Version 1.0.4 (2023-3-16)

THIS HAS BEEN YANKED.

- removed fork. install hastexo from main branch
- add all input parameters from hastexo/tutor-contrib-s3
- Bump actions/checkout from 3.3.0 to 3.4.0

## Version 1.0.3

THIS HAS BEEN YANKED.

## Version 1.0.2 (2022-12-16)

- revert to forked version https://github.com/lpm0073/tutor-contrib-s3.git@v14.0.2. Still getting a runtime error with the official hastexo version.

- bump openedx-actions/tutor-k8s-get-secret==v0.0.7

## Version 1.0.1 (2022-12-16)

- revert to https://github.com/hastexo/tutor-contrib-s3

## Version 1.0.0 (2022-06-16)

General production release

## Version 0.0.1 (2022-06-01)

**Experimental. Do not use in production.**

- Initial Git import
