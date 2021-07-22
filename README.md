# Moss-
Moss使用模板

import mosspy

userid = 241958773 # 我的id

m = mosspy.Moss(userid, "python")

m.addBaseFile("example.py")
# m.addBaseFile("submission/test_student.py")

# Submission Files
m.addFile("1.py")
m.addFile("2.py")

# progress function optional, run on every file uploaded
# result is submission URL
url = m.send(lambda file_path, display_name: print('*', end='', flush=True))
print()

print ("Report Url: " + url)

# # Save report file
# m.saveWebPage(url, "submission/report.html")

# # Download whole report locally including code diff links
# mosspy.download_report(url, "submission/report/", connections=8, log_level=10, on_read=lambda url: print('*', end='', flush=True)) 
# # log_level=logging.DEBUG (20 to disable)
# # on_read function run for every downloaded file
