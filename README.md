# shyonvif
Yet another python onvif lib

# Dependencies

requests, base64, http.client

# How to use:

1. Copy **lib** directory in you project (you can rename this dir).
2. Import:
```
import lib.shyonvif as shyonvif
```
**Warning!** if you rename lib dir, import like this:
```
import %folder_name%.shyonvif as shyonvif
```
3. Initialize the camera:
```
mycam = shyonvif.onvif(addr="192.168.1.13", port="80", usr='admin', pwd="12345", debug=True, basicauth=False)
```
4. Submit a request to onvif server on the camera:


**Ex:** ```mycam.execute("GET_NETWORK")```

**Additions:**

Change ip: 
```
print(mycam.setIP("192.168.1.12"))
```
5. Dont forget close session:
```
mycam.close()
```
