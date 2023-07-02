<!--
 * @Author: HU Zheng
 * @Date: 2023-01-15 13:51:47
 * @LastEditors: HU Zheng
 * @LastEditTime: 2023-01-15 13:53:55
 * @Description: file content
-->

# 最优化PJ

姜国超 22210980043

李保山 22210980010

## 数据准备

在datasets文件夹下下载两个数据集：[covtype](https://drive.google.com/file/d/1lPl1XVZjW5r_aD5i_a_gZtzx24xMscZZ/view?usp=sharing)和[gisette](https://drive.google.com/file/d/1Lhw6rpcZk1Mn2aEgY3Jr_OdcOMtVTOfB/view?usp=sharing)

## 代码使用示例

非随机方法实验：

```shell
python runall_non_stoch.py --data_path datasets/w8a --save_path D_100_w8a.json --diameter 100 --lamda 100 --rm_zeros 0
```

随机试验：

```shell
python run_stoch.py --data_path datasets/covtype.libsvm.binary.scale --save_path cov_D_500.json --diameter 500 --lamda 100 --rm_zeros 0
```

gisette实验：

```shell
python runipm.py --data_path datasets/gisette_scale.t --save_path D_10_gissette.json --diameter 10 --lamda 100 --rm_zeros 0
```

w8a.t实验：

```shell
python runctr_ipm.py --data_path datasets/w8a.t --save_path D_100_w8at.json --diameter 100 --lamda 100 --rm_zeros 0
```

其他参数请参照代码。
