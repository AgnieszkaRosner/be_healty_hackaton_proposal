# TOPIC PROPOSAL FOR BE HEALTHY HACKATHON 13 - 14 OF APRIL 2019

## HACKATHON MAIN GOAL:

Create an app that is going to promote healhy life style

## PROPOSAL BASICS: HEALTHY ROUTE

- App is directed to all people capable of moving outdoor or those that can be supported by any one to spent time moving outdoor.
- App is directed to encurage walking, nordic walking, cycling, skating, running, sight seeing or just spending time on freash air, ect.
- App main goal is to help any one to find interesting area near or close to any place of person interest that:
    * Is interesting in terms of sight seeing, views, nature.
    * Is safe in terms of being properly described and having all necessary informations: lights, distance, slopes, accesability, route, time, ect.
    * Has trafic informations attached.
    * Has air pollution information attached.
    * Has weather information attached.
    * Contains propability factors for weather, trafic and pollution shown in simple chance of good and bad traits for at least few days.
    * Contains statistics of above factors.
    * Contains information how route is reviewed.
- App is based on information from users and those collected from IOT apis of air pollution sensors, weather services and GPS devices.
- App, if allowed by user, can track user on the route, collecting information from device, than user can contribute by sharing route information. Allgorithms on back end are than refering to IOT data on the server adding all information about shared route. User can describe route personaly and tags (tags are compared and reviewed with geo data). Main goal is that the most crucial information are calculated from IOT informations wildly avaliable. No Bies.
- User can load path from data collected.
- User is navigated by this app, can go from A to B and path is proposed. NOTE: Not crucial.
- Therefore based on above assumption App serves precise information about such place of outdoor sport related activities and can be safly categorized. So any person can get enought information to perform choosen sport activity.
- This approach alllows for safe, bias proof, encouraing, community based amd interesting for outdoor activity places sharing and searching.
- In today coulture We love to share and as World is moving faster and faster We have to value our time more, so We are prone to gather more information about what We want to do, to not wast any minut. We want to get the best avaliable for Us.
- Sharing based on combined personal and objective information helps Us to avoid information flaws and overlods, simplifying given information, but not hiding what is important.

## PROJECT STRUCTURE:

Project will be divided to main services:

- Back End - collecting, storing and serving data for front end.
- Front End - clinet site app for displaying all data.
- Iot Bridges - back end services that are bridging between Back End and IOT Apis and services collecting requested data and send them in DB without engaing Back End. Additionally will acts as solver for navigtion, ect. Algorithm is going to take navigated data, and compare them with IOT sensors data, than store in db warehouse.

## TECHNOLOGY PROPOSED:

For sake of quick and reliable project implementation lets use what We are good at:

- Back End: Java, Python, NodeJs, Rust (bacouse I am in love with her...). Choose one.
- DB MySql, for back end approach, MongoDb plus SQLite for Navigation Services
- Fron End: Angular7, Rx, Material. Lets start web frinedly, then going mobile if We have more time and people resources.
- Navigation Services: Rust has to be fast to calculate in real time. Java at least.
- IOT could be Python, but I am not sure, last time We had have 'fuck up' caused by Python not being type sefe, and We will not have enough time for writing tests for sure. TO CONSIDERATION.

## POSSIBLY NOT ALL COULD BE DONE WITH TEAM OF FIVE. SO MAIN FEATURES TO FOCUS ON ARE:

- Back End - Collecting and storing data from client.
- Back End - Serving to front end:
    * weather params (bridged)
    * air pollution params (bridged)
    * route params (cooordinate, slope, ect from db)
    * route description (from db)
    * tags (suitable for cycling, running, walking, ect)
    * stats (bridged for now) avaliable in [airly api](https://developer.airly.eu/docs#concepts.measurements)
    * in case of no sensor avaliable in some area around given coordinates use line interpolation strategy to some extent
- Bridges - Collecting data from IOT apis, do not have to be stored if response is based on fetching data and calculating them on the fly for clinet.Should work for medium treffic. Some info if necessary could be stored in no relational db as data warehouse or SQLite.
- Bridges - composing path from navigation coordinates (simplistic filter to not serve rubbish), calculates slope, time, works on the fly for front end. No backend relations, take data from db and send to client.
- Front End:
    * Main Page with map on full window and serch input on the top, in left or right corner accoutn info.
    * Map shows all added places and tags plus distance when mouse over place.
    * When place clicked goes to view showing path with robust description, and stats.
    * Drawing path could use native google earth api, open street maps, ect. Not chosen yet.

 ## IMPORTANT INFORMATION.

 - As has been learned from past hackathons under the hood app mechanics is not so important as:
    * idea at all.
    * design.
    * nice icons, pix, layout.
    * greate look on mobile phone and web.
    * projecct is fully working and We can prove it.
    * animations of something on the screen, 'it is alive' thing.
    * fancy pseudo jargon for used technology: Neuro Network, Artificial Inteigence, Genetic allgorithm. All teams will have this, so do We.
    * Better to not use hardware, so We are not designing device of IOT network, just using what is avaliable.
    * Getting jury involved - asking and using their ideas. Never outsmarting or discussing on subject that is not disovered good enough.
    * Knowing how app will pay bills for its existing maybe a valued project feature, but I am not insisting.
    * Some statistical information that project is not sucked out of a finger but solidly tested and researched is important feature.
    * Know how you are going to sell it and to whom... reserch competition, buyers, (juri is your client, investor or both).

### DEVELOPERS BEFORE, IN MOMENT AND AFTER JOB:

- having as much fun as possible.
- code as much as possible, it is what We love.
- focuse on presentation part of the app.
- cooperate as much as possible.
- do not disturb those working hard.
- listen to scrum master.
- avoid solving two problems at once, monotask.
- report problem to the team, ask for help, do not hide issues.
- get head phones and good music with you, have playlist, it will help filter outside noice, and there is always a lot going on.
- get phone or any mobile internet accespoint with you, do not count in good internet connection on hackathon.
- get hydrated.
- get somthing that will help you rest, f. e. sleeping bag,
- DO NOT blurt out our idea to other participants.

### SCRUM MASTER BEFORE, IN MOMENT and AFTER JOB:

- get it all planed, You are the best person to do so.
- solve all obstacles for your team, so team can code.
- check what is done on regular basis (every 2h sounds ok).
- manage them so they do not have to worry what next.
- do not alllow to let developers put somthing on 'production' when juri is comming to check, to much hustle is a terible idea.
- stress is performance killer, let it be fun + fun + fun.
- Project PRESENTATION is your job, assume developers sucks at it. From last hackathon I have learned, there would be nice to let you manage quetion answares with jury by pointing question to team member. It is worth trying. Other way We are heading in to informational chaos.
- buy your team an ice creams after all. An tell them they are the best.
