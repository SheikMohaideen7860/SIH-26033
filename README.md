# Smart India Hackathon Workshop
# Date:25/11/2026
## Reference Number:26018610
## Name:Sheik Mohaideen M

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
.Expected Solution: Create a digital marketplace that:

* Connects farmers/FPOs directly with consumers and bulk buyers.
* Provides logistics support.
* Uses AI for demand forecasting and route optimization
Benefits:

• Better prices for farmers.
• Lower prices for consumers.
• Reduced supply chain inefficiencies.

## Proposed Solution
1. Detailed explanation of the proposed solution

The Local Farm-to-Consumer Digital Supply Chain is an online platform that lets local farmers sell their produce to local consumers. Since widely used web technologies are the building blocks of this system, the application is relatively easy to prototype and scale. The system has three key components, interfaces, and workflows for:

* Farmers to manage their listings and fulfillment.
* Consumers to search and place orders.
* An administrator to manage user accounts.

The system uses a seven step workflow to process an order from farm listing to delivery and payment:
The seven steps are: 
1. Farmers register and create a listing to advertise their products for sale.
2. Farmers post the details of the products they have for sale including the unit price, quantity available, expected date of harvest and estimated availability. 3. Consumers search and select the products they need, enter their delivery address and time slot.
4. Consumers place an order and reserve the product before the harvest date.
5. The farmer is not allowed to sell more of the product than is available to reserve.
6. Similar orders for the same product in the same area and within the same time slot are grouped together.
7. Lastly, the product is delivered to the collection point.

The system then suggests a local delivery partner or a collection point based on the travel distance and cost to the selected area. After delivery and settlement of the orders, the farmer is free to list more products for sale.

2.How it addresses the problem:
* Direct farmer-to-consumer interaction: Farmers can now fulfill pre-harvest orders, digitally record orders and payments, and ultimately meet consumer demands directly.
* More options for consumers: Local produce listings, with prices and harvest dates, and home delivery options are provided for consumers.
* Less expensive delivery: Orders are grouped by area and time, and delivery costs are shared among customers in the same group, as opposed to individual orders being delivered to each customer’s house.
* Order adjustments: Orders are immediately reflected in the seller’s stock inventory.
* More perishable stock: Transport windows and order scheduling are prioritized for more perishable produce to ensure the seller does not experience a loss in quantity or quality of the produce.
* Trust: Consumers are assured quality and quantity of the product, as they receive order confirmations, tracking deliveries, and have the option to request a refund.
* Basic interface: The simple and straightforward interface in various local languages eases farmers’ use of the platform.
* Price comparison: To compare mandi prices, users can also look up the daily rates on AGMARKNET/Open Government Data.
* Orders for delivery partners: Local delivery partners are also given an opportunity to provide the service for grouped orders.

3. Innovation and Uniqueness of the Solution:

Digital agricultural trading has gained traction in India with platforms like e-NAM and Farmpal. Solutions already available in the market cover order, payment and delivery management and demand forecasting and route optimization. This prototype will not claim that there are no digital agricultural solutions, and instead will explore if incorporating the following three features in a single, easy to use workflow would improve the situation for a particular farming community:

* Farmers make advance reservations and track the reservation against the quantity farmed
* Orders are grouped together by neighborhood, time slot, product and capacity to transport
* Orders are tracked in real time by the customers, farmers and delivery partners.
The focus of this solution is on a single locality to begin with to assess delivery costs, order fulfillment rates and quantity of unsold produce. Based on these findings it will be decided if the solution should be implemented in other localities. Though these are expected benefits, a structured pilot will allow for a more accurate assessment of whether the application has reduced costs and post-harvest losses for farmers.

The features “Easy adoption” and “Delivery partners” are from your Feasibility and Impact sections and thus, align with your proposal.
## Technical Approach
Technologies to Be Used:
Developing a dependable platform for local agricultural ordering does not require proprietary or overly complex software. The proposed system relies on widely used, well-documented web technologies that support clean prototyping and straightforward future scaling. The core technology stack selected for each layer of the application is as follows:

