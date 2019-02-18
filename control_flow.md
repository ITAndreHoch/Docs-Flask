
***

***Use case*** - show only page if variable = Alice



cat control.py 

```

from flask import Flask, render_template

app = Flask(__name__)


@app.route('/<user>')
def hello_name(user):
    return render_template('control.html', name = user)


app.run(host='0.0.0.0', port= 5000)

```



cat ./templates/control.html 

```
  {% if name == 'Alice': %}
      <h1>Hello  - {{name}} !</h1>
  {% endif %}

```
<img src="images/flask6.png " alt="drawing" width="300"/>

We can add elsif condition:

```
 {% if name == 'Alice': %}
      <h1>Hello  - {{name}} !</h1>
  {% else %}
      <h1> Oh no - wrong path {{name}}! </h1>
  {% endif %}
      
```

<img src="images/flask7.png " alt="drawing" width="300"/>



