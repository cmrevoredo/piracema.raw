# piracema.raw
This project proposes a free database to support the dataset definition for building phishing prediction models. The database has a time range from 2016 to 2020 and has 756,485 records.

In the fight against phishing attacks, many solutions try to minimize the incidence of these frauds. Still, these frauds continue to grow nowadays, making us reflect on the efficiency of the proposed solutions. Nevertheless, there is a significant increase in proposals in the literature that adopt Machine Learning (ML) techniques to predict phishing. 

Conceptually, the efficiency of this type of solution depends directly on an adequate dataset for training the intelligent models. Therefore, assuming that every dataset comes from a database is coherent. To be considered efficient, the database in question needs to have a good amount of records and a well-balanced heterogeneity.

However, many phishing repositories end up providing data info very unbalanced, inconsistent, or with a series of limitations. In addition, because phishing is very volatile, there is considerable effort in storing the content-page (body's content).


## Entries content details
|  Years  |   All entries   | Only with content-page |
|  :---:  |      :---:      |          :---:         |
|  2016   |      75,395     |         12,266         |
|  2017   |      96,667     |         15,356         |
|  2018   |     189,891     |         22,412         |
|  2019   |     176,010     |         27,574         |
|  2020   |     218,522     |         32,446         |

## Entries structure details
<table>
  <tr>
    <td align="center"><b>Field</b></td>
    <td align="center"><b>Type</b></td>
    <td align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="3" align="center"><b>Available</b></td>
  </tr>
  <tr>
    <td align="center">url</td>
    <td align="center">LONGTEXT</td>
    <td align="center">URL's page</td>
  </tr>
  <tr>
    <td align="center">arrival_time</td>
    <td align="center">DATETIME</td>
    <td align="center">Timestamp of phishing report</td>
  </tr>    
  <tr>
    <td align="center">http_status_code</td>
    <td align="center">INT</td>
    <td align="center">HTTP status code</td>
  </tr>
  <tr>
    <td align="center">response_content</td>
    <td align="center">LONGTEXT</td>
    <td align="center">HTTP body content</td>
  </tr>
  <tr>
    <td align="center">target_brand</td>
    <td align="center">VARCHAR</td>
    <td align="center">Target brand based on NLP</td>
  </tr>
  <tr>
    <td colspan="3" align="center"><b>Under construction</b></td>
  </tr>  
  <tr>
    <td align="center">hosting_service</td>
    <td align="center">VARCHAR</td>
    <td align="center">In case of the malicious page was hosted on a hosting service, this field identity the service name (only for cases where there is no registered domain)</td>
  </tr>
  <tr>
    <td align="center">domain_age</td>
    <td align="center">BIGINT</td>
    <td align="center">Domain age based on WHOIS (only registered domains)</td>
  </tr>
</table>

## Download section *
|  Year   |    Link   |  Release date |
|  :---:  |   :---:   |     :---:     |
|  2016   |  [phish_sample_2016.7z](https://github.com/cmrevoredo/piracema.raw/blob/main/phish_sample_2016.7z) |  2022-01-22  |
|  2017   |  [phish_sample_2017.7z](https://github.com/cmrevoredo/piracema.raw/blob/main/phish_sample_2017.7z) |  2022-01-22  |
|  2018   |  [phish_sample_2018.7z](https://github.com/cmrevoredo/piracema.raw/blob/main/phish_sample_2018.7z) |  2022-01-22  |
|  2019   |  [phish_sample_2019.7z](https://github.com/cmrevoredo/piracema.raw/blob/main/phish_sample_2019.7z) |  2022-01-22  |
|  2020p1 |  [phish_sample_2020.7z p1](https://github.com/cmrevoredo/piracema.raw/blob/main/phish_sample_2020.7z.001) |  2022-01-22  |
|  2020p2 |  [phish_sample_2020.7z p2](https://github.com/cmrevoredo/piracema.raw/blob/main/phish_sample_2020.7z.002) |  2022-01-22  |
|  2021p1 |  Under construction |  -  |
|  2021p2 |  Under construction |  -  |

*Note: The JSON files were compressed (7zip) with a password. Please request the password by email: cmrs@ecomp.poli.br


