### Set up Github
- Step 0
```sh
ssh-keygen -t rsa -b 4096 -C "<github 注册邮箱>" && cat ~/.ssh/id_rsa.pub.pub
```
- Step 1
<div style="text-align:center; margin:auto"><img src="img/2020-01-14-01-18-35.png"></div>

- Step 2
<div style="text-align:center; margin:auto"><img src="img/2020-01-14-01-19-34.png"></div>

- Step 3
<div style="text-align:center; margin:auto"><img src="img/2020-01-14-01-22-17.png"></div>

### Generate Package

- Open terminal
<div style="text-align:center; margin:auto"><img src="img/2020-01-14-00-57-48.png"></div>

- Create & Enter Project Folder
```sh
mkdir yuzhuhwq5
cd yuzhuhwq5
```
<div style="text-align:center; margin:auto"><img src="img/2020-01-14-00-59-30.png"></div>

- Create and Enter Package Folder
```sh
mkdir yuzhuhwq5public
cd yuzhuhwq5public
```
<div style="text-align:center; margin:auto"><img src="img/2020-01-14-01-01-31.png"></div>

- Create core files
```sh
touch __init__.py bubbler.py
echo 'name="yuzhuwanghwq5bubbler"' >> yuzhuhwq5public/__init__.py
```
<div style="text-align:center; margin:auto"><img src="img/2020-01-14-01-05-55.png"></div>

- Edit bubbler.py
```py
def bubbleSort(arr):
    n = len(arr)
 
    # 遍历所有数组元素
    for i in range(n):
 
        # Last i elements are already in place
        for j in range(0, n-i-1):
 
            if arr[j] > arr[j+1] :
                arr[j], arr[j+1] = arr[j+1], arr[j]
 
# #testing
# arr = [31, 2, 11, 23, 8, 7, 11,14,20]
 
# bubbleSort(arr)
 
# print ("sorted:")
# for i in range(len(arr)):
#     print ("%d" %arr[i]),
```
- Create `License` and `README.md`
- LICENSE
```license
MIT License

Copyright (c) 2020 Yuzhu Wang

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
- `README.MD`
```md
## Demo_car
This is a sample package to learn the steps of creating and publishing package.
```




### Publish


### References
- [How to Create and Publish Python Package.](https://dev.to/umeshdhakar/how-to-create-and-publish-python-package-62o)