# Node Ecosystem, TDD, CI/CD

---

## Array.map()

-  Allows you to iterate over an array and modify its elements using a callback function. The callback function will then be executed on each of the array's elements.

---

## Array.reduce()

- Allows you to iterate over an array with two arguments (previousValue, currentValue) and the final result will be a single value which means it will return a one value after the proccessing.

**example**

        const array1 = [1, 2, 3, 4];
        const reducer = (previousValue, currentValue) => previousValue + currentValue;

        // 1 + 2 + 3 + 4
        console.log(array1.reduce(reducer));
        // expected output: 10

        // 5 + 1 + 2 + 3 + 4
        console.log(array1.reduce(reducer, 5));
        // expected output: 15


---

## superagent()

**With normal Promise .then() syntax**

        superagent.get("https://swapi.dev/api/people/").then(data => {
            console.log(data.body);
        }).catch(err => {
            console.log(err);
        });


**With async / await syntax**

    let fetchData = async () => {
        try {
        let starWarsData = await superagent.get("https://swapi.dev/api/people/");

        await  console.log(starWarsData.body);
        } catch(err) {
            console.log(err);
        }
    };



---

## Promises

- Promises are used to handle asynchronous operations in JavaScript. They are easy to manage when dealing with multiple asynchronous operations where callbacks can create callback hell leading to unmanageable code.

**Benefits of Promises**

1. Improves Code Readability

2. Better handling of asynchronous operations

3. Better flow of control definition in asynchronous logic

4. Better Error Handling


**A Promise has four states**

1. fulfilled: Action related to the promise succeeded

2. rejected: Action related to the promise failed

3. pending: Promise is still pending i.e not fulfilled or rejected yet

4. settled: Promise has fulfilled or rejected


**Parameters**

1. Promise constructor takes only one argument,a callback function.

2. Callback function takes two arguments, resolve and reject

3. Perform operations inside the callback function and if everything went well then call resolve.

4. If desired operations do not go well then call reject.

![promise](https://www.freecodecamp.org/news/content/images/2020/06/Ekran-Resmi-2020-06-06-12.21.27.png)


--- 

**Are all callback functions considered to be Asynchronous? Why or Why Not?**

- A callback can be used synchronously or asynchronously. There's a difference in the order in which things happen in the timeline, depending on whether the callback is used synchronously or asynchronously.

![async](https://res.cloudinary.com/practicaldev/image/fetch/s--5e204O-Y--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/rjqf7w2vmlxxz5ez0dbz.png)

![sync](https://res.cloudinary.com/practicaldev/image/fetch/s--dqZaqp09--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/hyaxexxqnkl9ymxrjlh4.png)