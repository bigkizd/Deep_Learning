# Deep Belief Networks
[Hinton06] cho thấy RBMs có thể xếp chồng lên nhau và được đào tạo một cách tham lam để tạo thành cái gọi là Deep Belief Networks(DBN). DBNs là graphical models học cách trích xuất một đại diện phân cấp sâu của training data. They model phân bố chung giữa observed vector x and the l hidden layers h^k như sau:</br>
![](https://latex.codecogs.com/gif.latex?P%28x%2C%20h%5E1%2C%20%5Cldots%2C%20h%5E%7B%5Cell%7D%29%20%3D%20%5Cleft%28%5Cprod_%7Bk%3D0%7D%5E%7B%5Cell-2%7D%20P%28h%5Ek%7Ch%5E%7Bk&plus;1%7D%29%5Cright%29%20P%28h%5E%7B%5Cell-1%7D%2Ch%5E%7B%5Cell%7D%29)
</br>
where ![](https://latex.codecogs.com/gif.latex?x%3Dh%5E0%2C%20P%28h%5E%7Bk-1%7D%20%7C%20h%5Ek%29) là phân phối có điều kiện chó các đợi vị hiển thị được điều chỉnh trên hidden units của RBM tại level k, and ![](https://latex.codecogs.com/gif.latex?P%28h%5E%7B%5Cell-1%7D%2C%20h%5E%7B%5Cell%7D%29) là phân phối chung có thể nhìn thấy được ẩn trong top-level RBM. Điều này được minh họa trong hình bên dưới.</br>