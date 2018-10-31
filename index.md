## 一般复指数序列
#Python 代码：

```markdown
import numpy as np
import matplotlib.pyplot as plt

plt.rcParams['font.sans-serif']=['SimHei']
plt.rcParams['axes.unicode_minus']=False

x = np.linspace(0,5,50)
aa = 0+3j
bb = 0+x*2j
y = (np.e**aa)*(np.e**bb)*1*2**x
plt.subplot(1,2,1)
plt.title(r'$x_1[n]=|c||a|^n e^(j(ωn+θ)),ω=2,θ=3,|c|=1,|a|=2$')
plt.stem(x,y)
plt.xticks([])
plt.yticks([])


x = np.linspace(0,5,50)
cc =0+3j
dd =0+x*2j
y = (np.e**cc)*(np.e**dd)*1*(1/2)**x
plt.subplot(1,2,2)
plt.title(r'$x_2[n]=|c||a|^n e^(j(ωn+θ)),ω=2,θ=3,|c|=1,|a|=0.5$')
plt.stem(x,y)
plt.xticks([])
plt.yticks([])

plt.show()
```

#运行结果
![](http://m.qpic.cn/psb?/V105YmJH2gZua8/NVf39p8wG*7acJdpDfVDN5bdoh56QybwpmvTcrZV*5w!/b/dDQBAAAAAAAA&bo=gAfXAwAAAAADF2E!&rf=viewer_4)