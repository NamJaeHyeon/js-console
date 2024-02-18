# js-console
Collection of frequently used commands

"""
let query = "div > span.lecture-name";
let time = 0; document.querySelectorAll(query).forEach((v)=>{
    let k = (v.innerText.match(/\(\d{1,2}:\d{1,2}\)/g));
    if(k) k.forEach((v)=>{let i = v.indexOf(":"); time+=60*(+v.slice(1,i)); time+=+v.slice(i+1,v.length-1); console.log((v.slice(1,i)), v.slice(i+1,v.length-1))})
})
console.log(time)
"""
