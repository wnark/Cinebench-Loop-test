# 说明

用到了R23的参数执行方式，国人开发的pyecharts模块。
还没完全完成，因为R23的执行方式与R15完全一样，我暂时无法获取执行的结果。


# 部署
## need
├── Cinebench-R15-Loop-test-main.zip

├── Cinebench_R15_MAXON.zip

└── python-3.8.10-amd64.exe

## 安装环境
1.以管理员身份运行
2.勾选“Add Python 3.8 to PATH”
3.install now
4.Disable path length limit
5.修改dns添加GitHUB加速
6.`pip install pyecharts -U`

## 解压
解压到下载目录，减短长度链接。
Cinebench-R15-Loop-test-main.zip
Cinebench_R15_MAXON.zip

## 执行
将main.py文件移动到Cinebench_R15_MAXON文件夹，然后执行。

## 其他
使用的命令
g_CinebenchCpu1Test=true | 在 1 个 CPU 上测试
g_CinebenchCpuXTest=true | 多核测试一次
g_CinebenchAllTests=true | 连续多次测试
g_CinebenchMinimumTestDuration=100 | 设置最大持续时间
g_acceptDisclaimer=true | 自动接受使用条款

我们很遗憾无法直接从中得出分数，也无法通过此方法指定要使用的线程数。推荐使用以下典型命令：

start /b / wait "parentconsole" Cinebench.exe g_CinebenchAllTests=true