# Visualization
可视化课程所用代码

## Week3 Direct PCA, SVD, Dual PCA

  ### numpy
  
  print(a[::-1]) :取从后向前（相反）的元素
  [ 5 4 3 2 1 ]
  
  [0:p] ：取从第0个到p-1个
  [:,0] ：取所有集合第0个元素
  [1,:] ：取第个集合全部的元素
  
  np.linalg.eig():算全部的eginvalue和eginvecter
  np.argsort:将x中的元素从小到大排列，提取其对应的index(索引)，然后输出到y
  np.diag: creates a diagonal matrix that take a vector as input

## Week4 Kernel PCA

  ### matplotlib.pyplot
  pyplot的方式中plt.subplot()参数和面向对象中的add_subplot()参数和含义都相同
  .add_subplot(111) :表示“1x1网格，第一个子图”

  matplotlib.pyplot.scatter(x, y, s=None, c=None, marker=None, cmap=None, norm=None, vmin=None,       vmax=None, alpha=None, linewidths=None, verts=None, edgecolors=None, *, data=None, **kwargs)

  x，y：表示的是大小为(n,)的数组，也就是我们即将绘制散点图的数据点
  s:是一个实数或者是一个数组大小为(n,)，这个是一个可选的参数。
  c:表示的是颜色，也是一个可选项。默认是蓝色'b',表示的是标记的颜色，或者可以是一个表示颜色的字符，或者是一个长度  为n的表示颜色的序列等等，感觉还没用到过现在不解释了。但是c不可以是一个单独的RGB数字，也不可以是一个RGBA的序列。可以是他们的2维数组（只有一行）。
  marker:表示的是标记的样式，默认的是'o'。
  cmap:Colormap实体或者是一个colormap的名字，cmap仅仅当c是一个浮点数数组的时候才使用。如果没有申明就是   image.cmap
  norm:Normalize实体来将数据亮度转化到0-1之间，也是只有c是一个浮点数的数组的时候才使用。如果没有申明，就是默认为   colors.Normalize。
  vmin,vmax:实数，当norm存在的时候忽略。用来进行亮度数据的归一化。
  alpha：实数，0-1之间。
  linewidths:也就是标记点的长度。
  
  plt.title: a function to name your figure.
  plt.figure: a function to create a figure.
  
  ### numpy
  numpy.zeros(shape, dtype=float, order='C', *, like=None)
  >>> np.zeros(5)
  array([ 0.,  0.,  0.,  0.,  0.])
  
  np.ones: creates a matrix full of ones
  >>> np.ones((2, 1))
  array([[ 1.],
       [ 1.]])
  
  np.shape
  shape函数是numpy.core.fromnumeric中的函数，它的功能是读取矩阵的长度，比如shape[0]就是读取矩阵第一维度的长  度。shape的输入参数可以是一个整数（表示维度），也可以是一个矩阵。直接.shape返回矩阵形状。
  
  np. exp(x)   e的x幂次方
  
  np.identity: creates a identity matrix
  np.identity(3),要求n=m
  
  np.dot: does matrix multiplication
  np.dot(H,K)
  
  np.float32

