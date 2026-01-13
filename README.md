# Performance Testing Project – Apache JMeter

## Project Overview
This project contains automated performance test scripts for BlazeDemo, a demo flight booking website. The test suite simulates realistic user journeys through the complete booking flow:

-Visit homepage
-Search for flights
-Select a flight
-Complete purchase with passenger details
-Receive confirmation

Test Application: https://blazedemo.com

## 🛠 Tools Used
- Apache JMeter
- HTTP Request Sampler
- Thread Groups
- Listeners
- HTML Reports

## 🧪 Test Types
- Load Testing
- Stress Testing

## 📊 Test Scenario
1. Baseline Test
Purpose: Validate functionality with minimal load
Threads: 1 user
Ramp-up: 1 second
Loop: 1
Goal: Ensure all requests work correctly

2. Load Test
Purpose: Test performance under expected load
Threads: 50 users
Ramp-up: 30 seconds
Duration: 1
Goal: Measure normal operating performance

3. Stress Test
Purpose: Find system breaking point
Threads: 100-200 users
Ramp-up: 120 seconds
Duration: 10 minutes
Goal: Identify maximum capacity


## 📈 Metrics & KPIs
Key Performance Indicators
1-Response Time
-Average response time for all requests
-Target: < 2 seconds under normal load

2-Percentiles (90th, 95th, 99th)
-90th percentile: 90% of users experience this time or better
-Target: < 3 seconds for 90th percentile

3-Throughput
-Requests processed per second
-Indicates system capacity

4-Error Rate
-Percentage of failed requests
-Target: < 1% under normal load, < 5% under stress

5-Latency
-Time to first byte
-Network and server processing time

## Sample Results Summary
=================================================================
Test: Load Test (25 users, 25s ramp-up)
=================================================================
Summary +      1 in 00:00:01 =    1.0/s Avg:   486 Min:   486 Max:   486 Err:     0 (0.00%)
Summary +    124 in 00:00:30 =    4.1/s Avg:   523 Min:   234 Max:  1456 Err:     0 (0.00%)
Summary =    125 in 00:00:31 =    4.0/s Avg:   522 Min:   234 Max:  1456 Err:     0 (0.00%)

Average Response Time: 522ms
90th Percentile: 845ms
Error Rate: 0%
Throughput: 4.0 requests/sec

## 🚨 Findings
- Response time increased with concurrent users

## 📁 Project Structure
- TestPlan: JMeter test plans (.jmx)
- Results: JTL result files
- Reports: HTML performance reports
- Screenshots: Dashboard images

##🔗 Resources
Apache JMeter Documentation
BlazeDemo Website
JMeter Best Practices
Performance Testing Guide

##📧 Contact

Author: Basma Mohamed Khass
Email: basmamhmdd22@gmail.com
GitHub: @basmamhmd
LinkedIn: (https://www.linkedin.com/in/basma-khass-04b205336/)
