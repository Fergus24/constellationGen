from PIL import Image
import random

largeStar = Image.open('largeStar.png')
smallStar = Image.open('smallStar.png')
blankImage = Image.open('blank.png')
circleImage = Image.open('Circle only-01.png')


i = 200
theNumber = 0

while i < 300:

  starCopyIm = blankImage.copy()


  starCopyIm.paste(circleImage, (0,0))


  for left in range(500, 2000, 100):
    for top in range(1000, 2500, 100):
     
      theNumber = random.randint(1,101)
      if theNumber > 85:
        if (top-1700)**2 + (left-1200)**2 <= 630**2:
          starCopyIm.paste(largeStar, (left, top))
      elif theNumber < 12:
        if (top-1700)**2 + (left-1200)**2 <= 630**2:
          starCopyIm.paste(smallStar, (left, top))

  starCopyIm.save('Stars Folder/stars{0}.png'.format(i + 1))
  i = i + 1


#0 to 5300 and 0 to 5200

"""
import os

counter = 100

while counter < 200: 


  os.remove('stars{}.png'.format(counter + 1))
  counter = counter + 1
"""
