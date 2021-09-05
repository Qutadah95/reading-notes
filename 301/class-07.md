### Who is Roy Fielding?


Some guy. He's smart.He helped write the first web servers, that sent documents across the internet… and then he did a ton of research explaining why the web works the way it does. His name is on the specification for the protocol that is used to get pages from servers to your browser


### Why don’t the techniques that we use today work well when we need to be able to talk to all of the machines in the world?

Well, there's this concept that people are calling “Web Services” or "APIs". It means a lot of different things to a lot of different people but the basic concept is that machines could use the web just like people do.I don't mean that machines will be sitting down at the desk and browsing the web. But computers can use those same protocols to send messages back and forth to each other. We've been doing that for a long time but none of the techniques we use today work well when you need to be able to talk to all of the machines in the entire world.


### What is the HTTP protocol that Fielding and his friends created?


So anyway, HTTP—this protocol Fielding and his friends created—is all about applying verbs to nouns. For instance, 

### when you go to a web page, the browser does an HTTP GET on the URL you typed in and back comes a web page.

Web pages usually have images, right? Those are separate resources. The web page just specifies the URLs to the images and the browser goes and does more GETs using the HTTP protocol on them until all the resources are obtained and the web page is displayed. But the important thing here is that very different kinds of nouns can be treated the same. Whether the noun is an image, text, video, an mp3, a slideshow, whatever. I can GET all of those things the same way given a URL

### What does a GET do?

Our brains are somehow smart enough to know that the same verbs, like GET, can be applied to many different nouns. Some verbs are more specific than others and apply only to a small set of nouns. For instance, I can't "drive" a cup and I can't "drink" a car. But some verbs are almost universal like GET, PUT, and DELETE.

### What does a POST do?

From what I understand of this article polymorphism applies to REST by saying that we can have multiple nouns, ie things to be selected that have the same verb applied to them I.E. POST GET PUT DELETE. Which relate to SQL with INSERT, SELECT, UPDATE, DELETE.

### What does PUT do?

I can PUT a cup, I suppose... but you can't DELETE a cup.
Well, okay, but you can throw it away. Close enough, right?

### What does PATCH do?

 Exactly. Each of the systems would retrieve information from each other using a simple HTTP GET. If one system needs to add something to another system, it would use an HTTP verb of POST. If a system wants to replace something in another system, it uses an HTTP verb of PUT, or, to do a partial update, it'll hopefully use PATCH. The only thing left to figure out is what the data models should look like.