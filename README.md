# Example for Werkzeug 0.15.4 to 0.15.5 regression

## Steps

* Setup python virtual environment

* Install either requirements with either `pip install -r 15-5.txt` or `pip install -r 15-4.txt`

* See error when running `flask run` with Werkzeug 0.15.5 but not with 0.15.4 (both work when ran as `python -m flask run`)


### Example 0.15.5 output
```
(venv) C:\Users\conno\Desktop\werk_ex [master ≡]> flask run
 * Serving Flask app "application.py" (lazy loading)
 * Environment: development
 * Debug mode: on
 * Restarting with stat
c:\users\conno\desktop\werk_ex\venv\scripts\python.exe: No module named C:\Users\conno\Desktop\werk_ex\venv\Scripts\flask
(venv) C:\Users\conno\Desktop\werk_ex [master ≡]> python -m flask run
 * Serving Flask app "application.py" (lazy loading)
 * Environment: development
 * Debug mode: on
 * Restarting with stat
 * Debugger is active!
 * Debugger PIN: 316-770-638
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```

### Example 0.15.4 output
```
(venv) C:\Users\conno\Desktop\werk_ex [master ≡]> flask run
 * Serving Flask app "application.py" (lazy loading)
 * Environment: development
 * Debug mode: on
 * Restarting with stat
 * Debugger is active!
 * Debugger PIN: 816-527-897
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
(venv) C:\Users\conno\Desktop\werk_ex [master ≡]> python -m flask run
 * Serving Flask app "application.py" (lazy loading)
 * Environment: development
 * Debug mode: on
 * Restarting with stat
 * Debugger is active!
 * Debugger PIN: 316-770-638
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```
