import os, sys
import glob

# if not in directory w/ images, set directory
# Dir = '/Users/nkrell/Desktop/Southern Africa Food Security Classification/ALL_HFIC/Southern Africa'
# os.chdir(aDir)

files = glob.glob('*.png')
files.sort()
file = open('files.txt', 'w')  # writes text file
for item in files:
    file.write("%s\n" % item)
file.close()

os.system('convert -delay 50 @files.txt animated.gif') # set image delay

# Borrowed code: https://stackoverflow.com/questions/38444619/how-to-create-gifs-with-images-in-python
