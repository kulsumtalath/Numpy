```python
import numpy as np         
```


```python
data1=[[1,2,3],[4,5,6]]
```


```python
arr1=np.array(data1)
```


```python
arr1

```




    array([[1, 2, 3],
           [4, 5, 6]])




```python
data1.__class__
```




    list




```python
arr1.__class__
```




    numpy.ndarray




```python
arr1.ndim
```




    2




```python
arr1.shape
```




    (2, 3)




```python
#dtype the array holds
arr1.dtype
```




    dtype('int32')




```python
np.zeros((3,6))
```




    array([[0., 0., 0., 0., 0., 0.],
           [0., 0., 0., 0., 0., 0.],
           [0., 0., 0., 0., 0., 0.]])




```python
arr=np.arange(15).reshape(3,5)
```


```python
arr
```




    array([[ 0,  1,  2,  3,  4],
           [ 5,  6,  7,  8,  9],
           [10, 11, 12, 13, 14]])




```python
arr[2]
```




    array([10, 11, 12, 13, 14])




```python
arr.shape
```




    (3, 5)




```python
arr[2:3]
```




    array([[10, 11, 12, 13, 14]])




```python
arr[1:2]
```




    array([[5, 6, 7, 8, 9]])




```python
arr[1:4]
```




    array([[ 5,  6,  7,  8,  9],
           [10, 11, 12, 13, 14]])




```python
arr[0,0]
```




    0




```python
arr[2,]
```




    array([10, 11, 12, 13, 14])




```python
arr[2,3]
```




    13




```python
arr2d=np.array(([1,2,3],[4,5,6],[7,8,9]))
```


```python
arr2d

```




    array([[1, 2, 3],
           [4, 5, 6],
           [7, 8, 9]])




```python
arr2d.ndim
```




    2




```python
arr2d[0][2]
```




    3




```python
arr2d[:2]
```




    array([[1, 2, 3],
           [4, 5, 6]])




```python
arr2d[2:]
```




    array([[7, 8, 9]])




```python
arr2d[:,0:2]
```




    array([[1, 2],
           [4, 5],
           [7, 8]])




```python
arr2d[:,0]
```




    array([1, 4, 7])




```python
arr2d[0:2,:]
```




    array([[1, 2, 3],
           [4, 5, 6]])




```python
arr3=np.arange(9).reshape((3,3))
```


```python
arr3
```




    array([[0, 1, 2],
           [3, 4, 5],
           [6, 7, 8]])




```python
#arr3.T
```


```python
arr=np.random.randn(3,3)
```


```python
arr
```




    array([[ 2.08674009,  0.68056015,  0.11646808],
           [-1.13183364, -0.06870206,  1.67462105],
           [ 0.0727677 , -0.18658683,  0.80757936]])




```python
np.dot(arr3,arr)
```




    array([[-0.98629824, -0.44187572,  3.28977978],
           [ 2.09672419,  0.83393808, 11.08578528],
           [ 5.17974663,  2.10975188, 18.88179078]])




```python
arr=np.arange(10)
```


```python
np.sqrt(arr)
```




    array([0.        , 1.        , 1.41421356, 1.73205081, 2.        ,
           2.23606798, 2.44948974, 2.64575131, 2.82842712, 3.        ])




```python
np.square(arr)
```




    array([ 0,  1,  4,  9, 16, 25, 36, 49, 64, 81], dtype=int32)




```python
np.exp(arr)
```




    array([1.00000000e+00, 2.71828183e+00, 7.38905610e+00, 2.00855369e+01,
           5.45981500e+01, 1.48413159e+02, 4.03428793e+02, 1.09663316e+03,
           2.98095799e+03, 8.10308393e+03])




```python
np.ceil(arr)
```




    array([0., 1., 2., 3., 4., 5., 6., 7., 8., 9.])




```python
np.floor(arr)
```




    array([0., 1., 2., 3., 4., 5., 6., 7., 8., 9.])




```python
np.sign(arr)
```




    array([0, 1, 1, 1, 1, 1, 1, 1, 1, 1])




```python
np.log(arr)
```

    <ipython-input-63-a67b4ae04e95>:1: RuntimeWarning: divide by zero encountered in log
      np.log(arr)
    




    array([      -inf, 0.        , 0.69314718, 1.09861229, 1.38629436,
           1.60943791, 1.79175947, 1.94591015, 2.07944154, 2.19722458])




```python
np.log10(arr)
```

    <ipython-input-64-4473232fb1a0>:1: RuntimeWarning: divide by zero encountered in log10
      np.log10(arr)
    




    array([      -inf, 0.        , 0.30103   , 0.47712125, 0.60205999,
           0.69897   , 0.77815125, 0.84509804, 0.90308999, 0.95424251])




