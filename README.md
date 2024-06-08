# Data Visualization Dashboard

This project is a data visualization dashboard that provides insights into various global trends and factors using data from a provided JSON file. The dashboard is built using the MERN (MongoDB, Express.js, React, Node.js) stack and features interactive charts and graphs created with D3.js.

## Features

- Interactive data visualizations using react-chartjs-2 , @chakra-ui
- MongoDB database integration
- RESTful API built with Node.js and Express.js
- React-based frontend for a responsive and dynamic user interface
- Multiple filters for data analysis:
  - End Year
  - Topics
  - Sector
  - Region
  - PEST (Political, Economic, Social, Technological)
  - Source
  - SWOT (Strengths, Weaknesses, Opportunities, Threats)
  - Country
  - City

### Dashboard Overview
![image](https://github.com/pravesh2892/Blackcoffer_assignment/assets/112716122/f883809d-e46c-4780-8c50-ea480e2b4e65)
![image](https://github.com/pravesh2892/Blackcoffer_assignment/assets/112716122/a1b112af-99af-4b32-8f19-2da62feedeed)


*This is the main view of the dashboard, showcasing various charts and filters.*

### Intensity Chart
![image](https://github.com/pravesh2892/Blackcoffer_assignment/assets/112716122/e5e5b8bf-8929-4864-aac7-e1c44c46763f)



### Region Distribution
![image](https://github.com/pravesh2892/Blackcoffer_assignment/assets/112716122/940fa293-9888-45f8-b812-cd69036e348c)


### Topics Chart
![image](https://github.com/pravesh2892/Blackcoffer_assignment/assets/112716122/89996beb-efd5-4ebd-922d-bf40543af783)


### Relevance Chart
![image](https://github.com/pravesh2892/Blackcoffer_assignment/assets/112716122/388c9f8f-b8c5-40c9-a2ff-5a0d8a5023f2)

### Sector Chart
![image](https://github.com/pravesh2892/Blackcoffer_assignment/assets/112716122/83d1a87c-0bd8-4c05-b76b-1615ef6150d2)

### Likelihood Chart
![image](https://github.com/pravesh2892/Blackcoffer_assignment/assets/112716122/9f2aa8d9-566b-4e3d-8aac-fb4df8a52cef)

### Country Chart
![image](https://github.com/pravesh2892/Blackcoffer_assignment/assets/112716122/81315a48-0126-4447-8a6f-037169a87c6b)




## Data Insights

The dashboard provides insights into the following key variables:

- Intensity
- Likelihood
- Relevance
- Year
- Country
- Topics
- Region
- City

## Prerequisites

Before you begin, ensure you have the following installed:

- Node.js (v14.x or later)
- npm (v6.x or later)
- MongoDB (v4.x or later)

## Installation

1. Clone the repository:
2. Install dependencies for both frontend and backend:

3. Set up the MongoDB database:
- Make sure MongoDB is running on your local machine.
- In the `backend` directory, create a `.env` file with your MongoDB connection string:
  ```
  MONGODB_URI=mongodb://localhost:27017/datavizdashboard
  ```

4. Import data into MongoDB:
- Place the `jsondata.json` file in the `backend/data` directory.
- Run the data import script:
  ```
  cd backend
  node scripts/importData.js
  ```

## Running the Application

1. Start the backend server:

The server will run on `http://localhost:5000`.

2. Start the frontend development server:

The React app will run on `http://localhost:3000`.

3. Open your browser and visit `http://localhost:3000` to view the dashboard.

## API Endpoints

- `GET /api/data`: Fetches all data from the MongoDB database.
- `GET /api/data/filters`: Fetches available filter options (topics, sectors, regions, etc.).

For more detailed API documentation, refer to the `backend/README.md` file.

## Tech Stack

- **Frontend**: React, D3.js
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Additional Libraries**: Axios (for API calls), React Router (for routing)

## Contributing

Feel free to fork this repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is open-source and available under the [MIT License](LICENSE).

## Acknowledgments

- Data provided as part of the assignment
- Inspiration from various data visualization dashboards and tutorials
