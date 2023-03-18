import cv2
# Load the cascade
eye_cascade = cv2.CascadeClassifier(cv2.data.haarcascades+'haarcascade_eye.xml')
# Read the input image
path = r"C:\Users\sophy\Pictures\Camera Roll\eyes.jpg"
img = cv2.imread(path)
# Convert into grayscale
gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
# Detect eyes
eyes = eye_cascade.detectMultiScale(img, scaleFactor = 1.2, minNeighbors = 4)
print ("Found {0} Eyes!".format(len(eyes)))
# Draw rectangle around the faces
for (x,y,w,h) in eyes:
            cv2.rectangle(img,(x,y),(x+w,y+h),(0, 255, 0),3)
    # Display the output
cv2.imshow("Eyes Detected", img)
cv2.waitKey(0)