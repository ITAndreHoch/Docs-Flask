
**TEMPLATES**







***Key facts***

* Templates are stored in the /templates/ directory
* A template is an HTML file (Flask uses the Jinja template engine)
* Templates can contain Python variables using this syntax {‌{x}}
* Python functions can return templates

```
# your function
return render_template('example.html')
Don't forget the line

# top of python file
import from flask import Flask, render_template, request
```

