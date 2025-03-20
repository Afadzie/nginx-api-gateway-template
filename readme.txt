
Step 1: Install Dependencies
............................

docker-compose down
rm -rf nginx/nginx.conf
rm -rf jwt/auth.lua

Step 2: Build & Run
...................

docker-compose up -d --build


Step 3: Test API Gateway
Without JWT (Unauthorized):
............................

curl -X GET http://localhost/service1/

Response : {"error": "Missing Authorization Header"}


With JWT:
.........

{"error": "Missing Authorization Header"}



