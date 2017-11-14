# PyData NYC November 2017

## Set up
```
git clone git@github.com:parsing-science/pydata_nyc_nov_2017.git
cd pydata_chicago_june_2017
virtualenv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Present slides
```
jupyter-nbconvert --to slides Talk.ipynb --post serve
```

## Create and present slides

### Step 1: Convert slides to HTML
```
jupyter-nbconvert --to slides Talk.ipynb
```

### Edit the html file
Make font bigger:
```
   Reveal.initialize({
        width: '100%',
        height: '100%',
```

Also set scroll=true in setScrollingSlide function.

### Run the slides with HTTPServer
```
python -m http.server
```

### Go to the slides in your browser
Go to http://127.0.0.1:8000/Talk.slides.html in browser.