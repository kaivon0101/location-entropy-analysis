# Location Entropy Analysis on EPFL Mobility Dataset

# Overview
This project analyzes a spatio-temporal mobility dataset to compute location entropy per user, a metric that quantifies how predictable or diverse a user's movement behavior is. Using real-world GPS trajectory data from the EPFL Cabspotting dataset, we extract behavioral insights and propose potential data-driven product ideas.

## Dataset
The analysis uses the dataset which contains mobility traces of taxi cabs in San Francisco, USA. It contains GPS coordinates of approximately 500 taxis collected over 30 days in the San Francisco Bay Area.

You can download or refer it from link below:
Source: https://ieee-dataport.org/open-access/crawdad-epflmobility

After downloading, extract the zip and place at the same folder with the location_entropy.ipynb.
The path will be: 
Location Entropy/
└── cabspottingdata/
    └── _cabs.txt
    └── new_abboip.txt
    └── ...
└── location_entropy.ipynb
└── README.md

## Tools Used
- Python
- Pandas
- NumPy

## Key Insights
- Users exhibit a wide range of mobility behaviors, from highly routine to highly exploratory
- Location entropy effectively distinguishes predictable users from diverse movers
- High-entropy users tend to cover many distinct areas, while low-entropy users concentrate on a few locations
- Small discrepancies between metadata counts and processed records indicate proper data cleaning rather than data loss

## Business Impact
### Mobility Profiling & Fleet Optimization
Segment drivers or users based on movement diversity to:
- Optimize fleet deployment
- Improve driver assignment strategies
- Design personalized incentives

### Urban Planning & Smart Cities
Aggregate entropy metrics across regions to:
- Identify mixed-use and high-activity zones
- Improve public transportation planning
- Detect underutilized urban areas

### Anomaly & Event Detection
Sudden changes in entropy patterns can indicate:
- Traffic disruptions
- Large-scale public events
- Abnormal operational behavior
- Such insights can power real-time monitoring systems.

<hr>

### Product Ideas
Product Idea 1: Mobility-Based User Segmentation
- Segment users by entropy: routine vs exploratory
- Applications:
    - Targeted services
    - Urban planning
    - Transportation optimization

Product Idea 2: Anomaly Detection
- Monitor sudden changes in user entropy
- Use cases:
    - Fraud detection
    - Vehicle misuse
    - Emergency detection

Product Idea 3: Personalized Recommendations<
- Low entropy - recommend nearby services
- High entropy - recommend discovery-based offers
- This directly addresses their “creative application” feedback.

# Conclusion
This project demonstrates how spatio-temporal data and information theory can be combined to generate meaningful insights into human mobility. The approach is scalable, interpretable, and suitable for real-world deployment.