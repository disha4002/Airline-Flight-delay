### ✈️ AIRLINE AND FLIGHT DELAY ANALYSIS
## Project Background:
Airline delays and cancellations can significantly affect passenger experience, operational
efficiency, and airline performance. With multiple factors such as weather conditions, carrier
issues, security delays, and late aircraft arrivals contributing to disruptions, analyzing flight
data can help identify patterns and areas of operational improvement.
The Airline Delay Dataset includes records for 5,000,000+ commercial airline flights in 2015,
compiled for the U.S. DOT Air Travel Consumer Report. Each record represents a single
flight, including the airline name, flight number, origin/destination airport and flight distance,
as well as scheduled/actual departure and arrival times.
The analysis focused on comparing airlines, understanding the distribution and causes for flight
delays, monitoring cancellation rates, and examining overall flight performance.
## Executive Summary:
Overview of Peak Findings:
The line chart illustrates the average arrival and departure delays of flights throughout
2015. Departure delays generally remain higher than arrival delays across most months. Delays
reach their first major peak in February, followed by the highest point in June, when average
departure and arrival delays reach 14.0 minutes and 9.6 minutes, respectively. Delays then
decline during the second half of the year, with arrival delays briefly falling below zero in
September and October. Toward the end of the year, delays rise again during the holiday season,
reaching 11.8 minutes for departure delays and 6.1 minutes for arrival delays in
December.
Airlines Page:
Overview of Airline Performance:
Spirit Air Lines and Frontier Airlines record the highest average arrival delays (14 and 13
minutes respectively), nearly double the delay seen at JetBlue and Atlantic Southeast (7
minutes each). In contrast, Southwest Airlines and Delta lead in on-time flight volume
(1.03M and 0.76M respectively) — though this reflects their larger overall flight volume as
much as punctuality. Smaller carriers like Virgin America and Frontier show comparatively
fewer on-time flights, consistent with their smaller fleet size and higher average delays.
Airport Page- Flight Delay Tab
Overview of Delay Concentration by Airport:
Chicago O'Hare International Airport accounts for the highest total delay minutes (2.38M),
nearly 50% more than the next-highest airport, Dallas/Fort Worth (1.61M). Together, the top 5
airports (O'Hare, DFW, Denver, LAX, and George Bush Intercontinental) account for a
disproportionate share of total delay minutes — highlighting that delays are concentrated at a
small number of high-traffic hub airports rather than spread evenly across the network.
Airports Page – Busiest Airport Tab:
Overview of Traffic Volume by Airport:
Hartsfield-Jackson Atlanta International Airport is the busiest named airport in the dataset
(0.35M flights), followed by Chicago O'Hare (0.29M) and Dallas/Fort Worth (0.24M).
## Key Insights:
June recorded the highest average flight delays, with departure and arrival delays reaching
14.0 and 9.6 minutes respectively.
Departure delays were generally higher than arrival delays, indicating that many delays
originated before or during the departure process.
December experienced another significant increase in delays, potentially reflecting
increased holiday-season traffic and operational pressure.
September and October recorded negative average arrival delays, suggesting that flights
arrived slightly ahead of schedule on average.
Airline performance varied considerably, allowing better- and worse-performing carriers to
be identified based on delay and cancellation metrics.
Delay-cause analysis highlighted the contribution of carrier issues, weather, NAS, security, and
late-arriving aircraft to overall disruptions.
Cancellation rates provided an additional measure of airline reliability, complementing
average delay metrics.
The analysis demonstrates how SQL and Power BI can transform raw flight records into
actionable insights about airline operational performance.
## Actions and Recommendations:
Address seasonal peak-period congestion:
Since delays peak sharply in June and again during the December holiday season, airlines and
airports should proactively increase staffing, ground crew capacity, and buffer time in flight
schedules during these two windows rather than applying uniform scheduling year-round.
Investigate departure-side bottlenecks:
 Since departure delays consistently exceed arrival delays, the root causes likely lie in predeparture processes (boarding, ground handling, aircraft turnaround) rather than in-flight or air
traffic control factors. A focused audit of gate operations and turnaround time at high-delay
airports would likely yield faster improvement than schedule padding alone.
Prioritize interventions at high-concentration hub airports:
 Since delay minutes are heavily concentrated at a small number of airports (O'Hare, DFW,
Denver, LAX, George Bush Intercontinental), operational improvements — additional runway
slots, better gate allocation, improved ground traffic flow — will have outsized impact if
focused on these hubs rather than spread evenly across the network.
Benchmark underperforming carriers against top performers:
 Airlines with disproportionately high delays relative to their fleet size (e.g., Spirit, Frontier)
should study the scheduling and turnaround practices of better-performing carriers with similar
route profiles, rather than only being compared against larger carriers with different operational
scale.
 Break down delay causes to target root fixes:
 Since delays stem from multiple distinct causes (carrier issues, weather, NAS, security, latearriving aircraft), airlines should treat these as separate operational levers — e.g., weatherdriven delays call for better contingency scheduling, while carrier-caused delays point to
internal process issues that are more directly controllable.
Use cancellation rate alongside delay metrics, not in isolation:
 Since cancellation rate captures a different failure mode than average delay, airports and
airlines with strong average-delay numbers but elevated cancellation rates should be flagged
separately — a low average delay can mask a policy of cancelling rather than delaying
problematic flights.
Resolve the missing-airport data gap before further analysis:
A meaningful share of records, lack an airport identifier (shown as "(Blank)" in the Busiest
Airports view). This should be investigated and cleaned, since it currently limits confidence in
airport-level comparisons and should be flagged as a known data-quality limitation if it can't be
fully resolved.
