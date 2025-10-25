# Task-by-24.10.25
Task 01



#✅ Task-1: Organize files by extension in a folder using "os"



import os

folder_path = r"C:\Users\bheem\.android"  
for doremon in os.listdir(folder_path):
    file_path = os.path.join(folder_path, doremon)

    if os.path.isfile(file_path):

        name, extension = os.path.splitext(doremon)

        extension = extension[1:]  

        if extension == '':
            continue

        new_folder = os.path.join(folder_path, extension)
        if not os.path.exists(new_folder):
            os.mkdir(new_folder)

        new_path = os.path.join(new_folder, doremon)
        os.rename(file_path, new_path)




#=======================================================================


**Task 2**

