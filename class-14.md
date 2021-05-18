## Local Storage
the Local Storage is an internal database created into the browser, which you can use to save data in a key-value format. Most popular and commonly used browser like Chrome, Firefox and Safari all support Local Storage. The data stored in local storage has no expiration data, so it will persist over closed browser window and session.

Local storage has a very simple set, retrieve and remove API, and the key-value pair is always of string type.

![image](https://developer-chrome-com.imgix.net/image/admin/sZ8JCGib96F45euuc4pi.png?auto=format)
## Local storage methods
* You can set data in local storage programatically by using the localStorage.setItem(key, value).
* The syntax for retrieving data is localStorage.getItem(key).
*To delete all data in the current web domain, use localStorage.clear().
![image](https://res.cloudinary.com/practicaldev/image/fetch/s--vYlmIKQX--/c_imagga_scale,f_auto,fl_progressive,h_500,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/2imjutnczd4f3jdhgbdx.png)
## Limitations of local storage
1. localStorage is not a safe database, and you should never use it for storing sensitive data.
2. It’s max storage size 5 MB. Never store large amount of data in it.
3. It’s synchronous

