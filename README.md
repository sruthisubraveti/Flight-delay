Predict Flight Arrival Delays 

The aviation industry in the USA faces a pressing challenge with the persistently high rate of flight delays over the past decade. The increasing frequency and duration of flight delays pose significant challenges to passengers, airlines, airports, air traffic control (ATC), and ground transportation services. These delays result in missed connections, disrupted travel plans, additional costs, and stress for passengers. For airlines and airports, delays lead to financial losses, operational disruptions, and damage to reputation. Air traffic control faces increased workload and safety risks, while ground transportation services experience disruptions, overcrowding, and increased costs. According to recent statistics, flight delays cost the industry billions of dollars annually, with an estimated loss of over $25 billion in revenue each year. It is imperative for the aviation industry to address this issue effectively to minimize financial losses, enhance operational efficiency, and improve customer satisfaction to secure long-term profitability and business growth. 

Through our project we aimed to predict the delay in flight arrivals based on data collected over a decade from 2013 to 2023. After studying the data, we determined post-covid years would be the appropriate time series data to use to build a regression model to predict an approximate delay in arrival for a flight (minutes). 

Data Source and pre-processing 

Data Source 

Bureau of Transportation Statistics: Airline On-time and Delay Causes 

https://www.transtats.bts.gov/OT_Delay/OT_DelayCause1.asp 

The dataset comprises information pertaining to delays in flights because of various reasons. Below is a concise overview of the dataset's variables: 



year : Year in the format YYYY (e.g., 2018) 

month : Month in the format MM (eg.,12) 

carrier : The two-character designator for the carrier/airline. 

carrier_name : The full name of the carrier/airline. 

airport : The three-character designator for the arrival airport. 

airport_name : The full name of the arrival airport. 

arr_flights : The total number of arriving flights for the carrier-airport pair for the month specified. 

arr_del15 : The number of arriving flights that were delayed. Delayed is when a flight arrives more than 15 minutes later than the scheduled arrival time. 

carrier_ct : The number of arriving flights delayed due to a carrier issue. 

weather_ct : The number of arriving flights delayed due to a weather issue. 

nas_ct : The number of arriving flights delayed due to a national air system issue. 

security_ct : The number of arriving flights delayed due to a security issue. 

late_aircraft_ct : The number of arriving flights delayed due to an earlier late arrival of an aircraft. 

arr_cancelled : The number of cancelled flights. 

arr_diverted : The number of diverted flights. 

arr_delay : The total number of delayed minutes due to delays. 

carrier_delay : The total number of delayed minutes due to carrier issues. 

weather_delay : The total number of delayed minutes due to weather issues. 

nas_delay : The total number of delayed minutes due to national air system issues. 

security_delay : The total number of delayed minutes due to security issues. 

late_aircraft_delay : The total number of delayed minutes due to earlier later arrival of aircraft. 

<img width="729" alt="image" src="https://github.com/sruthisubraveti/Flight-delay/assets/172334062/87f3d2fe-24fa-41d2-9a1e-5dee85b38f84">
<img width="485" alt="image" src="https://github.com/sruthisubraveti/Flight-delay/assets/172334062/7625d3e0-5c06-4609-ba4c-daeedd3dc8f1">



