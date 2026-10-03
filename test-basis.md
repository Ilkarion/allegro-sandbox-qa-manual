## 1. Purpose

This document defines the functional behavior and business rules
used as a basis for testing Allegro Sandbox.

Since formal product requirements are not available,
the test basis is derived from:
- observed application behavior
- UI elements and available functionality
- publicly visible information
- testing assumptions
- identified open questions

---

## 2. Authentication

### Registration

The user should be able to:
- open the registration page
- enter required registration data
- submit the registration form
- receive validation messages for invalid data
- successfully create an account when valid data is provided

### Login

The user should be able to:
- enter valid credentials
- log in successfully
- receive an error for invalid credentials
- receive validation messages for invalid or missing input

### Logout

The user should be able to:
- log out from the account
- be redirected to an appropriate page
- no longer access authenticated functionality

---

## 3. Search

### Search Input

The user should be able to:
- enter a search phrase
- submit the search
- view products matching the search phrase

### Categories

The user should be able to:
- select a product category
- navigate between categories
- view products belonging to the selected category

### Filters

The user should be able to:
- open available filters
- select filter values
- apply filters
- clear filters
- view products matching selected filters

---

## 4. Product

The user should be able to:
- open a product page
- view product information
- add the product to the cart

---

## 5. Cart

The user should be able to:
- view products in the cart
- change product quantity
- remove a product
- view the updated cart total

---

## 6. Responsive Behavior

The application should remain usable at the defined
screen resolutions.

The following areas should be checked:
- navigation
- search
- product pages
- filters
- cart
- buttons and interactive elements
- text visibility
- horizontal/vertical scrolling

---

## 7. API Testing

API testing will focus on the publicly available Allegro API and its observable behavior.

### 7.1 Authorization

Allegro API authentication is based on OAuth 2.0 rather than a dedicated REST login or registration endpoint.

The following authorization functionality will be considered:

* OAuth 2.0 authorization flow
* Authorization code generation
* Access token generation
* Access token validation
* Handling of invalid or missing authorization data
* Handling of unauthorized requests
* Authenticated API requests

### 7.2 Authenticated User

The authenticated user endpoint will be tested to verify access to user-specific API resources.

**Endpoint:**
`GET /me`

The following will be checked:

* Successful request with a valid access token
* Request without an access token
* Request with an invalid access token
* Response HTTP status code
* Response body
* Response structure
* Returned user information

### 7.3 Search API

Available search-related API endpoints will be tested to verify:

* Successful search requests
* Search by text
* Search using supported parameters
* Valid and invalid parameter values
* Missing required parameters
* Empty search results
* HTTP status codes
* Response structure and data

### 7.4 Cart API

Available cart-related API functionality will be tested where supported by the Allegro API.

The following will be checked:

* Adding a product to the cart
* Removing a product from the cart
* Changing product quantity
* Requests with valid and invalid data
* Authorization requirements
* HTTP status codes
* Response body and structure
* Error handling

### 7.5 Negative API Testing

Negative scenarios will be used to verify API behavior when invalid or incomplete requests are sent.

Examples include:

* Missing required parameters
* Invalid parameter values
* Invalid resource identifiers
* Missing authorization
* Invalid or expired access token
* Unsupported HTTP methods
* Invalid request body

### 7.6 API Limitations

The Allegro API does not provide dedicated REST endpoints for directly testing username/password login or user registration.

Therefore, API testing will not attempt to reproduce the website's login or registration forms through REST requests. Instead, authentication testing will focus on the documented OAuth 2.0 authorization flow and authenticated API resources.

### 7.7 Expected API Behavior

The following general API characteristics will be verified:

* HTTP status codes
* Response body
* Response structure
* Required parameters
* Authentication and authorization
* Validation of input data
* Error responses
* Consistency of responses for equivalent requests


---

## 8. Assumptions

- Observed application behavior is used as the expected behavior
  when formal requirements are unavailable.
- Sandbox behavior may differ from production.
- Business rules that cannot be verified are treated as assumptions.

---

## 9. Open Questions

- Which product fields are mandatory?
- What are the exact validation rules for registration?
- What are the expected limits for search input?
- Which filters are mandatory/optional?
- What are the exact rules for cart quantity?
