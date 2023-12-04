## How to Create a Flask + React Project | Python Backend + React Frontend

https://www.youtube.com/watch?v=7LNl2JlZKHA

# Steps:
1. Create the folder that contains the backend files. Type in the terminal:
mkdir flask-server
cd flask-server
touch server.py

2. Create react app
npx create-react-app client

3. Create virtual environment
python3 -m venv
source venv/bin/activate

4. Install Flask
pip3 install Flask

5. Write condes in server.py

6. Run the app
python3 server.py

7. Check the local host is working
http://127.0.0.1:5000/members

8. Connect React to backend. <package.json> (line 5):
"proxy": "http://127.0.0.1:5000",

9. Clean the app. Delete: 
- app.test.js
- logo
- index.js: 
- delete import .css
- app.js Delete all

10. app.js:
