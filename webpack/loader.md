#### 什么是loader

```
对模块的源代码进行转换,对文件进行预处理
使用方法：
1.webpack 配置, 执行顺序 【从右往左】
	module:{
		rules: {
			test: '/\.css$/',
			use: [
			    { loader: 'style-loader' },
          {
            loader: 'css-loader',
            options: {
              modules: true
            }
          },
          { loader: 'sass-loader' }
			]
		}
	}
2.内联
import Styles from 'style-loader!css-loader?modules!./styles.css';
3.

```

