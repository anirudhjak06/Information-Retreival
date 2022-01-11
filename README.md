# Information-Retrieval (Inverted Indexing)

Indian Institute of Information Technology, Sri City.
IR ASSIGNMENT - 01
Name : Anirudh Jakhotia
Roll : S20190010007

- Steps to execute the file:

1. The python code file and ths-181-dataset should be stored in the same folder for avoiding errors.
2. Now, we have to install certain packages for running the program without any errors.
* pip install tqdm
* pip install colorama
* pip install nltk


3. After the installation of nltk, Open Python Interpreter by command ”python”. Then type these two commands.
* import nltk
* nltk.download(‘punkt’)

4. Then, exit the interpreter by the command “quit()”.
5. All these above steps help us to get ready for code execution and allow us to write our code.
6. Now, import packages for our use like, in nltk.stem, import PorterStemmer.
7. In the code, give a correct path to the dataset directory in the main function to perform the tasks correctly.
8. Once the writing of code is done, we execute our program by typing the following command "python Assign012019007.py" in terminal.
9. We can see an output file in the name: "Assign012019007-output.txt"

Important Details :

1. The specific choice of Data Structure used is - Hash Tables, Arrays.
2. Dictionary Data Structure is used here which has properties of a Hash table that take O(1) i.e., it takes constant time to fetch data.
3. Initially, Time Complexity is - O(n*p*q) 
       where,  
       n => Total no of txt files 
       p => Words per document
       q => Average word-size 
       n*p*q => total no of characters in all documents
       As, q is almost negligible
       Hence, Time complexity is O(n*p)

4. Space Complexity - O(m*n)
     	m =>  Unique words 
	n => Number of text files
       	Hence, Space complexity is O(m*n)


## Implementation Explanation :

(i) class PositoningElements:

Explanation:
This class will take document id and its frequency and create a separate posting list.

(ii) class Inverted_Positions:
	def Task_strings(self, strings):

Explanation:
This function replaces special characters with space or nothing.

(iii) def Task_record(self, file_name, file_content):

Explanation:
This function extracts words from each file and counts the frequency of each word.


(iv) def position_archive(self, wordbook_track):

Explanation:
This function extracts each file from the folder and sends each file to the Task_record function


(v) def export_index(self, output_file_name="Assign012019007-output"):

Explanation:
This function exports the output of each item in the posting list to a new output file with the frequency of the total number of text files.




-------------------------- THE END  ----------------------------------