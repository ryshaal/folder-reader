
  

# Directory Structure Reader

Folder Reader is a command-line tool that helps you analyze and understand your directory structures. It provides detailed information about files and folders in a specified directory, making it easier to manage and organize your files.

This Python script reads the directory structure of a given folder and outputs the folder hierarchy in both **Markdown** and **Plain Text** formats. The generated files are saved into separate directories (`result_md` for Markdown and `result_txt` for plain text).

<a href="https://ko-fi.com/riyhsal">
  <img src="https://ryshaal.github.io/assets/img/doante.svg" width="182" alt="Donate">
</a>
  

## Features

  

- Recursively lists the contents of a directory, including subdirectories.

- Outputs directory structure with proper indentation.

- Saves the structure in both Markdown (`.md`) and Plain Text (`.txt`) formats.

- Automatically handles duplicate filenames by appending a unique identifier.

- Creates a `result_md` folder for Markdown files and a `result_txt` folder for text files.

  

## How to Use

  

1. Clone this repository and navigate to the directory:

```bash

git clone https://github.com/ryshaal/folder-reader.git
cd folder-reader

```

  

2. Run the script:

```bash

python list_directory.py

```
or
```bash

python list_directory_v2.py

```

  

3. Input the folder path when prompted:

```

Masukkan alamat folder yang ingin dibaca: /path/to/folder

```

  

4. The script will generate two output files:

- A `.md` file in the `result_md` directory.

- A `.txt` file in the `result_txt` directory.

  

The files will be named with the format `Directory structure <folder_name> <date>.md` and `Directory structure <folder_name> <date>.txt`.

  

## Example Output

  

For a directory with the following structure:

  

```

my_folder/

├── sub_folder1/
│ └── file1.txt
├── sub_folder2/
└── file2.txt

```

  

The output will be:

  

### Markdown File (`.md`)

  

```md

# Directory Structure for my_folder

  

📁 my_folder


- 📁 sub_folder1

    - 📄 file1.txt

- 📁 sub_folder2

    - 📄 file2.txt

```

  

### Plain Text File (`.txt`)

  

```

Directory Structure for my_folder

  

my_folder

- [Folder] sub_folder1
  - [File] file1.txt
- [Folder] sub_folder2
  - [File] file2.txt

```

  

## Requirements

  

- Python 3.x


## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request


## License

  

This project is licensed under the MIT License.
