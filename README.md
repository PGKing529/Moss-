# Moss 使用模板 python 简化版本
## Moss使用模板
## 使用前 pip install mosspy
## addbase 添加base文件 addfile增加要比的东西

import mosspy

userid = 241958773 

m = mosspy.Moss(userid, "python")

m.addBaseFile("example.py")


m.addFile("1.py")
m.addFile("2.py")


url = m.send(lambda file_path, display_name: print('*', end='', flush=True))
print()

print ("Report Url: " + url)
