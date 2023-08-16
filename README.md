## **Documentation: Epoch Converter Utility Program**

### **Introduction:**
This documentation outlines the design, functionality, and usage of the "Epoch Converter" utility program. The program is designed to convert user-provided dates into epoch time using an external API. It includes error handling, logging, and user interaction.

### **Aim:**
The aim of this program is to provide a simple and user-friendly way to convert dates to epoch time using an API. It utilizes Java's HttpClient, BufferedReader, and JSON parsing libraries to interact with the API and manage user input/output.

### **UML Diagrams:**
No UML diagrams are explicitly provided in the code.

### **Flowchart:**
No flowchart is explicitly provided in the code.

### **Code:**
```java
// The complete code is provided in the source file "EpochConverter.java".
// Please refer to the source code for the detailed implementation.
```

### **Explanation:**
1. The program starts by initializing the logging system using Log4j and reading configuration values from a properties file.
2. It enters an infinite loop that repeatedly prompts the user to input a date in the "YYYY-MM-DD" format.
3. The input date is validated using the `isValidDateFormat` function, which attempts to parse the input as a LocalDate and returns true if successful.
4. An HTTP request is created using HttpClient to an external epoch converter API. The API is provided with the input date, and the response is received and stored.
5. The JSON response from the API is parsed using the JSONObject class. The epoch time is extracted and displayed to the user.
6. The program then prompts the user if they want to convert another date. If "Y" is entered, the loop continues. If "N" is entered, the program terminates.
7. Error handling is implemented for various exceptions that may occur during the program's execution.

### **Conclusion:**
The "Epoch Converter" utility program demonstrates how to interact with an external API to convert user-provided dates to epoch time. It utilizes HTTP requests, JSON parsing, logging, and user interaction to achieve its goal. The code showcases error handling mechanisms to ensure smooth execution even in the presence of exceptions.

### **References:**
- Java Documentation: https://docs.oracle.com/en/java/
- HttpClient Documentation: https://docs.oracle.com/en/java/javase/11/docs/api/java.net.http/java/net/http/HttpClient.html
- JSONObject Documentation: https://stleary.github.io/JSON-java/index.html
- Log4j Documentation: https://logging.apache.org/log4j/2.x/manual/index.html
