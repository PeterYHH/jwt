# JWT Encoder/Decoder Tool

A simple, client-side web tool for encoding and decoding JSON Web Tokens (JWTs). This tool runs entirely in your browser, ensuring your secrets and tokens never leave your machine.

## Features

- **Decode JWTs:** Paste a JWT to view its header, payload, and signature.
- **Token Validity Check:** Automatically checks token validity based on `exp` (expiration) and `nbf` (not before) claims, displaying a clear status (e.g., Valid, Expired).
- **Expiration Countdown:** Shows a live countdown for valid tokens, indicating the remaining time until expiration.
- **Encode JWTs:** Create a new JWT by providing a header, payload, and a secret key.
- **HMAC Algorithm Support:** Supports HS256, HS384, and HS512 algorithms for signing.
- **Copy to Clipboard:** Easily copy the generated JWT with a single click.
- **Client-Side Only:** All operations are performed in your browser using the Web Crypto API. No data is sent to any server.
- **Responsive Design:** Usable on both desktop and mobile devices.

## How to Use

1.  Clone this repository or download the `index.html` file.
2.  Open the `index.html` file in your web browser.

### To Decode

1.  Select the "Decode JWT" tab.
2.  Paste your JWT into the input field.
3.  The decoded header, payload, and signature will be displayed automatically.
4.  If the token contains `exp`, `nbf`, or `iat` claims, its validity status and relevant time information will be shown.

### To Encode

1.  Select the "Encode JWT" tab.
2.  Modify the header and payload as needed.
3.  Choose an algorithm (HS256, HS384, HS512).
4.  Enter your secret key.
5.  Click "Generate JWT Token".
6.  The generated token will appear below.
7.  Click the "Copy JWT Token" button to copy it to your clipboard.

## Technologies Used

-   HTML5
-   CSS3 (with Flexbox and Grid for layout)
-   Vanilla JavaScript
-   Web Crypto API for cryptographic operations (HMAC signing).
