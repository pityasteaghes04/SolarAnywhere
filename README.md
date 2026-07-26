# SolarAnywhere: Global Solar Calculation Tool

## Abstract
SolarAnywhere is a high-precision, global solar calculation tool designed to bridge the gap between renewable energy and accessibility. Powered by the **Google Maps API** and **Visual Crossing API**, the system features a seamless location engine that resolves any point on Earth—from entire cities down to specific landmarks.

To demonstrate its power, the tool can pivot from a broad search like *Seattle, WA* to a high-precision target like the *Space Needle*, fetching hyper-local irradiance data instantly. SolarAnywhere provides reliable, data-driven insights to help users design solar setups tailored to their daily energy needs, regardless of environment.

---

## Project Overview
The 2026 update transforms the project from a theoretical model into a functional smart tool. By analyzing how solar panel energy output varies by location and device battery capacity, we translate complex solar radiation metrics into practical, consumer-facing insights.

### Core Features
* **Smart Search:** Resolves locations and landmarks by name for instant, hyper-local data.
* **Global Precision:** Integrates 365 days of live weather data to calculate exact solar potential anywhere on Earth.
* **Predictive Planning:** Models battery success rates across varied climate profiles.
* **Stress Testing:** Rigorously verified for all-weather reliability across extreme irradiance variances.
* **System Resilience:** Built with fallback logic to ensure reliable hardware efficiency insights.

> **Project Presentation:** [View SolarAnywhere Presentation (PDF)](https://github.com/pityasteaghes04/SolarAnywhere/blob/main/SolarAnywhere_Presentation.pdf)

---

## Technical & Hardware Specifications

### API & Data Stack
* **Location Engine:** Google Maps Geocoding API
* **Weather & Solar Data:** Visual Crossing Weather API
* **Battery Profiles:** Measured in Watt-hours (Wh) for modern mobile devices

### Hardware Specification Mapping
*Calculated at 3.85V nominal voltage.*

| Device Model | Capacity (mAh) | Energy (Wh) | Profile Type |
| :--- | :---: | :---: | :--- |
| **OnePlus 13** | 6,000 | 23.10 | High-Density |
| **Google Pixel 10 Pro XL** | 5,200 | 20.02 | Large Flagship |
| **Samsung Galaxy S25 Ultra** | 5,000 | 19.25 | Ultra-Premium |
| **iPhone 16 Pro Max** | 4,685 | 18.04 | Baseline |
| **iPhone 16 Pro** | 3,582 | 13.79 | Standard Pro |
| **iPhone 16** | 3,561 | 13.71 | Standard |

> **User Tip:** Don't see your device? Look up your specs on [GSMArena](https://www.gsmarena.com/) and calculate capacity using:  
> **Watt-hours (Wh) = (Capacity in mAh × 3.85) ÷ 1000**

## Project Visualizations

### Overall Panel Distribution & Outliers Across Device Models
*Highlights the distribution of solar panels required to charge each device fully, including extreme weather anomalies and high-irradiance outliers.*

![Panel Distribution](https://raw.githubusercontent.com/pityasteaghes04/SolarAnywhere/main/images/bar-1-requirement-model.png)

<br />

### Standard Hardware Requirements Range by Phone Model
*Presents the core 0.0 to 3.5 panel requirement range under normal conditions, making it easy to compare average daily hardware needs across flagship devices.*

![Requirement Boxplot](https://raw.githubusercontent.com/pityasteaghes04/SolarAnywhere/main/images/bar-2-requirement-model.png)

<br />

### Daily Solar Irradiance Profile (Space Needle)
*Tracks real-time solar radiation variance ($\text{W/m}^2$) over a full year, demonstrating seasonal energy availability shifts from winter lows to summer peaks.*

![Daily Solar Radiation](https://raw.githubusercontent.com/pityasteaghes04/SolarAnywhere/main/images/live-api-data.png)

<br />

### Solar Reliability Analysis: ICDF Curve (Space Needle)
*Illustrates the cumulative probability of achieving a full daily charge relative to the number of solar panels deployed across different smartphone battery profiles.*

![Solar Reliability ICDF](https://raw.githubusercontent.com/pityasteaghes04/SolarAnywhere/main/images/icdf-curve.png)

</div>

---

## Technical Skills Demonstrated
* **Python Engineering:** Pandas, NumPy, Matplotlib, Geopy, Seaborn, REST API integration.
* **Statistical Modeling:**
    * **ICDF Curves:** Probability modeling for energy sufficiency.
    * **Outlier Analysis:** Identifying seasonal variances using Box-and-Whisker plots.
* **Systems Design:** Fallback logic for API credentials and data stream continuity.
* **Project Management:** Git/GitHub version control.

---

<div align="center">

## How to Run

</div>

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/pityasteaghes04/SolarAnywhere.git](https://github.com/pityasteaghes04/SolarAnywhere.git)
    ```
    
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ``` 
                                    
3.  **Execution:** Open `solar-anywhere-pityast.ipynb` in VS Code or any Jupyter environment.
4.  **API Access:** Press **Enter** at the prompt to use the built-in demo fallback key.
