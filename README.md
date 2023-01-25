# piracema.raw

*this project is part of the <a href="https://piracema.io" target="_blank">piracema.io</a> service*

The piracema.raw project proposes a free database to support the dataset definition for building phishing prediction models. The database has a time range from 2016 to 2022 and has 1,368,434 records.

In the fight against phishing attacks, many solutions try to minimize the incidence of these frauds. Still, these frauds continue to grow nowadays, making us reflect on the efficiency of the proposed solutions. Nevertheless, there is a significant increase in proposals in the literature that adopt Machine Learning (ML) techniques to predict phishing. 

Conceptually, the efficiency of this type of solution depends directly on an adequate dataset for training the intelligent models. Therefore, assuming that every dataset comes from a database is coherent. To be considered efficient, the database in question needs to have a good amount of records and a well-balanced heterogeneity.

However, many phishing repositories end up providing data info very unbalanced, inconsistent, or with a series of limitations. In addition, because phishing is very volatile, there is considerable effort in storing the content-page (body's content).

*On the piracema.io page, in the <a href="https://piracema.io/repository" target="_blank">Repository</a> section, it is possible to show the piracema.raw data through an interface with filters.*

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
    <td align="center">report_time</td>
    <td align="center">DATETIME</td>
    <td align="center">Timestamp during phishing report/catch</td>
  </tr>    
  <tr>
    <td align="center">http_status_code</td>
    <td align="center">INT</td>
    <td align="center">HTTP status code during on the content-page extraction</td>
  </tr>
  <tr>
    <td align="center">response_content</td>
    <td align="center">LONGTEXT</td>
    <td align="center">HTTP body content of the maliciou's page</td>
  </tr>
  <tr>
    <td align="center">hosting_service</td>
    <td align="center">VARCHAR</td>
    <td align="center">Cases of the malicious page hosted on hosting service and recognized based on Regex and NLP. This detection based on URL; when these entries with the registered domain have been discarded.</td>
  <tr>
    <td align="center">target_brand</td>
    <td align="center">VARCHAR</td>
    <td align="center">Target brand recognized based on Regex and NLP</td>
  </tr>
  <tr>
    <td align="center">shortly_service</td>
    <td align="center">VARCHAR</td>
    <td align="center">URL shortening service recognized based on Regex and NLP</td>
  </tr>
  </tr>
  <tr>
    <td align="center">whois_creation_date</td>
    <td align="center">DATETIME</td>
    <td align="center">The domain age based on WHOIS lookup result (applied only .com, .net, and .edu registered domains)</td>
  </tr>
</table>

## Entries content details
|  Year  |   All entries   | With content-page | Hosting service detected | Target brand detected | Shortly service detected | With whois creation date |
|  :---: |      :---:      |      :---:        |         :---:            |        :---:          |          :---:           |          :---:           | 
|  2016  |      75,130     |      12,202       |            572           |        24,444         |            1050          |            -             | 
|  2017  |      96,195     |      15,307       |          1,971           |        28,887         |           2,128          |            -             |  
|  2018  |     189,491     |      22,355       |          7,809           |        66,854         |           4,025          |            -             | 
|  2019  |     175,976     |      27,566       |         18,294           |        44,405         |           2,296          |            -             | 
|  2020  |     218,459     |      32,441       |         23,167           |        57,505         |           2,430          |            -             |  
|  2021  |     187,220     |      25,671       |         18,784           |        36,321         |           3,079          |         123,285          |  
|  2022  |     425,963     |      93,815       |         40,991           |        28,767         |          13,318          |         187,962          |  
|  Total |    1,368,434    |     229,357       |        111,588           |       287,183         |          28,326          |         311,247          |  

## Download section *
|   Year    |    Link   |  Release date | SHA256 file checksum |
| :------:  |   :---:   |     :---:     |        :---:         |
| 2016-2022 |  contact us! |  2023-01-20  | - | 

**Note: The JSON files were compressed (7zip) with a password. Please request the password by email: cmrs@ecomp.poli.br*


