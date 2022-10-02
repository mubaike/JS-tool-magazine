```
/**
 * 
 * @param {Array} arr 
 * @param {Function} callback 
 * @returns 
 */
function filter(arr, callback){
    //声明空数组
    let result = [];
    //遍历数组
    for (let i = 0; i < arr.length; i++) {
        //执行回调
        let res = callback(arr[i], i);
        //判断 如果为真则压入到 result 结果
        if(res) {
            result.push(arr[i]);
        }
    }
    //返回结果
    return result;
}
```
