# django-analytics

## How to make this application run

1. Make sure you have Django 2.2 installed

        pip install Django==2.2

2. Run the application

        python manage.py runserver
        
3. Check the web application on your browser

        http://localhost:8000
        

## Add some data

1. Enter the Project interactive console

        python manage.py shell
        
2. Execute the following (line by line)

        from dashboard.models import Order
        o1 = Order(product_category='Books', payment_method='Credit Card', shipping_cost=39,unit_price=59.22)
        o1.save()
        o2 = Order(product_category='Newpaper', payment_method='Credit Card', shipping_cost=9,unit_price=12.00)
        o2.save()
        ...(add as many as you wish)
        
3. Run the appliciation again and, this time, check the following address

        http://localhost:8000/dashboard/
        
        
## More information

This project has been developed following the instructions at: https://www.freecodecamp.org/news/how-to-create-an-analytics-dashboard-in-django-app/

Although it was a very good exercise, the reader must know that the front end library used for this purpose is under license (more informmation: https://www.flexmonster.com/)

        