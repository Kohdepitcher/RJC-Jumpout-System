#  RJC Jumpout System
The Rockhampton Jockey Club is a local Thoroughbred racing club located within Rockhampton Queensland. On top of conducting race meetings, they also host Jumpouts to help educate race horses on the procedures for race meetings. Currently, nominations for Jumpouts are made over various communication mediums including telephone, email, messages, and all data entry is handled manually on a spreadsheet. They were seeking to find a small online system that would make handling Jumoputs and nominations easier and free up time for their office staff.

It is intended that office staff can easily add upcoming Jumpout meetings to the system so that trainers can login and nominate for these Jumpouts. Admin staff will be able to see all the nominations for each Jumpout and be able to easily create the fields that will be used on the morning of to organise the right horse into the right jump out and barrier position. The online system can keep trainers and RJC staff on the same page and reduce time spent collecting nominations. 

This project is still in development

## Technologies
This project utilises a variety of technologies and frameworks for all parts of the project. The front end is built as an Angular (not AngularJS) web app which utilises the Angular Material UI library for the User Interface elements and the AngularFire sdk for interactions with Firebase services including authentication.

The backend of the website consists of an REST API built as NodeJS middleware that communicates between the client and the Database. The middleware is written in Typescript and runs in Firebase Cloud Functions which means the backend is built to be server less. By building it to be server less, running costs are reduced as functions only run as requested by the REST API. The backend is secured via bearer auth tokens in which the middleware will reject any requests to endpoints where the token is missing, invalid, or the user of the token doesn't have the correct role.

For the Database component of the backend, MySQL is used running on Google Cloud SQL which is then interacted with via TypeORM, an ORM library to make interactions easier and enabled an easier modelling of objects.

 - Back end
	 - MySQL running inside Google Cloud SQL
	 - TypeORM - object-relational mapping library
	 - Express - middleware library
	 - TypeScript and NodeJS
	 - Firebase Admin SDK
 - Front end
	 - Angular
	 - AngularFire - Firebase Angular SDK
	 - Angular Material UI
	 - Typescript

## User interface
**Jumpout Meetings Page - Admin View**
List view of Jumpouts within a date range<a  href="https://drive.google.com/uc?export=view&id=14mY9kRg5wkkNZ8TldiDtVP8faU3XlnFR"><img  src="https://drive.google.com/uc?export=view&id=14mY9kRg5wkkNZ8TldiDtVP8faU3XlnFR" style="width: 500px; max-width: 100%; height: auto" title="Click for the larger version." /></a>

More menu for a Jumpout<a  href="https://drive.google.com/uc?export=view&id=1GqfB8qZXJNL1vKawdrParThzpPSVM51h"><img  src="https://drive.google.com/uc?export=view&id=1GqfB8qZXJNL1vKawdrParThzpPSVM51h" style="width: 500px; max-width: 100%; height: auto" title="Click for the larger version." /></a>



**Nominations Page**
List of all nominations for a Jumpout<a  href="https://drive.google.com/uc?export=view&id=1Lc-0hV8FQ0g8kuJNpOwcCGPkTQUOkDFX"><img  src="https://drive.google.com/uc?export=view&id=1Lc-0hV8FQ0g8kuJNpOwcCGPkTQUOkDFX" style="width: 500px; max-width: 100%; height: auto" title="Click for the larger version." /></a>

List of all trainers and their count of nominations<a  href="https://drive.google.com/uc?export=view&id=1nUuWJlIDR_IZ37d5LxFdlgyU4dN1rdjm"><img  src="https://drive.google.com/uc?export=view&id=1nUuWJlIDR_IZ37d5LxFdlgyU4dN1rdjm" style="width: 500px; max-width: 100%; height: auto" title="Click for the larger version." /></a>


**User Management Page**
List of users<a  href="https://drive.google.com/uc?export=view&id=1w_W2UFFe6Iqs8Vsg436Ng8C9Xj7s8KXG"><img  src="https://drive.google.com/uc?export=view&id=1w_W2UFFe6Iqs8Vsg436Ng8C9Xj7s8KXG" style="width: 500px; max-width: 100%; height: auto" title="Click for the larger version." /></a>

