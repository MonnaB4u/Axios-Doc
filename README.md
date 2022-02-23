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
 Thats All About Theory , Now we will use all theory practically .
 
## Using .get method. 
 we will use .get method for get the data from data_base . Now we will use it practically.
```
axios.get('/api/')
.then((res) => console.log(res.data))
.catch((error)=> console.log(error))

```
## Using .post Method
.post method used for if wanna send data in the database . 
```
axios.post('/api/',{
    method: 'POST',
    body:json.stringify(
        {
            id: '101',
            name:"Moheuddin Monna",
            age:"24",

        }
    )})
    .then(res=>console.log(res))
    .catch(err=>console.log(err))
```

## .put & .pathc Method
 .put & .pathc method both use for update data . 
 
 ```
 Example if put method
 
 axios.put('/api/',{
    method: 'POST',
    body:json.stringify(
        {
            id: '102',
            name:"Moheuddin Monna & Monna",
            age:"24 && 24",

        }
    )})
    .then(res=>console.log(res))
    .catch(err=>console.log(err))
 ```
```
 Example if put method
 axios.patch('/api/',{
    method: 'PATCH',
    body:json.stringify(
        {
            id: '102',
            name:"Moheuddin Monna & Monna",
            age:"24 && 24",

        }
    )})
    .then(res=>console.log(res))
    .catch(err=>console.log(err))
```

## .delete Method 
.delete method use for Delete data
```
axios.delete('/api/')
    .then(res => console.log(res))
    .catch(err => console.log(err))
```

# Applying Method using async & await

```
let makeRequest = async (config) => {
    return await axios(config)
}

const createData = () => {
    makeRequest({
        url: "https://jsonplaceholder.typicode.com/posts",
        method: "post",
        data: JSON.stringify({
            name: 'Monna',
            age: '24',
        }),
    })
        .then((res) => console.log(res))
        .catch((err) => console.log(err))
};
createData();


````


