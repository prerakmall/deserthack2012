Exotel Record Search

Description:

A GUI based desktop app which allows files to be processed just after a call is recorded. The solution provided by us includes the use of Google Speech to Text API for the 
conversion of the recordings and a Search Field to look through the converted files.

Expected Usage:
The customer of Exotel should use SpeechDB to add the transcript of the just recorded file to the database. The file should have a UNIQUE NAME. Then the DBSearch app can be used(with the database) to search for keywords.
Please note that the transcript may or may not be an exact textual version of the conversation, but, it is expected that it will include important keywords for sure. For better results, WAV files which have low background noise and a clear voice should be used.


Our Solution:
Separate Apps for preparing Database (SpeechDB) and Searching for text (DBSearch) in the transcript of the call recordings. 

Note:
Source code for both apps is provided with the compiled binaries for an Ubuntu 32-bit system. Source must be compiled using QT. Load the *.pro file into qt and build the application. By default the application is built in the source code folder.
The script "soxconvert.py" must be included with the binaries for functioning of the SpeechDB app.

Requirements :  
For A LINUX(Ubuntu, LinuxMint, (k,l,x)ubuntu) based system  
    1.Python - For the custom script to process files
    2.sox - For internal audio format conversions
    3.Qt (To compile/edit applications) - To prepare the GUIs

NOTE: Can be expanded to other systems supported by QT. eg. Windows.


Scope:

1.Currently provision for adding a file at a time to the database. Can be extended to handle multiple file additions too.
2.Additional Noise Reduction can be achieved before processing for greater precision.
