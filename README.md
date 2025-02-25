Flask app with postgres database (2 tier application )

Make sure you install docker and docker compose(apt install docker.io -y apt install docker-compose )

Then git clone https://github.com/avadaequare/Twotier-app.git

docker-compose up -d to run in application in background

This command runs the flask app and database two containers so now you can access the app at http://localhost:5000 to access our application if you deployed it in vm then 
replace localhost with public ip of vm.

Now we have two conatiners created one for flask app and postgres they are connected to each other.

Now as you can access you can type data in the column and it will be stored in postgres container.

You can check postgres container docker exec -it 704079456e63 psql -U postgres -d mydatabase you will get into postgres container you can give /dt to ✅ 
This will list all tables in your database and then SELECT * FROM data; you will get all data that you have stored in web app.

<img width="950" alt="image" src="https://github.com/user-attachments/assets/945ea810-5340-4ee7-8925-3a392209cc30" />
