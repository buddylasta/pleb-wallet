### APIs
- npm install axios
- import axios from 'axios'
ex:
  const getPrice = () => {
    axios
      .get("https://api.coinbase.com/v2/prices/BTC-USD/spot")
      // .then is a promise that will run when the API call is successful
      .then((res) => {
        setPrice(res.data.amount);
      })
      // .catch is a promise that will run if the API call fails
      .catch((err) => {
        console.log(err);
      });
  };

### Packages for bitcoin dev
- qrcode.react


### Extra
- callback functions = need to pass in a function to get things to execute