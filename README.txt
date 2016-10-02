

	 ██████╗ █████╗ ██████╗ ██████╗ ███████╗███████╗ ██████╗ ██╗   ██╗██████╗ 
	██╔════╝██╔══██╗██╔══██╗██╔══██╗██╔════╝██╔════╝██╔═══██╗██║   ██║██╔══██╗
	██║     ███████║██████╔╝██████╔╝█████╗  █████╗  ██║   ██║██║   ██║██████╔╝
	██║     ██╔══██║██╔══██╗██╔══██╗██╔══╝  ██╔══╝  ██║   ██║██║   ██║██╔══██╗
	╚██████╗██║  ██║██║  ██║██║  ██║███████╗██║     ╚██████╔╝╚██████╔╝██║  ██║
	 ╚═════╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝╚═╝      ╚═════╝  ╚═════╝ ╚═╝  ╚═╝
                                                                                                                                                         
        ██████╗██╗  ██╗ █████╗ ██╗     ██╗     ███████╗███╗   ██╗ ██████╗ ███████╗
       ██╔════╝██║  ██║██╔══██╗██║     ██║     ██╔════╝████╗  ██║██╔════╝ ██╔════╝
       ██║     ███████║███████║██║     ██║     █████╗  ██╔██╗ ██║██║  ███╗█████╗  
       ██║     ██╔══██║██╔══██║██║     ██║     ██╔══╝  ██║╚██╗██║██║   ██║██╔══╝  
       ╚██████╗██║  ██║██║  ██║███████╗███████╗███████╗██║ ╚████║╚██████╔╝███████╗
        ╚═════╝╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝╚══════╝╚══════╝╚═╝  ╚═══╝ ╚═════╝ ╚══════╝
                                                                                                                                                         
		Carrefour Delighting Customers Challenge Basket Data  
			    TADHACK  - 14-16 OCT 2016
                       (http://tadhack.com/2016/global/)

										
CONTENTS OF FILE
---------------------

  * Challenge Description	
  * Getting Started
  * Things to Note
  * Data Fields	
  * Data File Structure				


CHALLENGE DESCRIPTION
---------------------

Outstanding customer satisfaction  is Carrefour's absolute commitment. As one of the world's largest retailers, with presence in over 35 countries and more than €100 billion in sales, we strive to make our customer experience the best there is. That is why, as part of the Telecom Application Developer Hackathon taking place globally, Carrefour proposes a challenge: to use our anonymized basket data to make shopping a delightful experience.

The goal of the challenge is to design and develop a prototype app for mobile or the web that improves consumer experience.To help you achieve this goal we put at your disposal thousands of tickets with anonymized information. Create apps using the information provided and online sources like social media, geolocation, weather data, blogs, forums, and all kinds of websites to take our customer's shopping experience to a new level. Develop shopping assistants, food specialist apps that count calories and help make healthier choices, find new applications to virtual reality, predict the clients next necessity or create something totally different.

The challenge’s jury will be made up of experts from Madrid's Polytechnic University and Carrefour and will judge based of the following criteria:

## Improvement To Customer Experience       35%   (How much does it improve the shopping experience?)
## Creativity                               25%   (How much of a novel idea is it?)
## Disruptive Impact                        20%   (Does it solve a real problem?)
## Design                                   20%   (Technology, simplicity, scalability)


GETTING STARTED
---------------------

The data base you are being given consists of a 1 Gb json file. The file contains a sample of more than 580,000 tickets for two different stores that date since Jan 2016 to May 2016 containing more than 50,000 different products, over 60,000 clients. The goal of the challenge is to design and develop a prototype app for mobile or the web that improves consumer experience. 


THINGS TO NOTE
---------------------

## Not all customers have an ID. Some customers aren't registered in our loyalty program.
## Not all stores have the same products. 
## Some customers buy in both stores others do not.
## Items with the same description might have different prices. This depends on what type of article it is, some priced are based on weight, others carry a discounted price if bought while a promotion was active. 


DATA FIELDS
---------------------

The file contains the following fields:

## ID      - Number id for that individual ticket.
## MALL    - Store where the ticket was printed. It has two values, 1 and 2. 
## DATE    - Date and time the ticket was printed.
## CLIENT  - Some tickets will have a Customer ID. Many tickets will share a Customer ID. 
## ITEMS   - List of items contained in the printed ticket. The list contains a dictionary with a product description (desc), the amount charged (net_am), and the number of units bought (n_unit).


DATA FILE STRUCTURE
---------------------

_id    : NumberInt
mall   : NumberInt 
date   : ISODate
client : NumberLong(77021708271)
items  : [{
            "net_am" : NumberInt
            "n_unit" : NumberInt 
            "desc"   : String
         }] 

This Carrefour-dataset is made available under the Open Data Commons Attribution License: 
http://opendatacommons.org/licenses/by/1.0/


