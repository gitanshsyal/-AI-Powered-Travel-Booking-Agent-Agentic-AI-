# AI-Powered-Travel-Booking-Agent-Agentic-AI
-------------------------------------------------------------------------
## Project Overview
-------------------------------------------------------------------------
The Travel Booking Agent is an AI-powered agentic application designed to help users plan their trips through intelligent tool calling.

Instead of manually searching for flights, hotels, calculating expenses, and preparing travel plans, users can interact with an AI agent using natural language.

The agent understands user requirements, identifies the appropriate tools, executes them, and generates a personalized travel itinerary.

## Problem Statement
---------------------------------------------------------------------------
Planning a trip involves multiple activities:

- Finding suitable flights.
- Searching for hotels based on budget and preferences.
- Calculating the overall trip expenses.
- Organizing travel activities into an itinerary.

Performing these tasks separately can be time-consuming.

This project aims to simplify the travel planning process using an Agentic AI approach.

##  Technologies Used
---------------------------------------------------------------------------------------
- Python
- LangChain
- Agentic AI
- PySpark
- Pandas
- LLM and Tool Calling
- CSV-based datasets

##  Agent Tools
-----------------------------------------------------------------------------------------
The agent uses four primary tools:

### 1. search_flights()

Searches for available flights based on user requirements.

**Inputs:**
- Origin
- Destination
- Departure date
- Return date (optional)
- Number of adults
- Number of children and infants (optional)
- Cabin class (optional)
- Maximum stops (optional)
- Preferred airline (optional)

**Output:**
Relevant flight options with flight details and ticket prices.

### 2. search_hotels()

Finds suitable hotels based on the user's preferences.

**Inputs:**
- Destination
- Check-in date
- Check-out date
- Number of guests
- Number of rooms (optional)
- Budget (optional)
- Star rating (optional)
- Amenities (optional)
- Preferred area (optional)

**Output:**
Matching hotel options with pricing and hotel details.

### 3. calculate_trip_budget()

Calculates the estimated total travel expenses.

**Cost components:**
- Flight expenses
- Hotel accommodation
- Food expenses
- Transportation
- Activities

**Budget calculation:**

Total Budget = Flight Cost + Hotel Cost + Food Cost + Transportation Cost + Activities Cost

### 4. create_itinerary()

Creates a structured travel itinerary based on the trip details.

**Inputs:**
- Destination
- Start date
- End date
- Travel preferences
- Selected flight and hotel details

**Output:**
A day-wise travel plan with activities and estimated expenses.

##  Agent Workflow
------------------------------------------------------------------------------------
1. User provides travel requirements in natural language.
2. AI agent understands the user's intent.
3. Agent identifies the required tools.
4. Flight search tool retrieves relevant flight options.
5. Hotel search tool retrieves suitable accommodation.
6. Budget calculator estimates total expenses.
7. Itinerary tool generates the final travel plan.
8. Agent presents the results in a user-friendly format.

##  Architecture
-----------------------------------------------------------------------------------
User Query → AI Agent → Tool Selection → Tool Execution → Results Processing → Final Travel Plan

##  Functional Requirements
-------------------------------------------------------------------------------------
- Understand natural-language travel requests.
- Search flights using travel dates and passenger details.
- Search hotels using location, dates, and preferences.
- Calculate estimated trip expenses.
- Generate day-wise travel itineraries.
- Handle optional parameters.
- Validate required inputs.
- Handle missing or invalid information gracefully.
- Avoid inventing flight and hotel availability or prices.

##  Sample User Queries
-------------------------------------------------------------------------------------
1. Find flights from Delhi to Jaipur on 15 December 2026 for two adults.
2. Find hotels in Jaipur for two guests from 15 December to 18 December.
3. Plan a 3-day trip to Jaipur with a budget of ₹30,000.
4. Calculate the total trip budget, including flights, hotels, food, and transportation.
5. Create a complete itinerary for my Jaipur trip.
6. Find budget-friendly flights and 4-star hotels for my family vacation.

##  Future Enhancements
----------------------------------------------------------------------------------------
- Integration with real-time flight booking APIs.
- Integration with hotel reservation APIs.
- Weather forecasting integration.
- Map-based sightseeing recommendations.
- User preference and conversation memory.
- Booking confirmation and payment integration.
- RAG-based travel knowledge assistant.

##  Key Learning Outcomes
--------------------------------------------------------------------------------------------
- Building an Agentic AI application.
- Implementing custom tools using LangChain.
- Understanding tool selection and execution.
- Handling optional tool parameters.
- Integrating multiple tools into a single workflow.
- Designing a multi-step travel planning solution.

## Project Goal
-----------------------------------------------------------------------------------------------
To build an intelligent travel assistant that simplifies trip planning by combining multiple tools and AI-driven decision-making in a single application.
