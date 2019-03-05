# Data_Augmentation
In this project data augmentation technique has been demonstrated using ImageDataGenerator tool from keras.preprocessing tool. Keras ImageDataGenerator tool takes images as input and generate set number of images in a given directory. It Generate batches of tensor image data with real-time data augmentation. The data will be looped over (in batches).

## Steps
- Set data_path: Url for all class folders. Class folder name is the name of that class

- Read image and labels: Read class names and number of classes. Read all images and put them in a nd-array. In image_read function all images have been normalized between -1 and 1, nulls are removed. All images have been rolled into 1 row. Nd-array shape will be [1, #images, imageWidth, imageLength, channels] 

- Data augmentation: Data augmentation was done using keras preprocessing tools. Random rotation, random zoom and random width shift operations were performed to augment data. After running augmentation operation all were read and appended in an nd-array.
More details are available at https://keras.io/preprocessing/image/

## Use your won data_path and test_path. My paths are as below. 
data_path = r'C:\Users\aman0\Desktop\ME\My_project\Data Sink\GIW'
test_path = r'C:\Users\aman0\Desktop\ME\Tutorial\Data Sink\TransferF_course\validation_data\test.jpg'
