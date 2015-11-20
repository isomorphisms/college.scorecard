#US colleges where less than ¼ of the graduates are making more than $25,000/year, 10 years after graduating.

(reference diagram for how much $25k is: http://visualizingeconomics.com/blog/2006/11/05/2005-us-income-distribution)

(data source: https://collegescorecard.ed.gov/data/)

```
|------------------------------------------------------+------------------------------------------|
|  Name of Institution                                 | % Earning over $25k, 10 years after grad |
|------------------------------------------------------+------------------------------------------|
|  Rogers Academy of Hair Design                       | 10%                                      |
|  Salon Success Academy-San Bernardino                | 14%                                      |
|  Cannella School of Hair Design-Chicago              | 14%                                      |
|  Sierra College of Beauty                            | 15%                                      |
|  Searcy Beauty College Inc                           | 15%                                      |
|  Empire Beauty School-Dixie                          | 15%                                      |
|  Professional Institute of Beauty                    | 15%                                      |
|  Louisiana Academy of Beauty                         | 15%                                      |
|  Creations College of Cosmetology                    | 16%                                      |
|  La Belle Beauty School                              | 18%                                      |
|  House of Heavilin Beauty College-Kansas City        | 18%                                      |
|  Empire Beauty School-Elizabethtown                  | 18%                                      |
|  Olympian University of Cosmetology                  | 19%                                      |
|  Arthur's Beauty College Inc-Fort Smith              | 19%                                      |
|  Hair Academy of Safford                             | 20%                                      |
|  Trend Setters' Academy of Beauty Culture-Louisville | 20%                                      |
|  Marinello Schools of Beauty-Moreno Valley           | 20%                                      |
|  Little Big Horn College                             | 20%                                      |
|  Rosemead Beauty School                              | 21%                                      |
|  Rudae's School of Beauty Culture-Kokomo             | 21%                                      |
|  Mr Bela's School of Cosmetology Inc                 | 21%                                      |
|  Marinello Schools of Beauty-Burbank                 | 21%                                      |
|  Joseph's College                                    | 22%                                      |
|  Beauty Schools of America-Miami                     | 22%                                      |
|  Twin City Beauty College                            | 22%                                      |
|  Robert Fiance Beauty Schools-West New York          | 22%                                      |
|  La James International College-East Moline          | 22%                                      |
|  Faust Institute of Cosmetology-Storm Lake           | 22%                                      |
|  Victor Valley Beauty College Inc                    | 22%                                      |
|  Neosho Beauty College                               | 22%                                      |
|  Elaine Steven Beauty College                        | 23%                                      |
|  Delta Beauty College                                | 23%                                      |
|  Manhattan Hairstyling Academy - North               | 23%                                      |
|  Manhattan Hairstyling Academy                       | 23%                                      |
|  La'James International College                      | 23%                                      |
|  Guy's Shreveport Academy of Cosmetology Inc         | 23%                                      |
|  Mr Leon's School of Hair Design-Moscow              | 23%                                      |
|  Empire Beauty School-Waterville                     | 23%                                      |
|  Empire Beauty School-Bangor                         | 23%                                      |
|  Empire Beauty School-Caribou                        | 23%                                      |
|  Empire Beauty School-Maine                          | 23%                                      |
|  New Tyler Barber College Inc                        | 23%                                      |
|  Marinello School of Beauty                          | 24%                                      |
|  Marinello School of Beauty                          | 24%                                      |
|  Marinello School of Beauty                          | 24%                                      |
|  Marinello School of Beauty                          | 24%                                      |
|  Marinello School of Beauty                          | 24%                                      |
|  Marinello School of Beauty                          | 24%                                      |
|  Marinello School of Beauty                          | 24%                                      |
|  Marinello School of Beauty                          | 24%                                      |
|  Marinello Schools of Beauty-Los Angeles             | 24%                                      |
|  Chris Beauty College                                | 24%                                      |
|  Marinello Schools of Beauty-Hemet                   | 24%                                      |
|  Hot Springs Beauty College                          | 24%                                      |
|  Mac Daniels Beauty School                           | 24%                                      |
|  Gem City College                                    | 25%                                      |
|  Arkansas College of Barbering and Hair Design       | 25%                                      |
|  Arkansas College of Barbering and Hair Design       | 25%                                      |
|------------------------------------------------------+-----------------------------------------+------|
```


We can draw some useful advice from this:

1. Don't be from a poor geography.
2. Be a beauty-school dropout.
3. Don't trust Mr Leon.


That's a quick look (using `csvkit`).

The next obvious question is, how can we adjust for some of the geographic factors?
Little Big Horn, [Shreveport](https://www.youtube.com/watch?v=sOcnITphyjk "This might be Lake Charles rather than Shreveport, but it captures a bit of Louisiana for you if you haven't been through there."), Gem City, Hot Springs, Hemet/Moreno Valley, Waterville, and Bangor
(all of which I think I've seen in person) are not high on the list of places with
employment opportunities bursting out of the stitching.


My next idea is to try to adjust for _family_ income. That should cover both Empire
Beauty School in Manhattan, and the "South Dakota effect".