* Frontend: HTML, CSS, and JavaScript
* Backend: Python with Django
* Database: SQLite for the prototype; PostgreSQL for future deployment
* User Authentication: Django authentication and role-based permissions
* Mapping and Routes: OpenStreetMap with a suitable routing service
* Market-Price Information: AGMARKNET / Open Government Data, subject to data-access conditions
* Payment: Simulated payments in the prototype; a compliant payment gateway for deployment
* Development Tools: Visual Studio Code, Git, and GitHub

To keep day-to-day operations organized and secure, the system is structured around three primary user interfaces: a farmer interface for managing produce and fulfilment, a consumer interface for browsing and placing orders, and an administrator interface for account verification, oversight, and support.

Methodology and Process for Implementation:
The platform operates through a structured seven-step workflow that carries an order from initial farm listing through final delivery and settlement:

1. Farmer Registration: Farmers create accounts on the platform and provide basic identity and farm details for verification before publishing listings.
2. Product Listing: Verified farmers list their available fruits and vegetables along with the quantity on hand, price per kilogram, harvest date, and expected availability window.
3. Consumer Ordering: Consumers browse local listings, select the products and quantities they need, enter their delivery address, and choose a preferred delivery slot.
4. Advance Demand Reservation: Consumers can reserve produce before the expected harvest date. The system tracks every confirmed reservation against the farmer's declared quantity so available stock is never oversold.
5. Smart Order Grouping: Rather than dispatching each order separately, the application groups compatible orders by delivery neighbourhood, time slot, product availability, and delivery capacity.
6. Delivery Allocation: Based on travel distance, available capacity, and estimated cost, the platform suggests either a local delivery partner or a shared collection point.
7. Order Tracking and Settlement: Consumers track order status through each stage while farmers and delivery partners update fulfilment progress. Payments and any required refunds are recorded through the selected payment process.

System Workflow:
The six-stage operational sequence connecting farmers, consumers, and delivery partners within the application:

1. List Produce: Farmer lists available produce
2. Place Orders: Consumers place orders
3. Confirm Orders: Check stock & confirm orders
4. Group Orders: Group by location and time
5. Assign Delivery: Partner or collection point
6. Complete Order: Deliver produce & complete

Working Prototype and Demonstration Plan:
The initial working prototype is designed to verify that the core ordering and grouping workflow operates reliably end to end. During demonstration, the prototype will show:

* Farmer account registration and produce listing management.
* Consumer browsing, shopping cart handling, and order placement.
* Advance demand reservations tracked directly against available stock.
* Automated order grouping across a sample local neighbourhood.
* Estimated delivery cost calculation alongside a suggested delivery route.
* Order-status updates and an administrator oversight dashboard.

At the prototype stage, payments will be simulated and routing will run on sample delivery data. Real payment gateways, live GPS location tracking, and external market-data integration can be added once the core workflow functions reliably.

## Feasibility and Viability
Feasibility Analysis:
* Technical Feasibility: The application can be developed using widely available web technologies. Django's authentication and permission system natively supports user accounts, groups, and access controls, making it well suited for separating farmer, consumer, and administrator roles.
* Economic Feasibility: A working prototype can be built at minimal cost using free, open-source development tools and a local SQLite database. Early testing can rely on sample products, simulated payments, and a small delivery zone.
* Operational Feasibility: Rollout can begin with a limited group of farmers and consumers in a single locality. Initial orders can be fulfilled by participating farmers or local delivery partners without investing in a dedicated transport fleet.

Potential Challenges and Risks:
Transitioning from a software prototype to real local farm trade involves practical operational and adoption challenges:

* Unreliable Stock Information: Farmers may sell produce offline at local markets after listing it online, creating inventory mismatches.
* Delivery Costs: Delivering individual small household orders separately can become too expensive to sustain.
* Perishable Products: Fresh fruits and vegetables deteriorate rapidly; any delay in pickup or transit reduces freshness and saleable quantity.
* Trust and Quality: Consumers need consistent confidence that the produce delivered matches the quality and weight listed online.
* Digital Accessibility: Some farmers may have limited prior experience with web or mobile applications, which can slow adoption.
* Competition: Existing agricultural trading platforms, such as e-NAM, already provide several relevant digital services in India.

