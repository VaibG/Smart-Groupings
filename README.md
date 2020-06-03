# Smart-Groupings

## Description
A script to automate the generation of small groups within a larger organization utilizing Messenger API and Airtable API. Small group bonding sessions are essential to strengthen an organization's relationships, empathy, and culture by connecting peers together to get to know each other better. While Slack does have a donut bot feature that does a similar thing, this algorithm is customizable to many different factors including size of the group, the probability of people being paired with each other again, people joining the organization in different semesters do not get paired with each other and the ability to add your own customized features. 

The algorithm is built in python and assigns an initial weight to every possible pairing. This weight represents the probability of person A being matched with person B. It then randomly generates groups using these weights. Once the groups are generated, it will use the *unofficial* messenger API to send a custom message to the group. It then loads the groups into an Airtable base using the Airtable API, where a form should be set up such that the group can fill out the form when they meet up (tracking attendance). Based on whether the group met up or not, it will update the weightings accordingly and reset the airtable base for the generation of the next group pairings. 

## Usage
1. Install the dependancies (`pip install`)
2. Use Jupyter Notebook to run the notebook
3. Enter Facebook account Email and Password 
4. Set up Airtable Base and connect using Base ID and API_key. You can then set up the form generated from that table.
5. Upload the roster.csv in the same folder/enter the file path to the roster.
6. Follow the instructions on the notebook and enjoy the productivity of small groups!
