# HW2

List of commands used are:

Forecast:
GET request: /forecast/{DATE}
Input: DATE (string)
Output: Json containing list of seven days data with status code
Status code: 200 OK is returned

GET request: /historical/{DATE}
Input: DATE (string)
Output: json containing {DATE, TMAX, TMIN} 
Status code: 202 OK is returned along with json if DATE is found or else 404 is returned.

GET request for retreiving the whole data information: /historical/
Input: No input is given
Output: provides a list of all dates
status code: 200 OK is returned

DELETE request: /historical/{DATE}
Input: DATE (string)
Output: status code 
status code: 204 is returned

POST request /historical
Input: Json which contains DATE, TMAX, TMIN
Output: Json along with status code
Status code: 201
