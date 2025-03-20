# Disaster Resource Allocator

## Overview
Disaster Resource Allocator is a **Java-based project** designed to calculate **risk scores** for districts based on **population, land type, and urbanization** to optimize resource allocation during disasters. This system ensures efficient distribution by prioritizing high-risk areas with limited resources.

## Features

- **Risk Assessment**: Computes risk scores for districts based on key factors.
- **Resource Allocation**: Distributes resources effectively to high-risk areas.
- **Dynamic Sorting**: Uses a risk-to-demand ratio for optimal prioritization.
- **Partial Allocation Support**: Handles cases where demand exceeds available resources.

## How It Works

1. **Input district details**: Name, population, land type, urbanization, and resource demand.
2. **Risk Calculation**: Computes scores using weighted factors.
3. **Sorting**: Ranks districts based on their risk-to-demand ratio.
4. **Resource Allocation**: Prioritizes high-risk districts.
5. **Final Report**: Displays allocation results and remaining resources.

## Project Structure

- **RiskStatistics.java**: Contains methods to calculate risk scores.
- **District.java**: Defines the District class and its attributes.
- **DisasterResponse.java**: Main driver class for input handling and allocation.

## Input Details

- **Number of Districts**: Specify the total districts.
- **Total Resources**: Enter the total available resources.
- **District Data**:
  - Name
  - Population
  - Land Type: Forest, Coastal, Desert, Urban
  - Urbanization: Rural, Suburban, Urban
  - Resource Demand

## Output

- Displays computed risk scores.
- Allocates resources based on priority.
- Reports remaining resources or incomplete allocations.

## Example Usage

### Running the Program
```sh
javac DisasterResponse.java
java DisasterResponse
```

### Sample Input & Output
```
Enter the number of districts: 3
Enter the total available resources: 100

Enter details for District 1:
Name: Alpha
Population: 20000
Land Type: Urban
Urbanization: Urban
Resource Demand: 50

Enter details for District 2:
Name: Beta
Population: 5000
Land Type: Forest
Urbanization: Rural
Resource Demand: 30

Enter details for District 3:
Name: Gamma
Population: 60000
Land Type: Coastal
Urbanization: Suburban
Resource Demand: 40

Risk Scores:
Alpha: 24
Beta: 8
Gamma: 19

Resource Allocation:
Allocating 50 resources to Alpha
Allocating 30 resources to Gamma
Allocating 20 resources to Beta (partial allocation)

All resources have been allocated.
```

## Technologies Used

- **Java**: Core programming language
- **Scanner**: For user input
- **Arrays**: For storing and sorting district data

## Contributing

Contributions are welcome! Feel free to submit issues or pull requests.

## License

This project is licensed under the **MIT License**.

---

### Contact
For any questions or suggestions, reach out via GitHub issues.

🚀 Happy Coding!

