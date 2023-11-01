# feedbackloop-overheid.nl

Repository for Hackathon Feedbackloop Overheid.nl November 9 and 10, 2023.
Collaborating on a Smarter Citizen-Government Interaction.

(c) Staat Der Nederlanden 2023

## Introduction
Welcome to the Hackathon and Designathon Feedback Loop Overheid! This GitHub repository has been set up for the event on November 9 and 10, 2023. In this repository, you'll find all the resources you need to collaborate on innovative solutions. Thank you for helping us design the 'feedback mechanism' on overheid.nl.

Inside this repository, you'll discover annotated data and hyperlinks to the data that you can use to address the challenges presented during this event. Our goal is to make the government more responsive to citizen feedback and improve the user experience on government websites. Whether you're a software developer, data scientist, UI/UX designer, or service designer, this GitHub repository is your hub for the event.

We look forward to your contributions and innovative ideas as we work towards a more efficient and citizen-centric government. Let's make a difference together!

### Team collaboration
To contribute, create an account on GitHub ([Sign up here](https://github.com/)) and read this readme. Each team can fork this repository to work on their own design, making it an open source project. We encourage everyone to view and explore the projects within the repository after the hackathon has concluded.

### Disclaimer
The code within this repository primarily focuses on innovative solutions, design, and data science methods to improve government services and enhance citizen-government interaction. While extensive code review may not be the primary focus, the code serves as a foundation for the development of solutions and enhancements.

## Data annotation
The available data for the Hackathon/designathon includes all visitor interactions with the Rijksoverheid.nl website and the customer contact center around the theme of 'Education'. This theme is made up of various sub topics, listed at https://www.rijksoverheid.nl/onderwerpen/themas/onderwijs. The csv-files contain two weeks of Piwik clickstream data, the customer contact counting logs and the Google organic search keywords for all sessions that touched one or more sub-pages for these topics.

![Available data during Hackathon/Designathon](Images%20and%20files/Available%20data%20-%20Hackathon%20and%20Designathon%20Feedback%20Loop%20Overheid.png)

The table relations are visualized in this PDF: [Table relations](https://feedbackloopoverheidnl.blob.core.windows.net/feedbackloopoverheidnl/tables.pdf)

Below the specific datasets are described and a link to the dataset is provided.

### The datasets
#### Piwik sessions
This database comprises a set of fields, offering insights into visitor behaviour and interactions with a website, covering various aspects such as session details, visitor characteristics, and site engagement metrics. It includes data points like session timestamps, visitor types (returning or new), device and browser details, as well as referral source and campaign information. This dataset can be linked to the “Piwik events” dataset by the variables "pw_session_id" and “pw_visitor_id”.
This dataset primarily centers on sessions, visitor characteristics, and engagement metrics, providing insights into how users interact with a website at a session level.

![Piwik sessions](Images%20and%20files/Piwik%20sessions%20-%20Hackathon%20and%20Designathon%20Feedback%20Loop%20Overheid.png)

Link to the data: https://feedbackloopoverheidnl.blob.core.windows.net/feedbackloopoverheidnl/piwik_sessions.csv

#### Piwik events
This dataset provides information on website visitor interactions and event tracking, capturing various aspects of user behaviour and session details. It includes data points like session and event indices, visitor identifiers, timestamps, event types (including custom events, downloads, outlinks, page views, and searches), associated URLs and titles, previous and next event details, and page view metrics. Additionally, it encompasses contextual information such as website codes, date details, page types, ministerial departments, and subjects. This dataset can be linked to the “Piwik session” dataset by the variables "pw_session_id" and “pw_visitor_id”.
This dataset is centred on tracking visitor interactions and events on the website, offering more detailed insights into user behaviour and session-specific details.

![Piwik events](Images%20and%20files/Piwik%20events%20-%20Hackathon%20and%20Designathon%20Feedback%20Loop%20Overheid.png)

Link to the data: https://feedbackloopoverheidnl.blob.core.windows.net/feedbackloopoverheidnl/piwik_events.csv

#### Piwik search queries
This dataset consists of all search queries that visitors typed in the internal search in the website (e.g. https://www.rijksoverheid.nl/zoeken). Records are linked to the Piwik events table through the variable pw_event_id.

![Piwik search queries](Images%20and%20files/Piwik%20search%20queries%20-%20Hackathon%20and%20Designathon%20Feedback%20Loop%20Overheid.png)

Link to the data: https://feedbackloopoverheidnl.blob.core.windows.net/feedbackloopoverheidnl/piwik_search_queries.csv

#### Google organic
This dataset originates from Google Service Control and provides insights into Google web search activities, including user behaviour and website performance. It encompasses key data points such as search queries, associated page URLs, visitor countries, device types, registered clicks, impressions, and the click-through rate (CTR). Additionally, it includes position data indicating the page's ranking, search type (web or image), website codes, and timestamps (year, month, and day). 
This dataset aids in understanding how users interact with search results, optimizing web content, and evaluating the effectiveness of online presence.

![Google organic](Images%20and%20files/Google%20Organic%20-%20Hackathon%20and%20Designathon%20Feedback%20Loop%20Overheid.png)

Link to the data: https://feedbackloopoverheidnl.blob.core.windows.net/feedbackloopoverheidnl/piwik_search_organic.csv

#### Customer contact centre Rijksoverheid (phone number 1400)
This dataset records customer interactions with the 1400 customer contact centre of the Rijksoverheid, providing insights into various contact-related details. It includes information such as the date and time of the contact, the channel used for contact, the title of the last page on rijksoverheid.nl accessed by the agent to address the query, the associated ministry, and the subject. Additionally, the dataset covers details about the reason for contact as registered by the agent, the outcome of the contact, whether it was forwarded to the ministry's back office, and any associated forward code. 
This data can be used for monitoring and improving customer service interactions and outcomes within the government.
![Customer contact centre Rijksoverheid](Images%20and%20files/Contact%20centre%20Rijksoverheid%20(phone%20number%201400)%20-%20Hackathon%20and%20Designathon%20Feedback%20Loop%20Overheid.png)

Link to the data: https://feedbackloopoverheidnl.blob.core.windows.net/feedbackloopoverheidnl/contacts_1400.csv

