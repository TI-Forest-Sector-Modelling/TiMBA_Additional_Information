# README: Data Extraction and Calculation for Ad Valorem Tariffs Rates and Forest Growing Stock and Forest Stock Growth for TiMBA v1.0.1

# Content

# 

# Calculation of Ad Valorem Tariffs Rates

## Overview

The Timber market Model for policy-Based Analysis - TIMBA - is a partial
economic equilibrium model for the global forest products market. It
simulates production, consumption, and trade of wood-based products
across 180 countries.

Trade in TiMBA depends, among others, on the transportation costs.
Transportation costs entails commodity-specific freight costs and
tariffs. Tariffs are calculated as a percentage of the value of the
imported product using ad valorem rates. They are derived from WTO
Integrated Database (IDB) \[WTO 2024:
http://tariffdata.wto.org/Default.aspx?culture=en-US\] notifications
using 6-digit (subheadings) or 4-digit codes (headings) HS Codes.

This Readme provides a detailed explanation of how the ad valorem rates
were extracted and calculated for different wood-based products across
different countries. The rates are based on the **Most-Favored-Nation
(MFN)** applied tariff, and trade agreements were not considered in the
calculations.

This research updates previous data as published with the Forest Sector
Model GFPM \[Buongiorno 2003; GFPM-base 2021\]. The base for the tariff
update is the least available HS code version for each country, with
updates based on data from **July 2024** sourced from the **World Trade
Organization (WTO) Integrated Database (IDB)** Tariff Download Facility
(Link: http://tariffdata.wto.org/Default.aspx?culture=en-US).

## 2. Notes on Tariff Data Calculation and Updates

### HS Code Selection

The extraction and / or calculation of ad valorem rates is based on the
**HS (Harmonized System) codes** for each product. The HS codes provide
standardized classifications of goods, used internationally for tariff
purposes. The HS classifies products using 6-digit codes that are
organized by chapters (2 digits), headings (4 digits), and subheading (6
digits). If applicable, we extract information stated on the **4-digit
level**. However, in some cases, a product in the TiMBA model framework
is represented by **6-digit HS codes**.

### Base for Updates 

The calculation uses the **least available HS version** for a particular
country. The rates were carefully checked for accuracy, and changes to
earlier entries were marked using **flags** for transparency.

The different **flags** associated to the ad valorem rates in Table 2
carry additional information: **O** indicates that the update are based
on a very old HS version, **U** indicates that the updated value differs
from a earlier entries, **C s**hows that the value has been checked in
the with WTO IDB data from July 2024 and remains unchanged compared to
the data provided by GFPM (2021), and **X** means that no information
are available for the corresponding product and country. For these
countries, we assume an ad valorem rate of zero.

Differences between provided data provided in Table 2 and the
information delivered with the GFPM-base (2021) should come from the
updates of the values. However, especially when combined HS code
combinations are used for product representation, the difference may
also arise from the different use of product classifications and
assignments in the current work and the GFPM (Buongiorno 2003)
(Buongiorno 2015)

### Ad Valorem Rate Acquisition

In general, mean ad valorem rates for those specific products are
extracted from the WTO IDB. Products represented by more than one
HS-code are treated separately for calculating mean ad valorem rates for
those specific products. Thus, depending on the number of HS codes digit
levels involved, ad valorem rates were either extracted or calculated:

Where possible, the ad valorem rate for a specific country and product
are extracted directly from the **WTO** **IDB** as (mean) ad valorem
rates on the 4-digit or 6-digit code level. Prerequisite for the former
case is, that the product representation in TiMBA is congruent with the
4-digit level in the HS system.

Some products are represented by more than one 4-digit and / or 6-digit
HS code. When this occurs, the tariffs for these codes are treated
separately for the calculation, and the final ad valorem rate reflects
the aggregate or a representative value based on the available data. In
case that a product in TiMBA is composed of **multiple HS codes (see
Table x), the ad valorem rate is calculated** based on the available
tariff data for the product and country as the average of ad valorem
duties of the respective reporter country and product.

### List of Products

Table 1: Products and assignment of HS codes used for the ad valorem
rate calculations.

  -----------------------------------------------------------------------
  Product                                                        HS codes
  ---------------------- ------------------------------------------------
  Fuelwood                                                           4401

  Industrial Roundwood                                               4403

  Sawnwood                440721, 440722, 440723, 440724, 440725, 440726,
  Non-coniferous          440727, 440728, 440729, 440791, 440792, 440793,
                                   440794, 440795, 440796, 440797, 440799

  Sawnwood Coniferous      440710, 440711, 440712, 440713, 440714, 440719

  Veneer and Plywood                                                 4412

  Particleboard                                                      4410

  Fibreboard                                                         4411

  Mechanical Pulp                                                    4701

  Chemical and                                           4703, 4704, 4705
  Semi-chemical pulp     

  Other Fibre Pulp                                                   4706

  Waste Paper                                                        4707

  Newsprint                                                        480100

  PWP                                                                4802

  Paper and Paperboard    4804, 4805, 480620, 480630, 480640, 4807, 4808,
                                     4810, 4811, 481500, 4819, 4821, 4823
  -----------------------------------------------------------------------

# Data Extraction and Calculation for Forest Growing Stock and Forest Stock Growth

## Overview

This dataset contains information on forest growing stock and forest
stock growth for 180 countries, as considered in the TiMBA model. While
data on forest area and forest growth for the reporting year 2020 is
adequately provided by the **FRA 2020** (Forest Resources Assessment),
the data on growing stock and stock growth is fragmented and not fully
reported for all countries. This README explains the methodology used to
extract data as well as fill in the data gaps and provide consistent
values for forest growing stock and stock growth across all countries.
