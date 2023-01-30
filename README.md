# LightBnbjs
A database application project developed as a part of Lighthouse Labs Web development course.
The front-end is forked from lighthouse-labs/LightBnB_WebApp Install the LightBnB_WebApp npm install, run it npm run local, and view it at localhost:3000.
ERD Info
users

id: Primary Key
name
email
password
property_types

id: Primary Key
type
properties

id: Primary Key
title
description
thumbnail_photo_url
cover_photo_url
owner_id : Foreign Key users(id)
cost_per_night
country
street
city
province
postal_code
parking_spaces
number_of_bedrooms
number_of_washrooms
property_type : Optional, defaults to 1, in future may references property_types(id)
active
reservations

id: Primary Key
start_date
end_date
property_id : Foreign Key properties(id)
guset_id : Foreign Key users_id(id)
property_reviews

id: Primary Key
guest_id : Foreign Key users(id)
property_id : Foreign Key properties(id)
reservation_id : Foreign Key reservations(id)
message
rating

![lightbnb2](https://user-images.githubusercontent.com/111916382/215593248-b76f7779-f19b-43fe-a119-8d452cd1f978.png)
![Screenshot 2023-01-30 102057](https://user-images.githubusercontent.com/111916382/215593328-5d23cb41-ec5f-43b0-b064-3d0e40c787b1.png)



