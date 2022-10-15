# Vagmi Mudumbai

[Github](https://github.com/vagmi) | [LinkedIn](https://www.linkedin.com/in/vagmi/) | [Website](https://vagmi.ca) | [Talks](https://www.youtube.com/playlist?list=PLVbkwm50L3Yxy2LcthD8ln3JfvWVdF7Am) | [Blog](https://vagmi.medium.com/)

Technology leader with over 20 years of experience building software and software teams. I enjoy building software as much as I enjoy building great teams. 

**Skills**: Go, Rust, Typescript, Postgres, Distributed Systems, TDD, Kubernetes, Docker

## Tarka Labs, A division of Sedin Technologies

2014-onwards

I‘ve built this organization into a vibrant team of 35 members worldwide. Over these years, I have worked on the following projects as an individual contributor. To know more about the portfolio of the projects done by Tarka Labs, I’d recommend that you visit our [portfolio page](https://tarkalabs.com/projects/).

### Tunecore - Platform Architecture (Distribution)

(Ruby on Rails, Go, PostgreSQL, AWS services)

Tunecore is an indie music distribution company. It takes albums and singles from artists all around the world and distributes them to over 50 music stores like Apple, Spotify, Youtube Music, Amazon Music, etc. It paid out over $1 bn to artists for the year 2021. 

I helped them split up a 10-year Rails monolith based on Rails 3 into different services. We built the core distribution service into its own service on Rails 6. We also split the transcoding piece and moved it to AWS lambda. We evaluated AWS elastic transcoder and AWS elemental media file convert. We instead used Lambda with a statically compiled FFmpeg layer. This approach roughly had a 5x-6x throughput increase over the elastic transcoder. We also moved the actual SFTP delivery of the files to Go and refactored the job queue to three independent steps. This resulted in over 70% reduction in the infrastructure costs for the production cluster.

### Moove - (Location and Clustering services)

(Ruby on Rails, Android, Go, React, Google Maps SDK, OSRM)

Moove was a startup in India focused on providing transport and employee mobility solutions for large software companies. The companies in India run various shifts 24/7 and provide pick and drop services for their employees. This involved building both the driver and the employee app. This is very similar to the Uber app sans the payment.

The core location and the route planning were built with Rails. This was inefficient and unreliable. We moved the location service alone to use Golang and moved from long polling HTTP endpoints to using websockets. I also helped batch calls from the android app to send data efficiently to the backend.

We moved away from using Google Maps SDK for route planning to using OSRM. Google Maps SDK even with its distance matrix endpoints was too slow for the scale of Moove. We moved to OSRM for route planning and visualized the routes on Google Maps.

### PacketMedia - (SMS Marketing tool)

(Golang, Elixir, Phoenix, Postgresql, React)

PacketMedia was SMS marketing solution and used a Go service for interfacing with SMSC gateways and used a Phoenix app to manage campaigns and the CRM dashboard.

### Modus - (Vehicle fleet tracking)

(React, Google Maps, Rails, Elixir, Postgres)

We used React over a Rails app for vehicle fleet tracking. We used Elixir for the location service. The data for locations came from an OBD device plugged into the vehicle. The OBD device published the GPS coordinates and other telemetry information like acceleration and so on to the location gateway.

## Independent Consultant

2013-2014

I was the consulting CTO of Reduce Data and was working building the keypass system for Qube cinemas. I also conducted independent workshops and trainings on several Javascript frameworks and techniques like Test Driven Development.

### Qube Cinemas - Keypass

(Node, AngularJS, JS)

It was a small microservice and a dashboard app for Qube cinemas to manage and pull down keys for the DRM movie projectors.

### CTO, Reduce Data (Ad Tech)

(Java, Netty, Clojure, Weka, Ember, Play, PostgreSQL, Cassandra)

Built a demand side Real Time Bidding platform. Our campaigns were managed with a Java Play app on a PostgreSQL database. Our click stream information was stored in Cassandra. We sampled the data and built ensemble models on Weka (SGD, Random Forest) to classify potential clicks. We used Weka to ensure that the model on inference is very light and runs in the process. 

## Thoughtworks - Lead Consultant

2012-2013

### GruppoPAM - Buyer Dashboard

(Java/Spring, JDBI, Postgres, Teradata, Rails, jQuery, D3, Marionette)

We built a buyer performance dashboard for an Italian retail chain. It allowed them to view the performance metrics for various lines of products over different periods. All the heavy lifting was done by the Teradata and the Spring Java layer. Rails was used for preference management and to build custom reports. We used D3 for all the data visualization.

### GruppoPAM - Assortment Planning

(Clojure, PostgreSQL, Neo4j)

This was a microservice that did what-if analysis on different profitability profiles based configuration such as logistics, format of the store, SKU cluster membership and so on. This generated the assortment based on this configuration and projected profitability based on past metrics. This was a part of the replatforming efforts. The existing solution was written as a series of batch jobs on top of Oracle. It took over 6 hours of runtime to expand to the SKU level. Expressing them as a series of Graph expansions helped us arrive at the effective assortment much faster in the order of seconds. It allowed buyers to quickly create multiple what-if scenarios and aid in their contract negotiation accordingly.

## Dharana Software / Artha42 Software - CTO & Co-founder

(2009-2012)

I ran a digital agency building web and mobile applications. I also conducted Ruby on Rails trainings both as independent and in-house training workshops.

### AuditionMagic

(Rails, jQuery, HTML5 Video, PostgreSQL) - A HTML5 based in-video tagging solution.

### Apollo HealthHiway

(Rails, MongoDB, jQuery) - A white labeled personal health record system with integration points to several HIS systems.

## SAP Labs India - Associate Architect

(2004-2009)

I was a part of the developer tools ecosystem and was on a team building Visual Studio VSIP extensions and Eclipse (SAP Netweaver Development Studio) plugins for SAP’s development tools. Implemented a development framework on Adobe Flex closely mimicking Eclipse’s OSGi model for plugins. 

(Java, C#, Eclipse, Eclipse RCP, Visual Studio VSIP, C++)

## SlashSupport - CSS Corp Company - Engineer

(2003-2004) Was a part of the development support team for InstallShield suite of products.

## Bajaj Allianz General Insurance - IT Coordinator

(2002-2003) Was a part of the IT team building in-house tools with VB and SQL Server.

## Education

MBA - SP Jain Institute of Management and Research - 2007-2009
M.Sc (IT) - University of Madras - 2002-2003
B.Sc (Physics) - University of Madras - 1998-2001