# Denoising_ISRO
Denoising application

This application uses Python and Django in the backend to run. One can upload a .qub file and its associated .hdr file in order to run the denoising process.

We need the following python libraries to run the project:
  django
  numpy
  rasterio
  skimage
  os

We can install the above libraries using the command: pip install <library_name_here> 
eg: pip install django

After all the libraries have been installed, one needs to navigate the folder and go to the location where the "manage.py" file is present. Then, in the same location, one needs to open the commandline and run the following command:
 python manage.py runserver
After that we can open the application on our browser (without internet) with the url shown in the command line. 

Then, in the application, we need to enter the parameters weight which indicates the amount of denoising we want, and the number of iterations we want. Usually , we can keep weight as 5 and iterations as 40.

After a while, we will recieve a denoised .qub file as response in the downloads folder.
This .qub file needs to be associated with the original .hdr file of the image, and can be used accordingly.
