# js-console
Collection of frequently used commands   
   
   
### 강의 제목에 있는 시간(ex. "(2:30)")의 합 구하는 코드   
Code for calculating the sum of the time(ex. "(2:30)") in the lecture title   

```
let query = "div > span.lecture-name";
let time = 0; document.querySelectorAll(query).forEach((v)=>{
    let k = (v.innerText.match(/\(\d{1,2}:\d{1,2}\)/g));
    if(k) k.forEach((v)=>{let i = v.indexOf(":"); time+=60*(+v.slice(1,i)); time+=+v.slice(i+1,v.length-1);})
})
console.log(time)
```
