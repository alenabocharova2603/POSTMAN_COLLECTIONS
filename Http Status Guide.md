# HTTP Status Codes Reference

This repository provides an enumeration of HTTP status codes with descriptions, implemented in Java. HTTP status codes are essential in defining the responses returned by servers for various requests.

## Overview

The `HttpStatus` enumeration includes the most common HTTP status codes, grouped into categories for easier navigation:

- **1xx (Informational)**: Request received, continuing process.
- **2xx (Successful)**: The action was successfully received, understood, and accepted.
- **3xx (Redirection)**: Further action must be taken to complete the request.
- **4xx (Client Error)**: The request contains bad syntax or cannot be fulfilled.
- **5xx (Server Error)**: The server failed to fulfill an apparently valid request.

## Usage

You can use this enumeration in your Java projects to standardize and simplify working with HTTP status codes. Each code is defined as a constant with an integer value and a description.

### Example

```java
// Example usage of the HttpStatus enum
HttpStatus status = HttpStatus.OK;
System.out.println("Status code: " + status.getCode());
System.out.println("Description: " + status.getDescription());
```

### Output
```
Status code: 200
Description: OK
```

## HTTP Status Code Categories

### 1xx Informational

- **100 CONTINUE**: The server has received the request headers and the client should proceed to send the request body.
- **101 SWITCHING_PROTOCOLS**: The requester has asked the server to switch protocols.

### 2xx Successful

- **200 OK**: The request was successful.
- **201 CREATED**: The request has been fulfilled and resulted in a new resource being created.
- **204 NO_CONTENT**: The server successfully processed the request, but is not returning any content.

### 3xx Redirection

- **301 MOVED_PERMANENTLY**: The URL of the requested resource has been changed permanently.
- **302 FOUND**: The resource is temporarily located at a different URL.
- **304 NOT_MODIFIED**: The resource has not been modified since the version specified by the request headers.

### 4xx Client Error

- **400 BAD_REQUEST**: The server could not understand the request due to invalid syntax.
- **401 UNAUTHORIZED**: The client must authenticate itself to get the requested response.
- **403 FORBIDDEN**: The client does not have access rights to the content.
- **404 NOT_FOUND**: The server can not find the requested resource.

### 5xx Server Error

- **500 INTERNAL_SERVER_ERROR**: The server has encountered a situation it doesn't know how to handle.
- **501 NOT_IMPLEMENTED**: The server does not support the functionality required to fulfill the request.
- **503 SERVICE_UNAVAILABLE**: The server is not ready to handle the request.

## How to Contribute

If you want to add more HTTP status codes or improve this repository, feel free to:

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature/add-status-code`.
3. Commit your changes: `git commit -m 'Add HTTP status code XYZ'`.
4. Push to the branch: `git push origin feature/add-status-code`.
5. Open a Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

If you have any questions or suggestions, feel free to open an issue in the repository or contact the maintainer at [your-email@example.com].
