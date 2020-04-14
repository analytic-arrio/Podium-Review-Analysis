# Podium Review Analysis

This project is available for those who wish to see how I analyzed a large dataset (>800k rows) of data from Podium on the reviews that organizations received as a result of using Podium software and the effects therein.
Questions I'm interested in answering:

1. What organization had the best reviews after/while using Podium?
2. Which location had the best reviews after/while using Podium?
3. How should we define 'best' given the data?
4. How did using Podium software affect the quality and quantity of reviews that organizations received? How did it vary across the organizaitons?

Below is a legend that provides definitions for each data point found in the raw data:

data/organizations/organizations.csv (1 file)
- organization_id: unique ID for the organization.
- organization_name: name of organization.
- organization_start_date: date the organization joined Podium.
data/locations/locations.csv (1 file)
- location_id: unique ID for the location.
- organization_id: unique ID for the organization.
- location_start_date: date the location joined Podium.
data/invites/review-invitations.csv (1 file)
- invitation_id: unique ID for the invitation.
- organization_id: unique ID for the organization.
- invitation_sent_at: date the review invitation was sent by Podium’s software.
- location_id: unique ID for the location.
data/reviews/reviews-location-*.csv (58 files, includes both organic and solicited reviews)
- review_id: unique ID for the review.
- rating: star rating for the review (numeric).
- publish_date: date that the review was published.
- location_id: unique ID for the location.
- organization_id: unique ID for the organization.
- invitation_id: unique ID for the invitation (can be used to identify which reviews are solicited from
invitations sent via Podium).


Required Libraries

pandas
numpy
glob
matplotlib

NOTE: This project only runs on Python 3

Getting Started

NOTE: 
(1) Given the sheer size of the csv files, I did not make them directly accessible; you will need to unzip them and likely download to your local machine.
(2) Replace the filepath in the pynb file above with the filepaths from your local machine before running the code. You will likely need to wait a while for it to run.

Authors

Arrio Hoffman
