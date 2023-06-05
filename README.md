# MESSAGE BOARD APP 

## App logic
1. Initialize the app by using Express generator
2. I create 2 routes: 
    - One for the '/': home page, where I display all messages (by using pug's iterative each syntax) 
    - One for the '/new' new message page: where I am displaying a form which takes a user name and a message and sends a POST HTTP request
3. For accessing the content of my request, I can use ``req.body`` inside my ``post()`` method, along with the name of the input field.
4. Finally, I am pushing the content in my messages array, and redirecting to the homepage to display the new messages.

## Deployment
1. Here I am learning how to use a PaaS for the first time. (Platform as a Service, examples: [Heroku](https://www.heroku.com/), [Railway](https://railway.app/), [Render](https://render.com/) and [Fly.io](https://fly.io/))
2. The main difference between PaaS and other deployment options (i.e GitHub pages) is that in GitHub pages you cannot host NodeJS applications due to their dynamic nature. Such as in Twitter, every user will see different content when they access the app, compared to a static webpage where every user sees the same content. 
3. The ``Instance`` means the single instance of my app running of one time, like the localhost when I am running it.
4. The ``Database`` access is the most important thing that the PaaS providers give. Very easy, very important. Even automatic backups. Peace of mind. 
5. PaaS providers give a randomized domain name when I will first deploy, but if I want a custom domain I will have to buy it from a domain registrar like [Porkbun](https://porkbun.com/) or [NameSilo](https://www.namesilo.com/)
6. I will be deploying this on Fly.io. [Live](https://messaging-board-jana.fly.dev/)