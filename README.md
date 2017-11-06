# EC601-OPEN_CV_HW

HAVE DONE ALL THE 4 EXERCISES AS PART OF HW
ALL THE THEORY QUESTIONS OF THE EXERCISES ARE WRITTEN IN THS FILE.

EXERCISE 1


CvMat is a data structure used to create a 2D array in OpenCV. 
Matrices are stored row by row where all rows have a 4 byte alignment.
To create a Matrix : CvMat* matrix1(int rows, int cols, int type, data)
Each element in the matrix is like a pixel.
OpenCV, treats matrices in ROW-major order. I.e. the access is defined as (ROW, column). 

Therefore if we need to access element (i,j) in the matrix then:

  	cv::Mat matrix1(2, 3, CV_32FC1, 0.0f);  //create a 2 row, 3 column matrix with all 0.0
	matrix1.at<float>(1,0) = 2; // accessing element (1,0) and assign it 2.
	cout << m << endl;

	
	This will print the following:
	
	[0, 0, 0;
	 2, 0, 0]	// indicates that the program accessed it with row major order.

	
	If it was accessed column first, it would print this,
	
	[0, 2;
	 0, 0;
	 0, 0]
   
  
  
EXERCISE 2 

The Python file(Color_Image.py) is located in the files above.

The range of pixel values are 0-255 in all the 3 colorspaces. 
   
   
  
  
EXERCISE 4

The disadvantage of Binary Thresholding is that cuts the color spectrum in two equal parts, which makes it difficult to observe the brightness in the picture. Due to this technique there is a loss of image details as well which might not be desired.

The advantage of Adaptive Threshold is that, it can be added to multiple thresholds which is desireable during imagae processing. It can also help when there are multiple lighting conditions within a single image.
 
   
