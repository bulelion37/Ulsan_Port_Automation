# Ulsan_Port_Automation

> #### System for applicating reservation and searching Ulsan Port Yard


##### Language: JAVA, IntelliJ, Gradle
##### Function: API for applying, searching, and approving the company's yard reservation.

------------
------------
## Database Schema
<img src="https://user-images.githubusercontent.com/57051773/101279950-624ce600-3809-11eb-8c78-94370476fae8.jpg" width="100%">

### Entity
> ##### Wharf: Information on the yard (name, type [main port/new port], area, excluded area)
> ##### Company: Information about the company (company code, company name, number of warnings)
> ##### Orders: Company's reservation application information for the yard (Type, approval status, start date, end date, and other key information)
> ##### Usages: Information on the company's actual use of the yard (start date, end date, area, use company, use yard)
> ##### Fee: Rate information for use by type of yard (charge, type of yard)
> ##### Info: Information on announcements (notice title, announcement content)

------------
------------
## API
> ### GetMethod(ex)
> ##### [Get]http://localhost:8080/usage 
> ###### Response: 
<img src="https://user-images.githubusercontent.com/57051773/101280677-c5407c00-380d-11eb-8a14-cbb7fe4e578d.JPG" width="60%">

> ##### [Get]http://localhost:8080/usage/2 
> ###### Response: 
<img src="https://user-images.githubusercontent.com/57051773/101280684-cec9e400-380d-11eb-930e-1cd0172571e0.JPG" width="60%">

------------
> ### PostMethod(ex)
> ##### [Post]http://localhost:8080/usage 
> ###### Request body: 
> `{
	"start_date": "2020-11-06",
 	"end_date": "2020-11-08",
 	 "area": 3512,
  	"company_id": 5,
 	 "wharf_id": 4
}`
> ###### Response: 
<img src="https://user-images.githubusercontent.com/57051773/101280686-d8ebe280-380d-11eb-8bfb-0552db3bb9fc.JPG" width="60%">

------------
> ### PutMethod(ex)
> ##### [Put]http://localhost:8080/usage 
> ###### Request body:
> `{
    "id": 8,
	"start_date": "2020-11-06",
 	"end_date": "2020-11-08",
 	 "area": 3512,
  	"company_id": 5,
 	 "wharf_id": 4
}`
> ###### Response: 
<img src="https://user-images.githubusercontent.com/57051773/101280693-e6a16800-380d-11eb-86b3-25b784c4afe2.JPG" width="60%">

------------
> ### DeleteMethod(ex)
> ##### [Delete]http://localhost:8080/usage 
> ###### Response: 
<img src="https://user-images.githubusercontent.com/57051773/101280707-f325c080-380d-11eb-8810-0764f989a6bb.JPG" width="60%">

------------
------------
## Screenshot
<img src="https://user-images.githubusercontent.com/57051773/101280915-48ae9d00-380f-11eb-8af5-e81d133a4bde.JPG">
<img src="https://user-images.githubusercontent.com/57051773/101280918-4ba98d80-380f-11eb-8e5a-1d39bc15fb0c.JPG">

