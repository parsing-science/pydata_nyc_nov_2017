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

### Step 2: Edit the html file
Make font bigger:
```
   Reveal.initialize({
        width: '100%',
        height: '100%',
```

Allow scrolling by setting scroll = true:
```
 function setScrollingSlide() {
    var scroll = true
```

Change h3 font-weight:
```
.rendered_html h3{
    font-weight: normal;
}
```

### Step 3: Run the slides with HTTPServer
```
python -m http.server
```

### Step 4: Go to the slides in your browser
Go to http://127.0.0.1:8000/Talk.slides.html in browser.