
# PROJECT 4.2:  Twitter Clone Using Elixir and Phoenix Framework

### COP5615 - Distributed Operating Systems Principles

In this project, we use Elixir and Phoenix to make a Twitter engine. 
The functionalities of our project include:
1.	Register account (Signup)  
2.	Login and Logout  
3.	Delete account  
4.	Send and distributing tweets  
5.	Follow other users  
6.	Re-tweeting  
7.	Using Hashtags and mentions in tweets.   
8.	Querying Hashtags and Mentions.  
9.	Live feed without querying!  
In our demo video, to demonstrate the project, we create users and make them follow each other, tweet, retweet, mention each other and use hashtags. We also test the delete account functionality!  


## YOUTUBE VIDEO LINK: 
https://www.youtube.com/watch?v=xY25QMdj6ys


## Team Members:
1.	Karan Manghani (UFID: 7986-9199) Email: karanmanghani@ufl.edu 
2.	Yaswanth Bellam (UFID: 2461-6390) Email: yaswanthbellam@ufl.edu 


## Steps to run the code: 
1.	Extract the “manghanibellam.zip” file.
2.	Enter into the project folder via command prompt and type the following commands:
3.	mix ecto.create
4.	mix ecto.migrate
5.	mix phx.server
6.	Go to http://localhost:4000/
7.	You’re in!


## Functionalities and their explanation:
1.	Signup / Login: We create a separate channel for signup as well as login and based on the user’s input data, we store the login credentials in the Postgres database and then whenever he logs in, we query the database against the username and password entered. 
2.	Delete Account: We have provided a separate button on the user’s dashboards to enable the user to delete his/her account. To delete account, we first verify the request by asking the user to confirm with his password. If an incorrect password is entered, the user cannot delete the account. 
3.	Following: A text area is provided on the user’s dashboard to follow another user. The user can easily verify this by checking his followers and following using the buttons on his dashboard. Since, this is a major functionality, we use a separate channel for this.
4.	Tweeting: The core functionality of our project is tweeting. A user can easily enter his tweet on the text area provided on the UI and mention other users and use hashtags in the tweet. We parse the data as soon as it entered by the user, so as to provide live feed to the other users via the feed section. A user can also retweet other users’ tweets via a retweet button provided on the dashboard in the feed section. All the tweets that a user has done are visible via the My Tweets button on the dashboard. A user can easily see the tweets he has been mentioned in via the My Mentions button and also query the hashtags using a text area provided on the right side of the dashboard!  

To start your Phoenix server:

  * Install dependencies with `mix deps.get`
  * Create and migrate your database with `mix ecto.setup`
  * Install Node.js dependencies with `cd assets && npm install`
  * Start Phoenix endpoint with `mix phx.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.

Ready to run in production? Please [check our deployment guides](https://hexdocs.pm/phoenix/deployment.html).

## Learn more

  * Official website: http://www.phoenixframework.org/
  * Guides: https://hexdocs.pm/phoenix/overview.html
  * Docs: https://hexdocs.pm/phoenix
  * Mailing list: http://groups.google.com/group/phoenix-talk
  * Source: https://github.com/phoenixframework/phoenix
