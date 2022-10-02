```
function slice(arr, begin, end){
    //若 arr 数组长度为 0
    if(arr.length === 0) {
        return [];
    } 

    //判断 begin 
    begin = begin || 0;
    if(begin >= arr.length){
        return [];
    }

    //判断 end
    end = end || arr.length;
    if(end < begin) {
        end = arr.length;
    }
    //声明一个空数组
    const result = [];

    //遍历对象
    for(let i=0;i<arr.length;i++){
        if(i >= begin && i < end) {
            result.push(arr[i]);
        }
    }
    return result;
}
```
