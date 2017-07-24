# README

This repo demonstrates the use of [Active Storage](https://github.com/rails/activestorage) in Rails 5.2.

There are different branches demonstrating different features of the code:

* The `local` branch shows how to use Active Storage with local file storage
* The `aws` branch shows how to use Active Storage with Amazon Web Services
* The `gcs` branch shows how to use Active Storage with Google Cloud Storage
* The `mirror` branch shows how to use Active Storage with multiple storage backends at the same time
* The `variant` branchs shows how to to apply MiniMagic transforms to stored images

## A Note On Code Stability

It isn't. As the Active Storage README itself says:

    Active Storage only works with the development version of Rails 5.2+ (as of July 19, 2017). This separate repository is a staging ground for the upcoming inclusion in rails/rails prior to the Rails 5.2 release. It is not intended to be a long-term stand-alone repository.

    Furthermore, this repository is likely to be in heavy flux prior to the merge to rails/rails. You're heartedly encouraged to follow along and even use Active Storage in this phase, but don't be surprised if the API suffers frequent breaking changes prior to the merge.

That said, I'll try to keep [my article](https://afreshcup.com/home/2017/07/23/activestorage-samples) and these associated samples up-to-date. No promises though.</p>

## Change History

- 24 July 2017
  - Updated database schema. If you used an earlier version of the samples, you'll need to drop & recreate the database.
  - Replaced `.url` with `.service_url`
