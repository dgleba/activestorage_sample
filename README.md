# README

This repo demonstrates the use of [Active Storage](https://github.com/rails/activestorage) in Rails 5.2.

There are different branches demonstrating different features of the code:

* The `local` branch shows how to use Active Storage with local file storage
* The `aws` branch shows how to use Active Storage with Amazon Web Services
* The `gcs` branch shows how to use Active Storage with Google Cloud Storage
* The `azure` branch shows how to use Active Storage with Microsoft Azure
* The `mirror` branch shows how to use Active Storage with multiple storage backends at the same time
* The `variant` branch shows how to to apply MiniMagick transforms to stored images
* The `direct_upload` branch shows how to upload directly from the user's web client to the storage service

NOTE: To use the `aws` branch, you will need to edit config/storage_services.yml to include your own AWS information.

## A Note On Code Stability

It isn't. As the Active Storage README itself says:

    Active Storage only works with the development version of Rails 5.2+ (as of July 19, 2017). This separate repository is a staging ground for the upcoming inclusion in rails/rails prior to the Rails 5.2 release. It is not intended to be a long-term stand-alone repository.

    Furthermore, this repository is likely to be in heavy flux prior to the merge to rails/rails. You're heartedly encouraged to follow along and even use Active Storage in this phase, but don't be surprised if the API suffers frequent breaking changes prior to the merge.

That said, I'll try to keep [my article](https://afreshcup.com/home/2017/07/23/activestorage-samples) and these associated samples up-to-date. No promises though.</p>

## Change History

- 31 July 2017
  - Added Microsoft Azure sample
  - Added direct upload sample
  - Switched to using `url_for(document.url)` in show. See https://github.com/rails/activestorage/commit/d0e90b4a9dc1accd4f1044fde0dd9a347cd0afcf and future plans at https://github.com/rails/activestorage/issues/77
- 24 July 2017
  - Updated database schema. If you used an earlier version of the samples, you'll need to drop & recreate the database.
  - Replaced `.url` with `.service_url`
