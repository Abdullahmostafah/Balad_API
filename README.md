# 🧪 Restful-Booker API Testing with Postman

This project contains a Postman collection designed to test the public Restful Booker API as part of an API testing assessment.

## 📌 Table of Contents
- [Assessment Tasks](#assessment-tasks)
- [Tools Used](#tools-used)
- [How to Use](#how-to-use)
- [Files in the Repository](#files-in-the-repository)
- [API Base URL](#api-base-url)
- [Status](#status)
- [Author](#author)

## 📌 Assessment Tasks

The Postman collection includes the following test cases:

### Auth - CreateToken
- **Endpoint**: `POST /auth`
- **Description**: Generates an authentication token.
- **Details**: Saves the token using a Postman variable for reuse in subsequent requests.

### Booking - CreateBooking
- **Endpoint**: `POST /booking`
- **Description**: Creates a new booking.
- **Details**: Asserts that a `bookingid` is returned and saves it in a variable.

### Booking - UpdateBooking
- **Endpoint**: `PUT /booking/{id}`
- **Description**: Updates all fields of an existing booking.
- **Details**: Asserts that the booking is updated correctly.

### Booking - PartialUpdateBooking
- **Endpoint**: `PATCH /booking/{id}`
- **Description**: Updates only the name fields.
- **Details**: Asserts that `firstname` and/or `lastname` are correctly updated.

### Booking - DeleteBooking
- **Endpoint**: `DELETE /booking/{id}`
- **Description**: Deletes a booking.
- **Details**: Asserts that the response status code is `201`.

## 🧰 Tools Used
- **Postman**: For sending requests and running assertions.
- **Postman Collection Runner**: For executing the full test flow.
- **Environment Variables**: Used for managing token, booking ID, and other dynamic data.

## ▶️ How to Use
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Abdullahmostafah/Balad_API.git
   ```
2. **Import the Postman Collection**:
   - Open Postman.
   - Navigate to `Collections` → `Import`.
   - Select the `restful-booker-collection.postman_collection.json` file from the repository.
3. **Import the Environment (Optional)**:
   - If provided, import the `restful-booker-environment.postman_environment.json` file.
   - Select it in the environment dropdown in Postman.
4. **Run the Collection**:
   - Click `Run` on the collection to execute all requests in sequence.

## 📁 Files in the Repository
```
Balad_API/
├── BALAD.postman_collection.json
├── BALAD_API.postman_collection
├── Balad_Test_Environment.postman_environment
└── README.md
```

## 🔗 API Base URL
`https://restful-booker.herokuapp.com`

## ✅ Status
✔️ Completed and Ready for Review

## ✍️ Author
**Abdullah Mostafa**  
GitHub: [@Abdullahmostafah](https://github.com/Abdullahmostafah)
