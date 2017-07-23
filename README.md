# README

This repo demonstrates the use of [Active Storage](https://github.com/rails/activestorage) in Rails 5.2.

There are different branches demonstrating different features of the code:

* The `local` branch shows how to use Active Storage with local file storage
* The `aws` branch shows how to use Active Storage with Amazon Web Services
* The `gcs` branch shows how to use Active Storage with Google Cloud Storage
* The `mirror` branch shows how to use Active Storage with multiple storage backends at the same time

NOTE: To use the `mirror` branch, you will need to edit config/storage_services.yml to include your own AWS and GCS information, and supply a config/gcs.json file.