# Subplot Explained

```python
import matplotlib.pyplot as plt 
plt.subplot(1,2,1)
plt.imshow(data)
plt.subplot(1,2,2)
plt.plot(X,Y)
```

#### The meaning of (121) or (1,2,2) is that
- 111 is a shorthand for 1,1,1
- First param is the number of rows (how many rows are there in the image)
- Second param is the number of columns
- The last number is the image id in the grid starting top left = 1 and go all the way to bottom right = n
