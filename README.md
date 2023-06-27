# picture-vector

pixels to vector

from picturevector import Picvector
import json

dict = {}

tvi = Picvector("image0.jpeg")
t = tvi.vectorpixels()

dict["0"] = t

with open("bitmaps.json", "a") as file:
    json.dump(dict, file)
    print("save!")
