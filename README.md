# Periodic Table Python Script

This small Python script lets you query basic information about chemical elements by entering their atomic number.

The script uses the `periodictable` Python package to look up element details such as atomic number, symbol, name, atomic mass, and density.

## Files

- `periodic_table.py` — the main script. Prompts the user for an atomic number and prints element information.
- `requirements.txt` — lists the Python dependency required to run the script.

## Dependencies

- Python 3.7 or newer is recommended.
- The script depends on the `periodictable` package (installable from PyPI).

## Install (from scratch)

Open a PowerShell terminal and run the following commands.

1. Create and activate a virtual environment (recommended):

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2. Upgrade pip and install dependencies:

```powershell
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

If you prefer using a system-wide installation (not recommended), you can run:

```powershell
python -m pip install periodictable
```

## Run

With the virtual environment activated, run:

```powershell
python periodic_table.py
```

The script will prompt:

Enter atomic number:

Type an integer (for example `8` for oxygen) and press Enter. The script will print details for that element.

## Example session:

```
Enter atomic number: 8
Atomic Number: 8
Symbol: O
Name: oxygen
Atomic Mass: 15.999
Density: 0.001429
```

### Notes

- The script assumes the user inputs a valid integer atomic number. If you input an invalid number (e.g., 0 or a value beyond the known elements), `periodictable` may raise an IndexError or return None-like values.
- Consider adding input validation and nicer error messages if you plan to make this script more robust.

### License

This project contains a small utility script; no license is specified. Add a LICENSE file if you need one.

### I love you all! Happy coding!