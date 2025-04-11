# Travel Itinerary Planner 🗺️

This project is a **Travel Itinerary Planner** powered by AI agents. It helps users plan their trips by gathering information about destinations, finding the best local food spots, and creating detailed travel itineraries.

## Features

- **Destination Exploration**: Discover things to do, festivals, and attractions in your chosen destination.
- **Foodie Recommendations**: Find the best local food spots and must-try dishes.
- **Itinerary Planning**: Generate a detailed day-by-day travel plan based on your preferences.
- **Streamlit Interface**: User-friendly interface for inputting travel details and viewing results.
- **Downloadable Plans**: Download your travel plan as a text file.

## Project Structure.
    ├── .gitignore # Files and directories to ignore in version control
    ├── LICENSE # MIT License for the project 
    ├── agents.py # Defines AI agents for travel planning
    ├── app.py # Streamlit app for user interaction 
    ├── main.py # Core logic for orchestrating agents and tasks 
    ├── tasks.py # Defines tasks for the agents 
    ├── tools.py # Tools used by the agents (e.g., web search) 
    ├── utils.py # Utility functions (e.g., Streamlit callbacks)


### File Descriptions

- **[`agents.py`](agents.py)**: Contains the `TravelAgents` class, which defines three agents:
  - `location_expert`: Helps explore destinations.
  - `local_foodie`: Finds the best local food spots.
  - `travel_concierge`: Creates detailed travel itineraries.

- **[`tasks.py`](tasks.py)**: Contains the `TravelTasks` class, which defines tasks for the agents:
  - `gather_information_task`: Gathers information about the destination.
  - `foodie_task`: Finds local food recommendations.
  - `plan_task`: Creates a multi-day travel plan.

- **[`tools.py`](tools.py)**: Defines tools used by the agents, such as the `browser` tool for web searches.

- **[`utils.py`](utils.py)**: Contains utility functions, including `streamlit_callback` for displaying agent outputs in the Streamlit app.

- **[`main.py`](main.py)**: Implements the `TravelCrew` class, which orchestrates agents and tasks to generate travel plans.

- **[`app.py`](app.py)**: The main entry point for the Streamlit app. Provides a user interface for inputting travel details and viewing results.

- **[`LICENSE`](LICENSE)**: MIT License for the project.

- **[`.gitignore`](.gitignore)**: Specifies files and directories to be ignored by Git.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Travel-Itinerary-Planner.git
   cd Travel-Itinerary-Planner
2. Install dependencies
    ```bash
    pip install -r requirements.txt
3. Set up environment variables:
    Create a .env file in the root directory.
    Add your API keys and other configuration details.

## Usage
1. Run Ollama:
    ```bash
    ollama serve
1. Run the Streamlit app in separate terminal:
    ```bash
    streamlit run app.py

2. Open the app in your browser and follow these steps:

    Enter your destination city.
    Specify your travel dates and interests.
    Click "Plan My Trip" to generate your travel itinerary.
3. Download your travel plan using the "Download Plan" button.

## Dependencies.
    Python 3.8+
    Streamlit
    LangChain
    CrewAI
    dotenv
    License

This project is licensed under the MIT License.

Author
Created by PrathamDesai07. Contributions are welcome!

## Acknowledgments.
    LangChain Community
    Streamlit
    Google Serper API