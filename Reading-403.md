
# File and Stream I/O  
I/O stands for Input and Output. And I/O is talking about the transfer of data to or from a storage medium. 


**Files and Directories**  
Files can be used in I/O namespace to open up folders.   

**Streams**  
Stream supports reading and writing. 
Streams involve 3 things
1. Reading - Transferring data from the stream into a data structure
2. Writing - Transferring data to a stream from a source
3. Seeking - Looking for a modifying the current position in the stream


** Readers and Writers**  
The I/O namespace allows for encoded characters to be used. You can write them into the streams. 
Types of these are:
- BinaryReaders
- StreamReaders and Writers
- StringReaders and Writers
- TextReaders and Writers


# Write to a file  
By specifing a path to a ducument. You can write data to a file in C#. This can be done using several lines of code. 
``` string documentPath =
          Environment.GetFolderPath(Environment.SpecialFolder.MyDocuments);

        
        using (StreamWriter outputFile = new StreamWriter(Path.Combine(docPath, "WriteLines.txt")))
        {
            foreach (string line in lines)
                outputFile.WriteLine(line);
        }  
  ```
There are other ways to do this detailed [here](https://docs.microsoft.com/en-us/dotnet/standard/io/how-to-write-text-to-a-file)


# Read to a file  
Using some of the same logic we learned to write to a file. We can read from a file as well. We would write to the console the lines from the file. We can specify what characters we want to avoid like white space. 

        
        
