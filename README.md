# OST Monitoring Web Dashboard — QA Testing

This repository contains the automated testing suite (Katalon Studio) for the **OST (Oil Storage Tank) Monitoring System — PT. Citra Putra Kebun Asri (CPKA)**, a web dashboard used to monitor CPO (Crude Palm Oil) tank volume, mass, and temperature in near real-time.

This testing suite is built to verify the functionality of the web dashboard before and after deployment, covering UI testing, sensor-to-dashboard data flow, and validation of the system's core features.

> **Note:** This QA testing suite is still under active development. Current test cases cover the core dashboard features, and will be expanded over time to cover additional and more advanced features as the system evolves.

## Tech Stack

- **Test Automation Tool:** [Katalon Studio](https://katalon.com/)
- **Application Under Test:** OST Monitoring Web Dashboard (React + FastAPI + PostgreSQL)
- **Scripting Language:** Groovy

## Project Structure

```
├── Include/config             # Supporting configuration files for test execution
├── Object Repository/         # UI objects (page elements) used by the test cases
│   └── Page_OST Monitoring System - PT. CPKA
├── Profiles/                  # Execution profiles (e.g. environment variables, base URL)
├── Scripts/                   # Groovy scripts behind each test case
├── Test Cases/                # List of created test cases
├── settings/                  # Katalon project settings
├── OST MONITORING QA.prj      # Main Katalon Studio project file
├── build.gradle                # Build/dependency configuration
└── console.properties          # Katalon console runner configuration
```

## Test Coverage

The suite currently covers testing of the OST Monitoring dashboard, including:

- User login & authentication
- Dashboard page navigation and rendering
- Sensor data display (volume, mass, temperature) per tank
- Chart/history data visualization
- System status validation (MQTT connection & device reachability)
- Negative scenarios (invalid data / unreachable device)

### Planned / Upcoming Coverage

As the system continues to develop, this suite will be expanded to include:

- Additional edge cases and negative scenarios
- Cross-browser and responsiveness testing
- Role-based access control (RBAC) testing
- Regression testing for new dashboard features

## How to Run

1. Install [Katalon Studio](https://katalon.com/download) (latest version recommended).
2. Clone this repository:
   ```bash
   git clone https://github.com/raphs2506/OST-Monitoring-Web-Dashboord-QA-Testing.git
   ```
3. Open Katalon Studio, select **Open Existing Project**, and point it to the cloned folder (the `OST MONITORING QA.prj` file).
4. Select the desired Test Case in the **Test Cases** panel, then click **Run**.
5. Adjust the **Profile** (e.g. base URL environment) in the `Profiles/` folder before execution if needed.

## Related Project

This project is part of the development of the **OST Monitoring System**, being developed as a prototype-scale pilot for PT. Citra Putra Kebun Asri (CPKA), building on an IoT-based CPO tank monitoring system.

## Author

Rafif Farhan Putra Ardhana — Computer Engineering, Telkom University
