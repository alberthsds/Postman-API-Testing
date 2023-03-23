# 🌟 HTTP

    ➡️ Request - from client
    ➡️ Response - from server

## 🌟 Request

    📌 Contain the address
        ➡️ "https://simple-books-api.glitch.me/status"

    📌 Address API
        ➡️ "https://simple-books-api.glitch.me"

    📌 Endpoint
        ➡️ "/status"

## 🌟 GET status

    ➡️ https://simple-books-api.glitch.me/status

## 🌟 Postman Collection and Variables

    📌 Collection
        ➡️ is a list of multiple requests that are connected by the same API.

    📌 Variables
        ➡️ use all requests. And to use different endpoints.

            📌 Initial Value
                ➡️ public API

            📌 Current Value
                ➡️ private API

## 🌟 Query parameters

    📌 key = name

    📌 value = value

## 🌟 Assignment

    📌 key = limit

    📌 value = 2

    ➡️ limit value : a number between 1 and 20.

## 🌟 Path Varables

    ➡️ https://simple-books-api.glitch.me/books/:bookId

    📌 Path Variables
        ➡️ books/:bookId

## 🌟 Post request

    📌 Submit an order
        ➡️ POST/orders
            ➡️ Allows you to submit a new order. It Requires authentication

            📌 The request body needs to be a JSON format and include the following properties:

                ➡️ bookId ➡️ Integer ➡️ Required

                ➡️ customerName ➡️ String ➡️ Required

## 🌟 API Authentication

    📌 To submit or view an order, you need to register your API client.

    📌 POST /api-clients/

    📌 The request body needs to be in JSON format and include the following properties:

        ➡️ clientName ➡️ String

        ➡️ clientEmail ➡️ String

            📌 Example

                {
                "clientName": "Postman",
                "clientEmail": "valentin@example.com"
                }

    📌 The response body will contain the access token. The access token is valid for 7 days.

       ➡️ Possible errors

       ➡️ Status code 409 - "API client already registered." Try changing the values for clientEmail and clientName to something else.

## 🌟 API Status

    📌 Status

        ➡️ 200 ➡️ Good

        ➡️ 400 ➡️ Bad

        ➡️ 500 ➡️ Server Problem

## 🌟 JSON format

    📌 POST /orders

    📌 Allows you to submit a new order. Requires authentication.

    📌 The request body needs to be in JSON format and include the following properties:

        ➡️ bookId ➡️ Integer ➡️ Required
        ➡️ customerName ➡️ String ➡️ Required

        📌 Example

            POST /orders/
            Authorization: Bearer <YOUR TOKEN>

            {
            "bookId": 1,
            "customerName": "John"
            }

### 🌟 Resources

    🔗 Youtube Link: https://www.youtube.com/watch?v=VywxIQ2ZXw4
    🔗 Github Link: https://github.com/vdespa/introduction-to-postman-course/blob/main/simple-books-api.md
