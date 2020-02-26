# Customer Import Platform

### Assignment
A system that imports CSV files with certain parameters. After file import, a **Customer** entity is created with appropriate fields.

CSV file must contain the following mandatory values:
`first_name`, `last_name`, `email`, `date_of_birth`

The system is available by: https://testtaskmatic.herokuapp.com

### Requirements
* Cover the platform at least by one automation test
* Use **Ruby** as the primary language for the tests
* Use **Rspec** framework in your solution

### Recommendations
* You may use any gems that you like
* You could write API and UI tests
* Not necessary to cover all possible cases, just decide which are the most important


### The platform has following API endpoints:

**Create import:**
```
POST /api/imports
content-type: multipart/form-data
import[file]=@list.csv
import[title]=MyImport
```

**Start import:**
```
POST /api/imports/<import_id>/start
```

**Get import:**
```
GET /api/imports/<import_id>
```

**Get customers:**
```
GET /api/imports/<import_id>/customers
```

**Delete import:**
```
DELETE /api/imports/<import_id>
```

**Authorization Header:**

`Authorization: Bearer 1f43d455fgjkgfjgf48`

As you work on your solution you will inevitably have questions - please send all inquiries via slack. We are happy to assist and help
