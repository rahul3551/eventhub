# EventHub

## Run

pip install -r requirements.txt

python manage.py migrate

python manage.py runserver

## Endpoints

GET /api/events/
POST /api/events/

GET /api/reservations/
POST /api/reservations/

POST /api/reservations/<id>/cancel/

## Design Decision

Reservation creation deducts available seats inside the serializer create() method so reservation creation and seat deduction stay together.