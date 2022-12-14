## Adel Gataullin




tg: [@what_you_see](https://t.me/what_you_see)


***

``` 
    for (let i = 7; i < paperValuesPayLr; i++){
      let paperPayNum = paper.getRange(i, 14, 1, 2).getValue();
      paperPayNum = (typeof(paperPayNum) === "string") ?  paperPayNum.substr(5) : paperPayNum;
      paperValuesPay[paperPayNum] = {
        money: 0,
        payMethod : "",
        typeMethod : "",
      }
    }
``` 


```
  for (key in reportValues){
    if (reportValues[key].money > 0 && reportValues[key].payMethod === "CARD"){
      card += reportValues[key].money
      cardCounter += 1
    } else if (reportValues[key].money > 0 && reportValues[key].payMethod === "CASH") {
      cash += reportValues[key].money
    }
  }
``` 