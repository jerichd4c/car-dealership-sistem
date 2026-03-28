<a id="readme-top"></a>

<div align="center">
  <h3 align="center">Car Dealership System</h3>

  <p align="center">
    A C++ console application for managing a car dealership with client and vehicle management
  </p>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#project-structure">Project Structure</a></li>
    <li><a href="#license">License</a></li>
  </ol>
</details>

## About The Project

This is a car dealership management system built in C++ following the MVC (Model-View-Controller) architectural pattern. The application allows users to manage clients and vehicles, track purchases and sales, and calculate profits.

**Key Features:**
- Client management with personal information
- Vehicle inventory tracking
- Purchase and sale transaction recording
- Profit calculation from vehicle transactions
- Data persistence via CSV files

### Built With

* [![C++][Cpp-shield]][Cpp-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Getting Started

To get a local copy up and running, compile the source code natively via GCC/G++.

### Prerequisites

* GCC / G++ (MinGW on Windows)
* C++11 or higher

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/username/car-dealership-system.git
   ```
2. Navigate to the project directory
   ```sh
   cd car-dealership-system
   ```
3. Compile the project:
   ```sh
   g++ src/main.cpp src/modelo/modelo.cpp src/vista/vista.cpp src/controlador/controlador.cpp -o bin/proyectoConcesionaria.exe
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Usage

Execute the binary to run the interactive console application:

```sh
./bin/proyectoConcesionaria.exe
```

The application provides the following menu options:

1. **Display Client Cars Info** - View all vehicles associated with a specific client
2. **Add Bought Car** - Record a new vehicle purchase
3. **Update Sold Car** - Mark a vehicle as sold and update client association
4. **Get Profit** - Calculate total profit from all vehicle transactions
5. **Delete Item** - Remove a client or vehicle from the system
0. **Exit** - Close the application

**Data Files:**
The system reads and writes data to CSV files located in the `assets/` directory:
- `clients.csv` - Client information
- `cars_data.csv` - Vehicle inventory and transaction data

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Project Structure

```
car-dealership-system/
├── src/
│   ├── main.cpp              # Application entry point
│   ├── modelo/                # Model layer
│   │   ├── modelo.h
│   │   └── modelo.cpp        # Client and Cars classes, file I/O
│   ├── vista/                 # View layer
│   │   ├── vista.h
│   │   └── vista.cpp         # Menu and display functions
│   └── controlador/           # Controller layer
│       ├── controlador.h
│       └── controlador.cpp    # Business logic operations
├── assets/
│   ├── clients.csv           # Client data
│   └── cars_data.csv         # Vehicle data
├── bin/                      # Compiled executables
└── README.md
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## License

Distributed under the MIT License.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
[Cpp-shield]: https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white
[Cpp-url]: https://isocpp.org/s