Strategies for Overcoming These Challenges:
Each risk can be mitigated through practical operational rules and a gradual pilot rollout:

* Update inventory immediately when orders are confirmed and automatically block purchases that exceed remaining available stock.
* Group orders by locality and delivery time slot to share transport costs across nearby buyers.
* Establish realistic delivery windows and give scheduling priority to highly perishable produce.
* Maintain user trust through clear order confirmations, step-by-step delivery tracking, responsive complaint handling, and defined refund procedures.
* Offer a simple regional-language interface along with assisted onboarding during farmer registration.
* Pilot the application in one locality first, comparing delivery costs, fulfilment rates, and unsold quantities before deciding to expand.


## Impact and Benefits
 Potential Impact on the Target Audience:
How the proposed platform is designed to support each primary group within the local supply chain:

* Farmers: Direct access to local consumer demand, advance pre-harvest reservations, and clearer digital records of orders and earnings.
* Consumers: Easier access to local produce listings, transparent prices, harvest-date details, and home-delivery options where available.
* Local Delivery Partners: Structured opportunities to fulfil grouped orders and coordinate efficient deliveries within defined local service areas.

 Benefits of the Solution:
* Social: Improves community access to fresh agricultural produce and practical digital ordering services.
* Economic: Helps reduce repeated small delivery trips while giving local farmers an additional channel to reach nearby customers.
* Environmental: Stronger demand planning paired with fewer unnecessary trips may help reduce avoidable food waste and transport emissions.
* Operational: Provides organized digital records covering inventory, customer orders, payments, and delivery status.
* Long-Term: Creates a base that can expand over time to additional localities, farmer groups, local restaurants, and other bulk buyers.

Evaluation Note: These are expected benefits rather than proven outcomes. A structured local pilot study is needed to measure whether the application actually lowers delivery costs and reduces post-harvest waste in practice.

## Research and References
Research Work:
Reviewing existing agricultural platforms and published policy research helps establish what is already available in India and where this proposal can make a distinct contribution:

* National Agriculture Market (e-NAM): A government-backed electronic trading platform (e-NAM) supporting market access, price discovery, and related agricultural services. Its adoption demonstrates that digital agricultural trading is already well established in India.
* AGMARKNET and Open Government Data: Public market-data portals (AGMARKNET Daily Price and Arrival Report) publish daily wholesale agricultural prices, including minimum, maximum, and modal rates, which could help users compare local listing prices against reported mandi rates.
* Agricultural Supply-Chain Research: A Reserve Bank of India (RBI) Bulletin study published on 18 January 2024 examined farmers' share of consumer prices and the role of market infrastructure in supply-chain efficiency, providing a useful empirical foundation for studying price differences and intermediary costs.
* Farmpal Case Study: In its Compendium of 75 Agri Entrepreneurs and Innovators, NITI Aayog describes Farmpal's farm supply-chain model covering customer ordering, payments, delivery management, demand forecasting, and route optimisation.

Reviewing these existing capabilities helps ensure the proposed application defines a realistic, distinct contribution.

Identified Research Gap: Rather than claiming that no digital agricultural applications exist, this prototype investigates whether combining advance consumer reservations, neighbourhood-level order grouping, and transparent fulfilment in one simple workflow can improve outcomes for a selected local farming community.

References:
1. National Agriculture Market (e-NAM). Government of India Agricultural Trading Platform. https://enam.gov.in/
2. AGMARKNET / Open Government Data Platform India. Daily Price and Arrival Report, Agricultural Market-Price Dataset. https://agmarknet.gov.in/daily-price-and-arrival-report
3. Reserve Bank of India (Department of Economic and Policy Research). Agriculture Supply Chain Dynamics: Evidence from Pan-India Survey. RBI Bulletin, 18 January 2024. https://www.rbi.org.in/Scripts/BS_ViewBulletin.aspx?Id=22326&utm
4. Django Software Foundation. User Authentication in Django, Authentication and Permissions Documentation. https://docs.djangoproject.com/en/6.1/topics/auth/
5. NITI Aayog. Compendium of 75 Agri Entrepreneurs and Innovators (Farmpal Case Study). https://www.niti.gov.in/node/555