```python
np.log2(arr)
```

    <ipython-input-66-45ec4562025d>:1: RuntimeWarning: divide by zero encountered in log2
      np.log2(arr)
    




    array([      -inf, 0.        , 1.        , 1.5849625 , 2.        ,
           2.32192809, 2.5849625 , 2.80735492, 3.        , 3.169925  ])




```python
np.rint(arr)
```




    array([0., 1., 2., 3., 4., 5., 6., 7., 8., 9.])




```python
np.modf(arr)
```




    (array([0., 0., 0., 0., 0., 0., 0., 0., 0., 0.]),
     array([0., 1., 2., 3., 4., 5., 6., 7., 8., 9.]))




```python
np.isnan(arr)
```




    array([False, False, False, False, False, False, False, False, False,
           False])




```python
np.cos(arr)
```




    array([ 1.        ,  0.54030231, -0.41614684, -0.9899925 , -0.65364362,
            0.28366219,  0.96017029,  0.75390225, -0.14550003, -0.91113026])




```python
x1=[4,2,3]
x2=[1,1,2]
```


```python
np.greater_equal(x1,x2)
```




    array([ True,  True,  True])




```python
arr=np.array(([1,2,3],[4,5,6]))
```


```python
arr.mean()
```




    3.5



arr


```python
arr.sum()
```




    21




```python
x=np.random.random(10)
y=np.random.random(10)
z=np.random.random(10)
z

```




    array([0.36036396, 0.88835314, 0.85950039, 0.35043734, 0.80406475,
           0.69997891, 0.6210788 , 0.35277136, 0.81707636, 0.68896842])




```python
x
```




    array([0.76736142, 0.3820155 , 0.81825131, 0.3980884 , 0.16679601,
           0.13916988, 0.42334946, 0.92103214, 0.43555582, 0.26756916])




```python
y
```




    array([0.5907024 , 0.25752439, 0.98005795, 0.79528245, 0.86090427,
           0.94706593, 0.31737931, 0.14584475, 0.62023667, 0.96521039])




```python
data=np.array(zip(x,y,z))
```


```python
data
```




    array(<zip object at 0x00000166377B2C00>, dtype=object)




```python
a=np.array(([1,2,3],[2,3,4]))
```


```python
a
```




    array([[1, 2, 3],
           [2, 3, 4]])




```python
z=np.zeros([2,1])
```


```python
z
```




    array([[0.],
           [0.]])




```python
np.append(a,z,axis=1)
```




    array([[1., 2., 3., 0.],
           [2., 3., 4., 0.]])




```python
a=np.array(([1,2,3],[2,3,4]))
```


```python
z=np.zeros([2,2])
```


```python
np.append(a,z,axis=1)
```




    array([[1., 2., 3., 0., 0.],
           [2., 3., 4., 0., 0.]])




```python
z=np.zeros([2,3])
```


```python
np.append(a,z,axis=0)
```




    array([[1., 2., 3.],
           [2., 3., 4.],
           [0., 0., 0.],
           [0., 0., 0.]])




```python
data=np.array(([123,234,564],[345,876,980],[345,678,986],[342,675,897],[987,657,453],[564,765,654]))
```


```python
data
```




    array([[123, 234, 564],
           [345, 876, 980],
           [345, 678, 986],
           [342, 675, 897],
           [987, 657, 453],
           [564, 765, 654]])




```python
subset=data[data[:0]==912]
subset
```




    array([], dtype=int32)




```python
data
```




    array([[123, 234, 564],
           [345, 876, 980],
           [345, 678, 986],
           [342, 675, 897],
           [987, 657, 453],
           [564, 765, 654]])




```python
arr=np.random.random((4,5))
```


```python
arr
```




    array([[0.19435898, 0.97056277, 0.32998517, 0.15934107, 0.1749251 ],
           [0.361749  , 0.81627145, 0.69811987, 0.1682191 , 0.79601608],
           [0.60456278, 0.94101255, 0.39200636, 0.43006296, 0.86919177],
           [0.32538027, 0.00771593, 0.25879117, 0.1830865 , 0.38207057]])




```python
np.concatenate([arr,arr],axis=0)
```




    array([[0.19435898, 0.97056277, 0.32998517, 0.15934107, 0.1749251 ],
           [0.361749  , 0.81627145, 0.69811987, 0.1682191 , 0.79601608],
           [0.60456278, 0.94101255, 0.39200636, 0.43006296, 0.86919177],
           [0.32538027, 0.00771593, 0.25879117, 0.1830865 , 0.38207057],
           [0.19435898, 0.97056277, 0.32998517, 0.15934107, 0.1749251 ],
           [0.361749  , 0.81627145, 0.69811987, 0.1682191 , 0.79601608],
           [0.60456278, 0.94101255, 0.39200636, 0.43006296, 0.86919177],
           [0.32538027, 0.00771593, 0.25879117, 0.1830865 , 0.38207057]])




```python

```
