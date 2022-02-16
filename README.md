# Rental Apartment on Den Haag

## Table of Contents
* [Dataset](https://github.com/Bayunova28/Rental_Apartment/tree/main/Dataset)
* [Code](https://github.com/Bayunova28/Rental_Apartment/blob/main/WillibrordusBayu_00000034000_IS502_BL_UAS.ipynb) 
* [Background](#background)
* [Requirement](#requirement)
* [Twitter API](#twitter-api)
* [Web Scrapping](#web-scrapping)
* [Inspiration](#inspiration)
* [Director](#director)

## Background
<img src="https://github.com/Bayunova28/Rental_Apartment/blob/main/Images/images.png" height="200" width="1000">

Pararius is the largest independent website for rental properties in the Netherlands. Pararius brings together tenants and landlords. Hundreds of professional organisations offer 
their available rental properties on Pararius. These organisations consist of real estate brokers, property management companies, developers and housing associations throughout 
the Netherlands. Visitors of Pararius can easily search the large selection of rental properties and then contact them by email or simply just by calling. Pararius was developed 
by real estate brokers that are expat rental specialists. Pararius is very convenient for both tenant and landlord. Pararius is Latin for Real Estate broker or Intermediate. 
<br />
<br />
Pararius is derived from the verb parare. Parare means prepare, to complete, to organise, to equip. The English word prepared is derived from Pararius. It is a wonderful metaphor 
for a property for rent in any category. The accommodation is ready to move in to. After signing the agreement (in most cases) the tenant will be able to move in without too much 
hassle of improving the house. Pararius wants to create a place on the internet where the rental market is transparent and where offer and demand will meet each other.

## Requirement
* **Python 3.5+**
* **Tweepy (`$ pip install tweepy`)**
* **NumPy (`$ pip install numpy`)**
* **Pandas (`$ pip install pandas`)**
* **Deep-Translator (`$ pip install deep-translator`)**
* **requests (`$ pip install requests`)**
* **BeautifulSoup4 (`$ pip install beautifulsoup4`)**
* **MatplotLib (`$ pip install matplotlib`)**

## Twitter API
To start using the Twitter API, you need to [register your application with Twitter](https://developer.twitter.com/en/products/twitter-api). Registration requires you to answer some questions about your application and agree to the [Twitter API Terms of Use](https://developer.twitter.com/en/developer-terms/agreement-and-policy).

Your new application will be assigned a consumer key/secret pair that identifies your application to Twitter. This is all you need to configure your client for application-only authentication.

```
#generate twitter API
api_key = "YOUR API KEY"
api_secret_key = "YOUR API SECRET KEY"
access_token = "YOUR ACCESS TOKEN"
access_token_secret = "YOUR ACCESS TOKEN SECRET"
```
If you have been generate the twitter API, authentication it.

```
#authentication twitter API
auth = tweepy.OAuthHandler(api_key, api_secret_key)
auth.set_access_token(access_token, access_token_secret)
api = tweepy.API(auth)
```
## Web Scrapping

### [Twitter](https://twitter.com/Pararius)
* **ID :** the id of the tweet
* **Datetime :** the date of the tweet 
* **Tweet :** the text of user tweet

### [Website](https://www.pararius.com/apartments/den-haag)
* **Name :** the name of apartment 
* **Location :** the location of apartment
* **Area :** space area of apartment
* **Price :** the price of apartment

## Inspiration
* What is the most sentiment from user tweet at Pararius?
* What is the most expensive apartment at Den Haag on Pararius website?

## Director
* Christofer Miko Lee
* Lexand Silaban
* Nicholas
* Thendy Rhenaldy
* Willibrordus Bayu

