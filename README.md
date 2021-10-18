
## lab note 🧪 

The **Lab** is a very powerful feature 🔥that allows you to run JavaScript code directly in the preview.
You can use the **Node fs API** as well as the pre-included libraries to **explore and visualize your data**. ✨

**Disclaimer**: Like any coding platform, keep in mind that you are running code on your machine with full access to your computer!


## Examples 

Use the `print()` function to display your result.
```js
const array1 = [1, 4, 9, 16];
const map1 = array1.map(x => x * 2)
print(map1)
    `````

    Open a local file with Node fs: `_fs`
    ```js
    const data = _fs.readFileSync('/tmp/finance-charts-apple.csv', 'utf8');
    print(data);
    `````

    Data exploration with [DanfoJs](https://danfo.jsdata.org/)
    ```js
    const df = await dfd.read_csv("https://raw.githubusercontent.com/plotly/datasets/master/finance-charts-apple.csv");
    print(df.describe())
    `````

    Plot example
    ```js
    const df = await dfd.read_csv("https://raw.githubusercontent.com/plotly/datasets/master/finance-charts-apple.csv");
    const new_df = df.set_index({ key: "Date"  });
    new_df.plot(el).line({ columns: ["AAPL.Open", "AAPL.High"]  });
    `````


    Only JS code is runnable (Java below)

    ``` java
    public class MyClass {
        private static String myVar = "";
        public MyClass () {
                super();
                    
        } 
        
    }
`````

## Diagram

Make diagrams thanks to [mermaid](https://mermaid-js.github.io/)

```mermaid
sequenceDiagram
Alice->>John: Hello John, how are you?
loop Healthcheck
    John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts!
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
    `````````
````
    ````
    ````
    ````
    ````
