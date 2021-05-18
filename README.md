# Postman OCAPI Collection
Postman collection for Salesforce Commerce Cloud OCAPI (Open Commerce API)

## Usage
* [Download Collection](../../raw/master/SFCC_OCAPI.postman_collection)
* Import it in your Postman environment
* Edit the collection by adding these data at *Pre-Request Scripts*
  * **ocapi-instance-host** - Hostname or public domain for your SFCC instance (e.g. `development-eu01-mycompanyname.demandware.net`),
  * **ocapi-site** - Site ID of the actual site to be used (e.g. `SiteGenesis`),
  * **ocapi-version** - OCAPI Version used by your current SFCC instance (e.g. `v21_3`),
  * **bm_username** - Username for BM grant at SFCC,
  * **bm_password** - Password for BM grant at SFCC,
  * **ocapi-client-id** - Client ID for Client Credentials grant at SFCC,
  * **ocapi-client-secret** - Client password for Client Credentials grant at SFCC
* Save

## Collection
This collection integrates following OCAPI resources.

### Authentication
| **Method** | **OCAPI Resource** | **Description**                                                                     |
|------------|--------------------|-------------------------------------------------------------------------------------|
| POST       | OAuth 2.0          | Retrieve access token based on Business Manager (BM) credentials                    |

### Shop API
| **Method** | **OCAPI Resource** | **Description**                      |
|------------|--------------------|--------------------------------------|
| GET        | Orders             | Fetch information for a single Order |
| POST       | OrderSearch        | Search for Orders                    |

### Data API
| **Method** | **OCAPI Resource** | **Description**           |
|------------|--------------------|---------------------------|
| POST       | JobSearch          | Search for Job executions |

### Meta API
| **Method** | **Description**                |
|------------|--------------------------------|
| GET        | List of available API versions |

## Contributions
* Want to extend the current collection? Awesome! Feel free to create a [PR](https://github.com/edro15/postman-ocapi-collection/pulls)
* Found a bug? Open an [issue](https://github.com/edro15/postman-ocapi-collection/issues)

## License
MIT Licensed. See [LICENSE](https://github.com/edro15/postman-ocapi-collection/blob/master/LICENSE) for full details.
