# Axios-Doc
## Basic Information About Axios
```
- Axios is a JS library . 
- It helps to make requst from browser (Plain Js / react // Angular), node.js
- Very Easy to use
- It supports all modern browser and old browser because axios made based on XMl HTTP request and more   update than that .
- Its return promise
- Throw error Brilliantly
- No need to set header cause axios is intelligent

```
## Basic method of Axios
```
 axios(config)
- axios(url [, config])
- axios.get(url [, config])
- axios.post(url [, config])
- axios.put(url [, config])
- axios.patch(url [, config])
- axios.delete(url [, config])
- axios returns response object - data, status, statusText, headers, config
```
# Thats All About Theory , Now we will use all theory practically .

## Using .get method. 
### we will use .get method for get the data from data_base . Now we will use it practically.
```
axios.get(' api's in here ')
.then((res) => console.log(res.data))
.catch((error)=> console.log(error))

```
