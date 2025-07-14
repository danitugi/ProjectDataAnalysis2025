# 🏡 Real Estate Price Predictor – Rehovot 🧠  
*Final Project – Data Analyst Course 2025 | Part 1*

[![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Processing-lightgrey?logo=pandas)]
[![BeautifulSoup](https://img.shields.io/badge/Web%20Scraping-BeautifulSoup4-green?logo=html5)]
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 🧾 About the Project

This project is part of the final assignment for the **Data Analyst course (2025)** – Part 1.

We built a **web scraper** that collects rental listings data from [ad.co.il](https://www.ad.co.il/nadlanrent) focusing on apartments in neighborhoods of **Rehovot**.

The dataset was cleaned, processed, and saved in a structured `.csv` format, ready for use in machine learning models for rental price prediction (coming in Part 2).

---

## 📊 Features

- Automated web scraping with **BeautifulSoup/Selenium**
- Full dataset exported to `apartments_data.csv`
- Standardized features as required (strict schema enforcement)
- Distance from **Rehovot Center** calculated using Geolocation API
- Ready for modeling (Part 2)

---

## 🗂️ Data Structure

The dataset includes the following columns:

| Column Name            | Type   | Description                             |
|------------------------|--------|-----------------------------------------|
| `property_type`        | str    | Apartment type                          |
| `neighborhood`         | str    | Neighborhood (from predefined list)     |
| `address`              | str    | Full address                            |
| `room_num`             | float  | Number of rooms                         |
| `floor`                | int    | Apartment floor                         |
| `area`                 | int    | Built area (sqm)                        |
| `garden_area`          | int    | Garden area (sqm)                       |
| `days_to_enter`        | int    | Days until entry                        |
| `num_of_payments`      | int    | Payments per year                       |
| `monthly_arnona`       | int    | Monthly municipal tax                   |
| `building_tax`         | int    | Monthly building fee                    |
| `total_floors`         | int    | Total floors in building                |
| `description`          | str    | Text description from the listing       |
| `has_parking`          | 0/1    | Has parking                             |
| `has_stotsge`          | 0/1    | Has storage                             |
| `elevator`             | 0/1    | Elevator in building                    |
| `ac`                   | 0/1    | Has air conditioning                    |
| `handicap`             | 0/1    | Handicap accessible                     |
| `has_bars`             | 0/1    | Has bars on windows                     |
| `has_safe_room`        | 0/1    | Has protected room                      |
| `has_balcon`           | 0/1    | Has balcony                             |
| `is_furnished`         | 0/1    | Furnished                               |
| `is_renovated`         | 0/1    | Renovated                               |
| `price`                | float  | Monthly rent (NIS)                      |
| `num_of_images`        | int    | Number of listing images                |
| `distance_from_center` | float  | Meters from Rehovot Center              |

---
