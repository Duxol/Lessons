# HOW TO USE "VENV" MODULE IN PYTHON USING THE TERMINAL

## 1. SETTING UP A VIRTUAL ENVIRONMENT:
`python3 -m venv My_project/venv`  
or  
`python3 -m venv venv (if it is in the same directory)`  
`python3 -m venv venv --system-site-packages (to incldue system packages)`  

## 2. CREATE REQUIREMENTS FILE AND .GITIGNORE
`touch requirements.txt`  
`pip freeze --> paste into requirements.txt`  
    
`touch .gitignore`  
`add "venv" to the file`

## 3. TO ACTIVATE ON WINDOWS:
`venv\Scripts\activate.bat`  
`pip install -r requirements.txt`  

## 3. TO ACTIVATE ON MAC/LINUX:
`source venv/bin/activate`

