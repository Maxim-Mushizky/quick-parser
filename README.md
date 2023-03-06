# quick-parser
Project for parsing tabular or document data easily, using pandas and spacy libraries.

## Introduction 
This is an open source project intended to make life easier for data analysis using Python. It is intended to be easily accessed, with short learning curve but also verstile enough to be used by advanced users.<br>
To achieve this, the project will provide the following API (example):

~~~python
from quick_parser import DataReader

path_to_file = "../sources/my_data.csv"
my_data = DataReader(path_to_file) # Robust enough to use the correct pandas load_* method - in this case load_csv
res = my_data.query('get from column 1,4 and 9 all values greater than 1, 5 and 16') # the main magic method- query (temporary naming)

print(res.result, res.query) # will save a dataclass containing all relevant parts of the query

~~~
### Explanation 

* DataReader- Will be the main class that will use the DataFrame object from pandas. It will be robust enough to read any tabular file and arrange it
* query- Will be DataReader's main method and will enable free search of the data contained by connecting free text to pandas methods

## How to Contribute
There are many ways you can contribute to quick-parser. Here are some ideas:

* Report bugs: If you find a bug, please open an issue on our GitHub repository and provide as much detail as possible.
* Suggest new features: If you have an idea for a new feature, please open an issue on our GitHub repository and explain your idea in detail.
* Write code: If you're a developer, you can contribute to [Your project name] by writing code. Check out our contributing guidelines for more information on how to get started.
* Improve documentation: If you're not a developer, you can still contribute by improving our documentation. If you find something that's unclear or could be explained better, please let us know by opening an issue on our GitHub repository.
* Spread the word: If you like [Your project name], please help us spread the word by telling your friends and colleagues about it.

### Getting Started
To get started with quick-parser, you'll need to [instructions on how to install and run your project]. Once you have everything set up, you can start [instructions on how to use your project].

### Code of Conduct
We take our code of conduct seriously and expect all contributors to adhere to it. Please read our code of conduct before contributing.

### License
quick-parser is released under the MIT License. The MIT License is a permissive open-source license that allows anyone to use, modify, and distribute the software for any purpose, as long as the original copyright and license notice is included. This means that anyone can use and modify [Your project name] for personal or commercial purposes without having to ask for permission. However, the license comes with no warranties or guarantees, and the original authors are not liable for any damages or losses caused by the software.

Please read the license file for more information.

Thank you for considering contributing to [Your project name]. We appreciate your support!
