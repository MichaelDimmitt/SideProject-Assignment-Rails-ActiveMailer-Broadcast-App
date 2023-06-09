# Rails-ActiveMailer-Broadcast-App
This side project will try to achieve the same outcomes with the latest rails, Rails 7, using built in tools like ActiveMailer. We are going to have open syncs around the project at Saint Augustine [Jax Code and Coffee](https://www.meetup.com/jax-code-and-coffee). 

Using Twilio &amp; Mailgun APIs. Fly your SMS broadcasts to the moon!

### How This Thing Works

Rails-ActiveMailer-Broadcast-App started off as a rewrite of [Sinatra Broadcast](https://github.com/nbkkb7x/sinatra-broadcast) which started off as a fork from [The Baby Broadcast System](https://github.com/GregBaugues/twilio-broadcast) but has since evolved into a little bit more. Sinatra Broadcast is a CRUD based app that uses the Twillio API to broadcast MMS messages to a group of contacts you create. Any inbound messages to your TWILIO_NUMBER gets routed to your personal number. Users can request to sign up to your broadcasts and Mailgun's API will handle the mail routing.

### Some Must Haves

This app does make a few assumptions. Have these guys handy to help deploy:

-  Twillio account & number
- Mailgun account
- Some type of S3 bucket for an image repo to force MMS to correctly concatenate on all mobile carriers. (Not an issue for SMS, but you'll have to change the configurations in app.rb)
- Heroku account (with an .env file to make deploying a breeze)

### Get Started

1. Git clone this badboy
2. Bundle install
3. Add ENV Details (There is a default.env you can use to create your .env file)
4. rake db commands (create, migrate & seed)
5. ruby app.rb 

Any questions or help, hit me up on Twitter @somethingkillr or mpope@somethingkiller.com or https://twitter.com/m_dimmitt
