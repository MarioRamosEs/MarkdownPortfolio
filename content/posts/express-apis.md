---
title: First approach to Express.js APIs
date: 2020-12-25
published: true
tags: ["I+D", "Personal Project", "Node"]
series: false
cover_image: ./images/ExpressJsHeader.jpg
canonical_url: false
description: "Simple examples of APIs with Express.js, using MongoDB and Azure SQL"
---

In the process of learning the Node backend technology (being used to NetCore), I have built two REST API templates with Express.js

- Express + Mongoose (Mongo DB)

    I consider it the perfect stack for a simple project that needs a fast prototyping or a lot of flexibility. DB hosted in MongoDB Atlas.
    [Source Code on GitHub](https://github.com/MarioRamosEs/ExpressMongoDb)

- Express + TypeScript + TypeORM (MS SQL Server in Azure)

    A much more professional and scalable stack (in my opinion), since both the project itself and the ORM are TypeScript based. DB hosted in Azure.
    [Source Code on GitHub](https://github.com/MarioRamosEs/ExpressTypeORM)

As a result of this, I can say that I really liked the way of developing a backend API with Node.js and would certainly love to implement all of this in some future project. The only downside that I could put to Express is that beacuse being so open, the learning process can be very confusing, since everyone does things differently.

However think Express is at the same level as Net Core, since it compensates its liitle disadvantages with a great community and support, and as today it is one of the most used modern backend frameworks.

Finally, I am aware that they are very basic examples that require the integration of many other factors (CORS, JWT, Cache ...) but this for the next one!