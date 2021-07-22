# Moss 使用模板 python 简化版本
Moss使用模板

import mosspy

userid = 241958773 //我的id

m = mosspy.Moss(userid, "python")

m.addBaseFile("example.py")


//Submission Files
m.addFile("1.py")
m.addFile("2.py")


url = m.send(lambda file_path, display_name: print('*', end='', flush=True))
print()

print ("Report Url: " + url)
