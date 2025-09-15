🚀 CodeBook – Social Media Data Science Project

📖 Overview

CodeBook is a mini social network simulation built entirely in pure Python (without pandas, NumPy, or fancy libraries).
It demonstrates how raw JSON data can be loaded, cleaned, and analyzed to build real-world features like:

👥 People You May Know – friend recommendations based on mutual friends

📑 Pages You Might Like – page recommendations based on shared interests

📝 Tasks Breakdown
✅ Task 1: Load & Explore the Data

Load the JSON dataset containing users, their connections, and pages.

Print users along with their friends and liked pages.

Display the list of available pages.

Learning: Handling JSON data structures in Python and exploring graph-like relationships.

✅ Task 2: Clean the Data

Remove users with missing names.

Deduplicate friend lists for consistency.

Remove inactive users (those with no friends & no liked pages).

Remove duplicate pages with the same ID.

Learning: Data preprocessing & cleaning – a critical step before analysis.

✅ Task 3: People You May Know 👥

Analyze user connections to find mutual friends.

Suggest new friends who are not directly connected.

Rank suggestions based on the number of mutual friends.

Example:
Amit (ID:1) and Sara (ID:4) share Priya (ID:2) as a mutual friend → Sara is recommended to Amit.

Learning: Implementing recommendation logic using graph traversal & set operations.

✅ Task 4: Pages You Might Like 📑

Compare liked pages between users.

Suggest pages that similar users have liked.

Rank pages by the number of shared interests.

Example:
If Amit (ID:1) and Priya (ID:2) both like AI & ML Community (103), and Priya also likes Data Science Enthusiasts (102), then Page 102 is suggested to Amit.

Learning: Basics of collaborative filtering recommendation systems.

🎯 Example Output
Users and their connections:

Amit (ID:1) - Friends: [2,3] - Pages: [101]
Priya (ID:2) - Friends: [1,4] - Pages: [102]
Rahul (ID:3) - Friends: [1] - Pages: [101,103]
Sara (ID:4) - Friends: [2] - Pages: [104]

Pages:
101: Python Developers
102: Data Science Enthusiasts
103: AI & ML Community
104: Web Dev Hub

People You May Know for User 1: [4]
Pages You Might Like for User 1: [103]

🏆 Key Learnings

Working with JSON data in Python.

Performing data cleaning & structuring without libraries.

Implementing graph-based logic for friend recommendations.

Building a simple recommendation engine using collaborative filtering.

📊 Future Enhancements

🔗 Add Flask/FastAPI API endpoints for frontend integration.

🎨 Create a React + Tailwind UI for visualization.

🤖 Upgrade to Machine Learning–based recommendation system for smarter results.
