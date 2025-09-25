# JMeter API Test Plan

This repository contains a sample **Apache JMeter test plan** designed to demonstrate API testing and basic load testing skills.  

## 📂 Contents
- `api_test_plan.jmx` → JMeter test plan file.  
- `README.md` → Project documentation.  

## 🛠 Requirements
- [Apache JMeter 5.6+](https://jmeter.apache.org/download_jmeter.cgi)  
- Java 8 or higher  

## ▶️ How to Run
1. Download and install Apache JMeter.  
2. Open JMeter and load the test plan:  
3. Run the test by clicking the green **Start** button (▶).  
4. View results in:  
- **Summary Report** (aggregated results)  
- **View Results Tree** (detailed request/response info)  

## 📊 Test Plan Overview
- **Thread Group**:  
- 10 concurrent users  
- 20-second ramp-up time  
- Each user loops 5 times  

- **HTTP Request**:  
- Method: `GET`  
- URL: `https://jsonplaceholder.typicode.com/posts`  

- **Assertions**:  
- Verifies that the **response code = 200**  

- **Listeners**:  
- Summary Report  
- Results Tree  

## ✅ Expected Results
- All responses should return **HTTP 200 OK**.  
- The Summary Report will display response time, throughput, and error % for each request.  

---

📌 This sample demonstrates the ability to:  
- Design and run JMeter API test plans  
- Validate responses with assertions  
- Analyze test results through reports  
