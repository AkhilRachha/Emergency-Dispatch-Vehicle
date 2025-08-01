# 🚑 Emergency Vehicle Dispatch System

A mini project developed as part of the **Design and Analysis of Algorithms (DAA)** course. The project aims to efficiently dispatch emergency vehicles using **Dijkstra’s Algorithm** to determine the shortest and least congested path between a user’s location and the nearest or selected hospital.

## 📌 Objective

To find and allocate an available emergency vehicle by:
- Taking the source and destination inputs from the user.
- Providing the **optimal route** based on **traffic density and distance**.
- Offering a **rerouting** feature in case the destination hospital is unavailable.

## 🧠 Algorithm Used

- **Dijkstra’s Algorithm** is implemented to compute the shortest path considering both:
  - Distance between nodes.
  - Dynamic traffic density levels (converted to weights). 

## 🏙️ Project Overview

- City considered: **Prime City** with:
  - 22 locations (e.g., Georgopol, Novo, Rozhok, etc.)
  - 6 hospitals
- Each location is a **node** in a graph.
- Edges represent **roads** weighted by:
  - Distance
  - Traffic density (classified into 4 stages: Low, Medium, High, Very High)

## 🔁 Rerouting Support

- If the chosen hospital is unavailable due to:
  - No beds
  - Closed admissions
  - Lack of medical equipment
  - Patient’s condition worsening

  Then the system reroutes to the next optimal hospital with updated fare calculations.

## 🧾 Features

- User Registration/Login System
- Location selection from a predefined map
- Automatic fare calculation based on route
- Details of booking saved to file
- Re-routing logic based on real-world constraints
- Output displays:
  - Selected hospital
  - Distance and fare
  - Date & time of dispatch

## 💻 Code Structure

- `FINAL-CODE.c`: Main source code implementing the full logic.

## 🔍 Sample Inputs

```plaintext
Choose location: 1. Georgopol
Choose destination: 0 (for nearest hospital)
...
Fare estimated: ₹375
Would you like to confirm? -> Yes
Ambulance booked successfully!
