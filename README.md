# fortum-russian-projects
This work showcases some of the assignments I did for an advanced course on Excel, PowerQuery and Excel VBA.
You have applied for an investment analyst position to Finnish energy company Fortum. According to the call, one of your main tasks would be to plan and supervise Fortum’s renewable energy investment program in Russia. You just got a message that they are inviting you to the job interview. And you want to impress them and to leave no choice but to give this position to you.
Fortunately, you have found that Russian energy authorities openly publish data on renewable energy projects auctions. So you can analyze that data in order to get the feeling of the current state of Fortum’s renewable energy investment program, Fortum’s competitors, Russian renewable energy market development, etc.
Possessing such information would definitely make you outstanding among other job applicants.

### GET ACQUAINTED WITH THE RAW DATA
Let’s first have a look inside the first file 2013_solar.xlsx

* Company - The name of a company who is responsible for project implementation.
* Project-  The project name, given by the company.
* Code - The code, given by the energy authority (this started in later auctions, so here it’s empty).
* Region - Russian region where the project is planned to be built.
* Type - Technology type - solar, wind or small hydro.
* Auction - Year of the auction on which the project was selected.
* Planned commercialization date - The date when a project is planned to be completed and starts producing electricity.
* Planned installed capacity, MW - The size of the project, traditionally in the energy industry measured by the installe capacity.
* Planned capital expenses, rub/kW - Initial investment of a project, note, already divided by the project size – so it is per unit of the size.

### CREATE A POWER QUERY TO
i. Consolidate all the auction results.

ii. Merge it with ‘region’ file. This will allow you to break down the project data by energy zones (socalled unified power systems - UPS).

iii. Merge it with ’UPS’ file. You happen to find also some useful data about overall capacity demand (that is an approximation of how much power investment will be needed in different areas) and electrical grid conditions (that might affect the realization of the investment project). This data only for UPSs, but you want to have it together with the final data because that would help you to judge where to direct the Fortum’s investment focus for the future. 

### BUILD AN INTERACTIVE DASHBOARD
Include the following graphics.
i. How much (in terms of installed capacity) are there renewable energy projects, when they are planned to be built (commercialization date), and how does it look for different technology types (wind, solar, hydro)?

ii. Same information, but broken down not by technology type, but by auction year. This chart will tell you when market actors brought their projects to the auctions. The point here is that every auction selects projects to-be-built in a four-year ahead period. Therefore two projects with planned commercialization in 2020 could originate from auctions of different years. This information is important because it reflects actual decision-making.

iii. Market participants, who are they and which market share do they have. What is Fortum’s place in the market? Who are its main competitors?
iv. Total installed capacity broken down by UPS (and could be also by technology type) will give you an idea of where those projects are building.
v. Information on capacity demand across UPSs.
vi. Information on grid conditions across UPSs.
vii. Show also the average cost by commercialization year and by technology, this would tell you how the cost of the technology is developing over time independently of the project size.

### FURTHER ANALYZE DATA WITH DATA ANALYSIS TOOLPACK
For this task, you need the raw data but broken down by technology type.
With data analysis toolpack, get descriptive statistics for all technology types and place them on one separate sheet called ‘Descriptives’. Observe the differences in mean, standard deviation and other statistics.
Check if there is any linear relationship between the commercialization year and average costs. Also, place the results to one sheet called ‘Regression’. Find the regression coefficient (highlight it with color). What does it tell you? How different is it for three technology types?

### GET THE INSIGHT FROM DATA
i. What is the overall share of Fortum on the Russian renewable energy market?
ii. What types of projects (wind, solar, hydro) does it have(plan)? Where and when they are (will be) built?
iii. What is the decision pattern of Fortum in the wind sector? When and how much (in terms of capacity) wind projects Fortum brought to the auction in Russia? What could it mean?
iv. Who are the main competitors of Fortum in this market? Are these competitors operate in the same UPSs as Fortum?
v. What about project costs? How do they develop over time and is there any difference across technology types? (this one based on data analysis toolpack results too)
vi. Based on all available information, including info on UPSs, in which energy zones and with which technologies you would recommend Fortum to proceed in the future?

