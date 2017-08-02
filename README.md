# README

This repo demonstrates the use of [Active Storage](https://github.com/rails/activestorage) in Rails 5.2.

There are different branches demonstrating different features of the code:

* The `local` branch shows how to use Active Storage with local file storage
* The `aws` branch shows how to use Active Storage with Amazon Web Services
* The `gcs` branch shows how to use Active Storage with Google Cloud Storage
* The `azure` branch shows how to use Active Storage with Microsoft Azure
* The `mirror` branch shows how to use Active Storage with multiple storage backends at the same time

NOTE: To use the `mirror` branch, you will need to edit config/storage_services.yml to include your own AWS and GCS information, and supply a config/gcs.json file.

## A Note On Code Stability

It isn't. Active Storage has been merged to the main Rails project now, but it's not yet merged to master. Expect further changes and improvements, as well as potentially broken things.

That said, I'll try to keep [my article](https://afreshcup.com/home/2017/07/23/activestorage-samples) and these associated samples up-to-date. No promises though.</p>

## Change History

- 2 August 2017
  - Switch to Rails with merged Active Storage, remove separate Active Storage gem.
  - Added Microsoft Azure sample
  - Added direct upload sample
  - Switched to using `url_for(document.url)` in show. See https://github.com/rails/activestorage/commit/d0e90b4a9dc1accd4f1044fde0dd9a347cd0afcf and future plans at https://github.com/rails/activestorage/issues/77
- 24 July 2017
  - Updated database schema. If you used an earlier version of the samples, you'll need to drop & recreate the database.
  - Replaced `.url` with `.service_url`
