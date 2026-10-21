docker build -t greeter:v1 devops-2027-shoplist/lessons/02-docker-basics/homework/greeter
docker run -d --name greeter -p 9000:80 


כל השלבים עד COPY app.py כי זה הקובץ הראשון שמשתנה והקבצים שלפניו לא משתנים
