# base64helper
**VFP library to encode/decode strings &amp; files using Base64 format**


----

### Usage

    DO base64Helper   && This will create a global object called B64
    
    cEncoded = B64.encodeString("This is a test")
    ?cEncoded -> VGhpcyBpcyBhIHRlc3Q=

    ?B64.decodeString("SGVsbG8gd29ybGQh") --> "Hello world!"
    
    cEncoded = B64.encodeFile("c:\folder\myfile.bmp")
    B64.decodeFile("c:\folder\mycopy.bmp", cEncoded)
    
    cWebEncodedFile = B64.encodeFile("c:\folder\mydocument.pdf", .T.)  && This will return a web-compatible Base64 string.
    

