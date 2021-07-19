# pyqt5_make_exe
pyqt5编译exe  
###安装pyinstaller  
pip installer pyinstaller  
### 直接编译  
pyinstaller -F -w main.py  
### 编译依赖文件  
#### 1. pyi-makespec main.py 生成main.spec  
#### 2. 编辑main.spec  
a = Analysis(['main.py','所有.py文件'],  
    datas = [('需要导入的外部文件1'，'.'),('需要导入的外部文件2'，'.')],  
        .....)  
