# piracema.raw
This project proposes a free database to support the dataset definition for building phishing prediction models. The database has a time range from 2016 to 2020 and has 756,485 records.

In the fight against phishing attacks, many solutions try to minimize the incidence of these frauds. Still, these frauds continue to grow nowadays, making us reflect on the efficiency of the proposed solutions. Nevertheless, there is a significant increase in proposals in the literature that adopt Machine Learning (ML) techniques to predict phishing. 

Conceptually, the efficiency of this type of solution depends directly on an adequate dataset for training the intelligent models. Therefore, assuming that every dataset comes from a database is coherent. To be considered efficient, the database in question needs to have a good amount of records and a well-balanced heterogeneity.

However, many phishing repositories end up providing data info very unbalanced, inconsistent, or with a series of limitations. In addition, because phishing is very volatile, there is considerable effort in storing the source code (body's content).


## Entries content details
|  Years  |   All   | With content |
|  :---:  |  :---:  |    :---:     |
|  2016   |  75,395 |    12,266    |
|  2017   |  96,667 |    15,356    |
|  2018   | 189,891 |    22,412    |
|  2019   | 176,010 |    27,574    |
|  2020   | 218,522 |    32,446    |

## Entries structure details
|       Field       |    Type   |            Description          |
|       :---:       |   :---:   |              :---:              |
|         url       |  LONGTEXT |           URL's Page            |
|    arrival_time   |  DATETIME |        Timestamp Report         |
|  http_status_code |    INT    |         HTTP Status code        |
|  response_content |  LONGTEXT |        HTTP Body content        |
|    target_brand   |  VARCHAR  |    Target brand based on NLP    |

## Download section
|  Year   |    Link   |  Last update |
|  :---:  |   :---:   |    :---:     |
|  2016   |  download |  2022-01-22  |
|  2017   |  download |  2022-01-22  |
|  2018   |  download |  2022-01-22  |
|  2019   |  download |  2022-01-22  |
|  2020   |  download |  2022-01-22  |
