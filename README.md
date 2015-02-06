# ETL Hub Profiles

Hub Profiles instruct the [ETL Hub Services](https://github.com/UMNLibraries/ETLHub.services) application on how to extract and transform data from a given endpoint (e.g. an OAI provider) and then on how to load the metadata within the [ETL Hub Client](https://github.com/UMNLibraries/ETLHub.client) application. Profiles are stored and managed within the ETL Hub Client.

Hub Profile JSON documents consist of three main areas:
* An `extractor` section that instructs the ETL Hub services on how and where to find a batch of metadata and  supplimental "enrichment" metatada for later use within a transformation
* A `transformer` section that contains field transformation profiles, defualt metadata and field transformation profile template details
* A `storage_destinations` section that details where to load transformed metadata relative to a configurable local file system directory. Future support for Fedora 4 is planned and additional targets (e.g. S3) can be easily added.




