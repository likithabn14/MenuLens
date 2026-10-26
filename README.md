#MenuLens

### See the real dish before you order.

MenuLens is a community-powered food discovery and review platform designed to help people make better food choices by exploring reviews of individual dishes rather than relying only on restaurant ratings.

Whether someone wants to find a pizza, burger, biryani, dosa, pasta, dessert, coffee, or any other menu item, MenuLens aims to make it easier to compare dishes, explore customer experiences, and discover hidden food gems.

## Project Overview

Traditional restaurant review platforms primarily focus on overall restaurant ratings. However, the quality of individual dishes can vary significantly within the same restaurant.

MenuLens focuses on the dish itself.

Users can explore food items, compare dishes across restaurants, review their dining experiences, upload food photographs, and evaluate different aspects of a dish.

The application is being developed using Python and Streamlit, with SQLite for data storage and Plotly for interactive visualizations.

##  Planned Features

The following features represent the project scope. Features should be marked as implemented only after they have been completed and tested.

* **Dynamic Food Search:** Search for dishes, restaurants, and food categories.
* **Dish Reviews:** Rate individual food items instead of only rating restaurants.
* **Dish Comparison:** Compare the same or similar dishes across restaurants.
* **Community Food Photos:** Upload photographs showing the actual food received.
* **Expectation vs. Reality:** Compare menu photographs with customer-uploaded photographs.
* **Food Categories:** Explore categories such as pizza, burgers, biryani, desserts, beverages, pasta, and more.
* **Dish Analytics:** Visualize ratings, spice levels, freshness, value, and portion sizes.
* **Hidden Gems:** Discover highly rated dishes with relatively few reviews.
* **Dish Personality:** Generate descriptive tags from available review data.
* **Best Ordering Time:** Analyze community freshness ratings by ordering time.
* **Restaurant Profiles:** Explore restaurant details and their popular dishes.
* **Favorites:** Save dishes for future reference.
* **User Profiles:** View review activity, uploaded photographs, and achievements.
* **Responsive Dark Theme:** Use a modern interface with black backgrounds and orange accents.

##  Technology Stack

| Component                          | Technology      |
| ---------------------------------- | --------------- |
| Frontend and application framework | Streamlit       |
| Programming language               | Python          |
| Database                           | SQLite          |
| Data processing                    | Pandas          |
| Numerical operations               | NumPy           |
| Interactive charts                 | Plotly          |
| Image processing                   | Pillow          |
| Sample data generation             | Faker           |
| Date utilities                     | Python Dateutil |

##  Project Structure

```text
MenuLens/
├── app.py
├── database.py
├── models.py
├── helpers.py
├── image_upload.py
├── charts.py
├── requirements.txt
├── README.md
├── .gitignore
├── assets/
├── pages/
└── uploads/
```

* `app.py` — Main Streamlit application and home page.
* `database.py` — SQLite initialization, schema, database queries, and data operations.
* `models.py` — Data definitions and sample-data generation logic.
* `helpers.py` — Shared utility functions and reusable application logic.
* `image_upload.py` — Image validation, processing, and storage.
* `charts.py` — Plotly visualizations and review analytics.
* `pages/` — Additional Streamlit pages.
* `assets/` — Application assets.
* `uploads/` — Locally stored user-uploaded images.
* `requirements.txt` — Python dependencies.

##  Installation

### Prerequisites

Install Python 3.10 or a compatible version supported by the selected dependencies.

Install Git if you intend to upload the project to GitHub.

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd MenuLens
```

### 2. Create a virtual environment

Windows:

```bash
python -m venv .venv
.venv\Scripts\activate
```

macOS or Linux:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Run the application

After the application files have been implemented:

```bash
streamlit run app.py
```

Streamlit will provide a local address where the application can be opened in your browser.

##  Deployment on Streamlit Community Cloud

1. Upload the completed project to a GitHub repository.
2. Sign in to Streamlit Community Cloud.
3. Create a new application.
4. Select the MenuLens GitHub repository.
5. Select the branch containing the application.
6. Set the main file path to `app.py`.
7. Deploy the application.
8. Test the deployed application and its database and image-storage behavior.

**Deployment note:** A local SQLite database and local image directory should not be assumed to provide permanent storage on a hosted platform. Configure an appropriate persistent database and image-storage solution if user-generated content must survive application restarts and deployments.

##  Data and Privacy

MenuLens may store user-submitted reviews, ratings, and photographs.

A production deployment should validate uploaded files, restrict upload sizes, handle user content responsibly, protect any authentication credentials, and implement appropriate privacy and moderation controls.

##  Future Scope

Potential improvements include:

* User authentication and authorization
* Persistent cloud database integration
* Cloud image storage
* Duplicate-review detection
* Advanced dish recommendation systems
* Geolocation-based food discovery
* Restaurant menu integrations
* Review moderation
* Improved food image comparison
* Personalized recommendations based on preferences


##  Author
LIKITHA BN
