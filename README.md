# Digiplus
Digital signage software project in 4 ways

Global description :
This project is a global software for digital advertising. 
It comes in 4 ways :
- Server Sided (Back-end maintenance and managing interface for support / commercial team)
- Server Sided (Front-end for customers with private session / account and managing interface)
- Server Sided (Local main app with all core mechanics)
- Remote client (Local app on a NUC / BAREBONE in a passive way with scheduled sync protocol to main server)

Each part will be described in dedicated folders with complete documentation, visuals and draftworks as much as possible.


IMPORTANT :
Although development is based on free license principles, the work done to develop the entire tool remains the exclusive claim of the distributor.
Customers won't have access to software included in the core-server nor remote machine neither to the source-code. 
This part is a private creation that only Distributor can claim behavior.

------------------------------------------------------------------------
 Back-end (Server-sided) - FOR CUSTOMER SUPPORT & COMMERCIAL OPERATIONS 
------------------------------------------------------------------------

Global UX interface with 
- Account settings (session managing and security, licensing plan, user account informations, ...)
- Maintenance settings (Updates managing, Changelogs, remote actions, ticketing tool for customer support ...)
- Information settings (Newsfeed with teasers for incoming updates, videos links to YT with tutorials, salesplans...)
- LiveCheck [Like Nagios] (Global visualisation interface with realtime state of all remote machines sorted by customer account - possibly geolocalisation - triggers like mails to support team and customers where something wrong appears - disconnected from network, appcrash, catchlog...). 

------------------------------------------------------------------------
 Back-end (Server-sided) - FOR DEV AND SUPPORT ONLY 
------------------------------------------------------------------------

It's the core of the software. 
All the mechanics are there. Lot of technology used inside and constant optimizations to reach the best software using and comportment for customers and us of course.

------------------------------------------------------------------------
 Front-end (Server-sided) - FOR CUSTOMERS (MODULES)
------------------------------------------------------------------------

First, it's good to know each module will be described in a separate folder with all technical details and visuals inside. Here is a whole descritpion for all the UX interface customer-sided in a no exhaustive way. 

Global [CLEAN, GLITTER, ERGONOMIC and USER FRIENDLY] UX interface with
- Homepage with usual informations (Who's logged, latest newsfeed, All remote machines state, global infrastructure HEALTH with percentage and colour for best visibility)
- Left sided or top-sided menu with all access to functionalities.
- Access to the media library (all medias uploaded to the server in the customer cluster and  our library of proposed medias)
- Access to the playlists (all playlists created from the medias in the library)
- Access to the scheduling (a big schedule planner with all playlists with customizable vues - Day / Week / Months / Year) with full options to link to remote machines etc...
- Snapshots in real time (can call any remote machine in the infrastructure to catch what's playing in a T moment - Possibly connect with remote video preview)
- "Campaign proofing": Permit to create clean reports of advertising campaigns for R.O.I. optimizations or Marketing purposes
- "Triggering": Permit to create some special broadcast situations with added modules (Time, Light sensor, Temperature Sensor, Sound Sensor, software and API parsing sensors, ...) with ability to change the broadcast priority (OverCast ...)
- Support menu with access to pending tickets, basic actions (remote reboot ...) for customers who care about it.
- Licensing menu with all informations about license account used (depends on chosen package, ...) License status reminders and renewal deadlines...


------------------------------------------------------------------------
 REMOTE CLIENT - FOR DEV AND SUPPORT ONLY 
------------------------------------------------------------------------

Core embedded client-side software. 
It communicates in a scheduled timed way to the main server to check if there are new changes, files to download, files to update or new instructions to execute.
If no instructions, continue what's doing on and wait the next time to check.
If new instructions, catch and treat new ones, prepare in background and switch smoothly for transparent customer experience. After new instructions treated, send log for quality purposes.

