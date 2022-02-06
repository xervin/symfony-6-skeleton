Install:
1. docker-compose up -d --build
2. docker-compose exec app symfony new .
3. cp app/.env app/.env.local
4. insert .env.local DATABASE_URL=mysql://{root_user_name}:{root_pass}@db:3306/{database_name}?serverVersion=8.0

Additional:
* docker-compose exec app composer req --dev maker ormfixtures fakerphp/faker
* composer req doctrine twig

Based on: https://www.twilio.com/blog/get-started-docker-symfony
