# Timestamp Microservice

This is the boilerplate code for the Timestamp Microservice project. Instructions for building your project can be found at https://www.freecodecamp.org/learn/apis-and-microservices/apis-and-microservices-projects/timestamp-microservice
🔗 API Endpoint
GET /api/:date?


✅ Valid Inputs
- /api/2015-12-25
- /api/1451001600000
- /api/ (returns current time)
❌ Invalid Input
- /api/not-a-date
📄 Example Responses
|  |  | 
| /api/2015-12-25 | { "unix": 1451001600000, "utc": "Fri, 25 Dec 2015 00:00:00 GMT" } | 
| /api/1451001600000 | { "unix": 1451001600000, "utc": "Fri, 25 Dec 2015 00:00:00 GMT" } | 
| /api/ | { "unix": <current ms>, "utc": "<current UTC>" } | 
| /api/invalid-date | { "error": "Invalid Date" } | 


✅ Passed Test Cases
- Custom project URL used instead of example placeholder
- Valid date returns correct unix timestamp (Number)
- Valid date returns correct utc string in format: Thu, 01 Jan 1970 00:00:00 GMT
- Unix timestamp input returns correct conversion
- Accepts any date string parsable by new Date(date_string)
- Invalid date returns { error: "Invalid Date" }
- Empty date returns current time in unix
- Empty date returns current time in utc

