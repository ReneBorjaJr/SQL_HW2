# SQL_HW2
```sql
-- Using count, get the number of cities in the USA
mysql> select COUNT(name) AS '# of cities in USA'
    -> from city
    -> where countrycode = 'USA';
+--------------------+
| # of cities in USA |
+--------------------+
|                274 |
+--------------------+

-- Find out what the population and average life expectancy for people in Argentina (ARG) is!
mysql> select population AS 'population in ARG', lifeexpectancy AS 'life expectancy in ARG'
    -> from country
    -> where code = 'ARG';
+-------------------+------------------------+
| population in ARG | life expectancy in ARG |
+-------------------+------------------------+
|          37032000 |                   75.1 |
+-------------------+------------------------+

-- Display all the cities for any country of your choice besides the USA
mysql> select name AS 'cities in Brazil'
    -> from city
    -> where countrycode = 'BRA'
    -> order by name;
+--------------------------+
| cities in Brazil         |
+--------------------------+
| Abaetetuba               |
| Águas Lindas de Goiás    |
| Alagoinhas               |
| Alvorada                 |
| Americana                |
| Ananindeua               |
| Anápolis                 |
| Angra dos Reis           |
| Aparecida de Goiânia     |
| Apucarana                |
| Aracaju                  |
| Araçatuba                |
| Araguaína                |
| Araguari                 |
| Arapiraca                |
| Araraquara               |
| Araras                   |
| Atibaia                  |
| Bacabal                  |
| Bagé                     |
| Barbacena                |
| Barra do Piraí           |
| Barra Mansa              |
| Barreiras                |
| Barretos                 |
| Barueri                  |
| Bauru                    |
| Belém                    |
| Belford Roxo             |
| Belo Horizonte           |
| Bento Gonçalves          |
| Betim                    |
| Birigui                  |
| Blumenau                 |
| Boa Vista                |
| Botucatu                 |
| Bragança Paulista        |
| Brasília                 |
| Cabo de Santo Agostinho  |
| Cabo Frio                |
| Cachoeirinha             |
| Cachoeiro de Itapemirim  |
| Camaçari                 |
| Camaragibe               |
| Cametá                   |
| Campina Grande           |
| Campinas                 |
| Campo Grande             |
| Campo Largo              |
| Campos dos Goytacazes    |
| Canoas                   |
| Carapicuíba              |
| Cariacica                |
| Caruaru                  |
| Cascavel                 |
| Castanhal                |
| Catanduva                |
| Caucaia                  |
| Caxias                   |
| Caxias do Sul            |
| Chapecó                  |
| Codó                     |
| Colatina                 |
| Colombo                  |
| Conselheiro Lafaiete     |
| Contagem                 |
| Coronel Fabriciano       |
| Corumbá                  |
| Cotia                    |
| Crato                    |
| Criciúma                 |
| Cubatão                  |
| Cuiabá                   |
| Curitiba                 |
| Diadema                  |
| Divinópolis              |
| Dourados                 |
| Duque de Caxias          |
| Embu                     |
| Eunápolis                |
| Feira de Santana         |
| Ferraz de Vasconcelos    |
| Florianópolis            |
| Fortaleza                |
| Foz do Iguaçu            |
| Franca                   |
| Francisco Morato         |
| Franco da Rocha          |
| Garanhuns                |
| Goiânia                  |
| Governador Valadares     |
| Gravataí                 |
| Guaíba                   |
| Guarapuava               |
| Guaratinguetá            |
| Guarujá                  |
| Guarulhos                |
| Hortolândia              |
| Ibirité                  |
| Ilhéus                   |
| Imperatriz               |
| Indaiatuba               |
| Ipatinga                 |
| Itabira                  |
| Itaboraí                 |
| Itabuna                  |
| Itaituba                 |
| Itajaí                   |
| Itapecerica da Serra     |
| Itapetininga             |
| Itapevi                  |
| Itaquaquecetuba          |
| Itu                      |
| Ituiutaba                |
| Jaboatão dos Guararapes  |
| Jacareí                  |
| Jacobina                 |
| Jaraguá do Sul           |
| Jaú                      |
| Jequié                   |
| Ji-Paraná                |
| João Pessoa              |
| Joinville                |
| Juazeiro                 |
| Juazeiro do Norte        |
| Juiz de Fora             |
| Jundíaí                  |
| Lages                    |
| Lauro de Freitas         |
| Limeira                  |
| Linhares                 |
| Londrina                 |
| Luziânia                 |
| Macaé                    |
| Macapá                   |
| Maceió                   |
| Magé                     |
| Manaus                   |
| Marabá                   |
| Maracanaú                |
| Marília                  |
| Maringá                  |
| Mauá                     |
| Moji das Cruzes          |
| Moji-Guaçu               |
| Montes Claros            |
| Mossoró                  |
| Natal                    |
| Nilópolis                |
| Niterói                  |
| Nossa Senhora do Socorro |
| Nova Friburgo            |
| Nova Iguaçu              |
| Novo Hamburgo            |
| Olinda                   |
| Osasco                   |
| Ourinhos                 |
| Palhoça                  |
| Palmas                   |
| Paranaguá                |
| Parnaíba                 |
| Parnamirim               |
| Passo Fundo              |
| Passos                   |
| Patos                    |
| Patos de Minas           |
| Paulista                 |
| Paulo Afonso             |
| Pelotas                  |
| Petrolina                |
| Petrópolis               |
| Pindamonhangaba          |
| Pinhais                  |
| Piracicaba               |
| Poá                      |
| Poços de Caldas          |
| Ponta Grossa             |
| Porto Alegre             |
| Porto Velho              |
| Pouso Alegre             |
| Praia Grande             |
| Presidente Prudente      |
| Queimados                |
| Recife                   |
| Resende                  |
| Ribeirão das Neves       |
| Ribeirão Pires           |
| Ribeirão Preto           |
| Rio Branco               |
| Rio Claro                |
| Rio de Janeiro           |
| Rio Grande               |
| Rio Verde                |
| Rondonópolis             |
| Sabará                   |
| Salto                    |
| Salvador                 |
| Santa Bárbara d´Oeste    |
| Santa Cruz do Sul        |
| Santa Luzia              |
| Santa Maria              |
| Santa Rita               |
| Santana do Livramento    |
| Santarém                 |
| Santo André              |
| Santos                   |
| São Bernardo do Campo    |
| São Caetano do Sul       |
| São Carlos               |
| São Gonçalo              |
| São João de Meriti       |
| São José                 |
| São José de Ribamar      |
| São José do Rio Preto    |
| São José dos Campos      |
| São José dos Pinhais     |
| São Leopoldo             |
| São Lourenço da Mata     |
| São Luís                 |
| São Paulo                |
| São Vicente              |
| Sapucaia do Sul          |
| Serra                    |
| Sertãozinho              |
| Sete Lagoas              |
| Sobral                   |
| Sorocaba                 |
| Sumaré                   |
| Suzano                   |
| Taboão da Serra          |
| Tatuí                    |
| Taubaté                  |
| Teixeira de Freitas      |
| Teófilo Otoni            |
| Teresina                 |
| Teresópolis              |
| Timon                    |
| Toledo                   |
| Uberaba                  |
| Uberlândia               |
| Uruguaiana               |
| Varginha                 |
| Várzea Grande            |
| Viamão                   |
| Vila Velha               |
| Vitória                  |
| Vitória da Conquista     |
| Vitória de Santo Antão   |
| Volta Redonda            |
| Votorantim               |
+--------------------------+

## My two queries ##
-- 1) Display the # of cities per country, grouped by country code, ordered by the number of cities
mysql> select COUNT(name) AS '# of cities per country', countrycode AS 'Country Code'
    -> from city
    -> group by countrycode
    -> order by COUNT(name);
+-------------------------+--------------+
| # of cities per country | Country Code |
+-------------------------+--------------+
|                       1 | ABW          |
|                       1 | ALB          |
|                       1 | AND          |
|                       1 | ANT          |
|                       1 | ATG          |
|                       1 | BDI          |
|                       1 | BHR          |
|                       1 | BHS          |
|                       1 | BRB          |
|                       1 | BRN          |
|                       1 | BTN          |
|                       1 | CAF          |
|                       1 | COK          |
|                       1 | COM          |
|                       1 | CPV          |
|                       1 | CRI          |
|                       1 | CXR          |
|                       1 | CYM          |
|                       1 | DJI          |
|                       1 | DMA          |
|                       1 | ERI          |
|                       1 | ESH          |
|                       1 | FJI          |
|                       1 | FLK          |
|                       1 | FRO          |
|                       1 | GAB          |
|                       1 | GIB          |
|                       1 | GIN          |
|                       1 | GNB          |
|                       1 | GNQ          |
|                       1 | GRD          |
|                       1 | GRL          |
|                       1 | GUF          |
|                       1 | GUY          |
|                       1 | ISL          |
|                       1 | KNA          |
|                       1 | LBR          |
|                       1 | LCA          |
|                       1 | LSO          |
|                       1 | LUX          |
|                       1 | MAC          |
|                       1 | MDV          |
|                       1 | MHL          |
|                       1 | MKD          |
|                       1 | MLI          |
|                       1 | MNG          |
|                       1 | MNP          |
|                       1 | MSR          |
|                       1 | MTQ          |
|                       1 | MYT          |
|                       1 | NAM          |
|                       1 | NCL          |
|                       1 | NFK          |
|                       1 | NIU          |
|                       1 | PCN          |
|                       1 | PLW          |
|                       1 | PNG          |
|                       1 | QAT          |
|                       1 | REU          |
|                       1 | RWA          |
|                       1 | SGP          |
|                       1 | SHN          |
|                       1 | SJM          |
|                       1 | SLB          |
|                       1 | SLE          |
|                       1 | SPM          |
|                       1 | STP          |
|                       1 | SUR          |
|                       1 | SWZ          |
|                       1 | SYC          |
|                       1 | TCA          |
|                       1 | TGO          |
|                       1 | TKL          |
|                       1 | TMP          |
|                       1 | TON          |
|                       1 | TUV          |
|                       1 | UGA          |
|                       1 | URY          |
|                       1 | VAT          |
|                       1 | VCT          |
|                       1 | VGB          |
|                       1 | VIR          |
|                       1 | VUT          |
|                       1 | WLF          |
|                       1 | WSM          |
|                       2 | AIA          |
|                       2 | ASM          |
|                       2 | BLZ          |
|                       2 | BMU          |
|                       2 | BWA          |
|                       2 | CCK          |
|                       2 | COG          |
|                       2 | CYP          |
|                       2 | EST          |
|                       2 | FSM          |
|                       2 | GLP          |
|                       2 | GMB          |
|                       2 | GUM          |
|                       2 | HKG          |
|                       2 | IRL          |
|                       2 | KGZ          |
|                       2 | KIR          |
|                       2 | LAO          |
|                       2 | LBN          |
|                       2 | LIE          |
|                       2 | MCO          |
|                       2 | MLT          |
|                       2 | MRT          |
|                       2 | MWI          |
|                       2 | NRU          |
|                       2 | PAN          |
|                       2 | PYF          |
|                       2 | SMR          |
|                       2 | SVN          |
|                       2 | TCD          |
|                       2 | TJK          |
|                       2 | TTO          |
|                       3 | ARM          |
|                       3 | BFA          |
|                       3 | BIH          |
|                       3 | HND          |
|                       3 | JAM          |
|                       3 | KHM          |
|                       3 | KWT          |
|                       3 | LVA          |
|                       3 | MUS          |
|                       3 | NER          |
|                       3 | SOM          |
|                       3 | SVK          |
|                       4 | AFG          |
|                       4 | AZE          |
|                       4 | BEN          |
|                       4 | GTM          |
|                       4 | HRV          |
|                       4 | HTI          |
|                       4 | LBY          |
|                       4 | MDA          |
|                       4 | NIC          |
|                       4 | TKM          |
|                       5 | AGO          |
|                       5 | ARE          |
|                       5 | CHE          |
|                       5 | CIV          |
|                       5 | DNK          |
|                       5 | GEO          |
|                       5 | GHA          |
|                       5 | JOR          |
|                       5 | LTU          |
|                       5 | MDG          |
|                       5 | NOR          |
|                       5 | NPL          |
|                       5 | OMN          |
|                       5 | PRT          |
|                       5 | PRY          |
|                       6 | AUT          |
|                       6 | DOM          |
|                       6 | PSE          |
|                       6 | YEM          |
|                       6 | ZWE          |
|                       7 | CMR          |
|                       7 | ETH          |
|                       7 | FIN          |
|                       7 | LKA          |
|                       7 | SLV          |
|                       7 | ZMB          |
|                       8 | BOL          |
|                       8 | GRC          |
|                       8 | KEN          |
|                       8 | TUN          |
|                       8 | YUG          |
|                       9 | BEL          |
|                       9 | HUN          |
|                       9 | NZL          |
|                       9 | PRI          |
|                       9 | SEN          |
|                      10 | BGR          |
|                      10 | CZE          |
|                      10 | TZA          |
|                      11 | SYR          |
|                      12 | MOZ          |
|                      12 | SDN          |
|                      12 | THA          |
|                      13 | PRK          |
|                      14 | AUS          |
|                      14 | CUB          |
|                      14 | ISR          |
|                      15 | ECU          |
|                      15 | IRQ          |
|                      15 | SWE          |
|                      16 | BLR          |
|                      16 | MMR          |
|                      17 | UZB          |
|                      18 | COD          |
|                      18 | DZA          |
|                      18 | MYS          |
|                      21 | KAZ          |
|                      22 | MAR          |
|                      22 | PER          |
|                      22 | VNM          |
|                      24 | BGD          |
|                      24 | SAU          |
|                      28 | NLD          |
|                      29 | CHL          |
|                      29 | ROM          |
|                      37 | EGY          |
|                      38 | COL          |
|                      40 | FRA          |
|                      41 | VEN          |
|                      42 | TWN          |
|                      44 | POL          |
|                      44 | ZAF          |
|                      49 | CAN          |
|                      57 | ARG          |
|                      57 | UKR          |
|                      58 | ITA          |
|                      59 | ESP          |
|                      59 | PAK          |
|                      62 | TUR          |
|                      64 | NGA          |
|                      67 | IRN          |
|                      70 | KOR          |
|                      81 | GBR          |
|                      85 | IDN          |
|                      93 | DEU          |
|                     136 | PHL          |
|                     173 | MEX          |
|                     189 | RUS          |
|                     248 | JPN          |
|                     250 | BRA          |
|                     274 | USA          |
|                     341 | IND          |
|                     363 | CHN          |
+-------------------------+--------------+

-- 2) Display each government form and the # of countires per government form, grouped by government form and ordered by the # of countries per government form
mysql> select COUNT(name) AS '# of countries per government form', governmentform AS 'Government Form'
    -> from country
    -> group by governmentform
    -> order by COUNT(name);
+------------------------------------+----------------------------------------------+
| # of countries per government form | Government Form                              |
+------------------------------------+----------------------------------------------+
|                                  1 | Federation                                   |
|                                  1 | Islamic Emirate                              |
|                                  1 | Dependent Territory of the US                |
|                                  1 | Independent Church State                     |
|                                  1 | Parliamentary Coprincipality                 |
|                                  1 | Emirate Federation                           |
|                                  1 | Parlementary Monarchy                        |
|                                  1 | People'sRepublic                             |
|                                  1 | Co-administrated                             |
|                                  1 | Occupied by Marocco                          |
|                                  1 | Constitutional Monarchy (Emirate)            |
|                                  1 | Socialistic State                            |
|                                  1 | Monarchy (Emirate)                           |
|                                  1 | Autonomous Area                              |
|                                  1 | Administrated by the UN                      |
|                                  2 | Monarchy (Sultanate)                         |
|                                  2 | Dependent Territory of Norway                |
|                                  2 | Commonwealth of the US                       |
|                                  2 | Territorial Collectivity of France           |
|                                  2 | Part of Denmark                              |
|                                  2 | Special Administrative Region of China       |
|                                  2 | Islamic Republic                             |
|                                  2 | Nonmetropolitan Territory of The Netherlands |
|                                  3 | US Territory                                 |
|                                  3 | Socialistic Republic                         |
|                                  3 | Nonmetropolitan Territory of New Zealand     |
|                                  4 | Nonmetropolitan Territory of France          |
|                                  4 | Constitutional Monarchy, Federation          |
|                                  4 | Territory of Australia                       |
|                                  4 | Overseas Department of France                |
|                                  5 | Monarchy                                     |
|                                 12 | Dependent Territory of the UK                |
|                                 15 | Federal Republic                             |
|                                 29 | Constitutional Monarchy                      |
|                                122 | Republic                                     |
+------------------------------------+----------------------------------------------+
