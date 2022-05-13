# piracema.raw

*this project is part of the <a href="https://piracema.io" target="_blank">piracema.io</a> service*

The piracema.raw project proposes a free database to support the dataset definition for building phishing prediction models. The database has a time range from 2016 to 2021 and has 999,025 records.

In the fight against phishing attacks, many solutions try to minimize the incidence of these frauds. Still, these frauds continue to grow nowadays, making us reflect on the efficiency of the proposed solutions. Nevertheless, there is a significant increase in proposals in the literature that adopt Machine Learning (ML) techniques to predict phishing. 

Conceptually, the efficiency of this type of solution depends directly on an adequate dataset for training the intelligent models. Therefore, assuming that every dataset comes from a database is coherent. To be considered efficient, the database in question needs to have a good amount of records and a well-balanced heterogeneity.

However, many phishing repositories end up providing data info very unbalanced, inconsistent, or with a series of limitations. In addition, because phishing is very volatile, there is considerable effort in storing the content-page (body's content).

*On the piracema.io page, in the <a href="https://piracema.io/repository" target="_blank">Repository</a> section, it is possible to show the piracema.raw data through an interface with filters.*

## Entries content details
|  Year  |   All entries   | With content-page | Hosting service detected | Target brand detected | Shortly service detected | With whois creation date |
|  :---: |      :---:      |      :---:        |         :---:            |        :---:          |          :---:           |          :---:           | 
|  2016  |      75,388     |      12,266       |         576              |        24,508         |            623           |            -             | 
|  2017  |      96,664     |      15,356       |         1,972            |        28,983         |           1,325          |            -             |  
|  2018  |     189,883     |      22,411       |         7,822            |        67,017         |           2,539          |            -             | 
|  2019  |     176,009     |      27,575       |         18,299           |        44,418         |           1,919          |            -             | 
|  2020  |     218,522     |      32,446       |         23,179           |        57,513         |           1,999          |            -             |  
|  2021  |     242,544     |      43,478       |         24,168           |        43,739         |           3,556          |         156,694          |  
|           Total          |     153,532       |         76,016           |       266,178         |          11,963          |         156,694          |  

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
    <td align="center">Cases of the malicious page hosted on hosting service. This detection based on URL; when these entries with the registered domain have been discarded.</td>
  <tr>
    <td align="center">target_brand</td>
    <td align="center">VARCHAR</td>
    <td align="center">Target brand recognized based on Regex and NLP</td>
  </tr>
  </tr>
  <tr>
    <td align="center">whois_creation_date</td>
    <td align="center">BIGINT</td>
    <td align="center">The domain age based on WHOIS lookup result (applied only .com, .net, and .edu registered domains)</td>
  </tr>
</table>

## Download section *
|  Year   |    Link   |  Release date | SHA256 file checksum |
|  :---:  |   :---:   |     :---:     |        :---:         |
|  2016   |  [phish_sample_2016.7z](https://github.com/cmrevoredo/piracema.raw/blob/main/phish_sample_2016.7z) |  2022-01-22  | 303d166f8281448959421c9c467fe33aec95bae4745c8459be8e871402f31598 |
|  2017   |  [phish_sample_2017.7z](https://github.com/cmrevoredo/piracema.raw/blob/main/phish_sample_2017.7z) |  2022-01-22  | - |
|  2018   |  [phish_sample_2018.7z](https://github.com/cmrevoredo/piracema.raw/blob/main/phish_sample_2018.7z) |  2022-01-22  | - |
|  2019   |  [phish_sample_2019.7z](https://github.com/cmrevoredo/piracema.raw/blob/main/phish_sample_2019.7z) |  2022-01-22  | - |
|  2020p1 |  [phish_sample_2020p1.7z](https://github.com/cmrevoredo/piracema.raw/blob/main/phish_sample_2020p17z) |  2022-01-22  | - |
|  2020p2 |  [phish_sample_2020p2.7z](https://github.com/cmrevoredo/piracema.raw/blob/main/phish_sample_2020p2.7z) |  2022-01-22  | - |
|  2021p1 |  [phish_sample_2021p1.7z](https://github.com/cmrevoredo/piracema.raw/blob/main/phish_sample_2021p1.7z) |  2022-01-22  | - |
|  2021p2 |  [phish_sample_2022p2.7z](https://github.com/cmrevoredo/piracema.raw/blob/main/phish_sample_2021p2.7z) |  2022-01-22  | - |

**Note: The JSON files were compressed (7zip) with a password. Please request the password by email: cmrs@ecomp.poli.br*


