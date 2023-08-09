# Curse Word Detection Script

This is a Python script called `get_curses.py` that identifies and extracts sections of a transcript containing unacceptable curse words. The script reads a transcript file, searches for predefined curse words, and outputs identified sections to an Excel workbook.

## Prerequisites

- Python 3.x
- The `openpyxl` library (`pip install openpyxl`)

## Usage

1. Clone this repository or download the `get_curses.py` script.

2. Open a terminal/command prompt and navigate to the directory containing the `get_curses.py` script.

3. Run the script with the following command but Replace `filename` with the path to your transcript file:

```bash
python get_curses.py filename
```

4. The script will create an Excel workbook named `identified_sections.xlsx` containing the timecode, speaker, and lines with curse words.

## How it Works

1. The script checks for the correct command-line argument usage and the presence of a transcript filename.

2. It defines a list of unacceptable curse words.

3. The transcript file is opened and read line by line.

4. An Excel workbook and worksheet are created.

5. Headers for the worksheet are written.

6. The script iterates through the transcript, processing timecode, speaker, and lines of dialogue.

7. For each line, it checks for the presence of curse words using a case-insensitive comparison.

8. If a curse word is found, the corresponding section is written to the worksheet.

9. The Excel workbook is saved as `identified_sections.xlsx`.

## Note

- Make sure your transcript file is structured with timecodes, speakers, and lines of dialogue in consecutive lines.

- This script is case-insensitive when checking for curse words.

- The identified sections will be saved in an Excel workbook named `identified_sections.xlsx` in the same directory as the script.

## License

This project is licensed under the [MIT License](LICENSE).

Feel free to modify and use the script according to your needs.

---
