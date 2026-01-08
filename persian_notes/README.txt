============================================
   Persian Linear Algebra Lecture Notes
   (جبر خطی: ذات جبر خطی)
============================================

Based on 3Blue1Brown's "Essence of Linear Algebra" series

============================================
REQUIREMENTS
============================================

1. MiKTeX (Full Installation)
   Download: https://miktex.org/download
   - Select "Complete" installation
   - Make sure XeLaTeX is included

2. Persian Fonts (must be installed on system):
   - XB Zar (primary text font)
   - XB Titre (headers)

   If fonts are missing, the compilation will fail.
   You can download Persian fonts from:
   - https://fontlibrary.org
   - https://fontsquirrel.com

============================================
HOW TO COMPILE
============================================

Option 1: Using the batch script (Windows)
------------------------------------------
1. Navigate to the scripts folder
2. Double-click build.bat
3. The PDF will be saved to:
   persian_notes/output/linear_algebra_persian.pdf

Option 2: Using Python script
------------------------------------------
1. Open command prompt
2. Navigate to the project directory
3. Run: python scripts/compile_pdf.py
4. The PDF will be saved to:
   persian_notes/output/linear_algebra_persian.pdf

Option 3: Manual compilation
------------------------------------------
1. Open command prompt in persian_notes folder
2. Run these commands:
   xelatex main.tex
   xelatex main.tex
   xelatex main.tex
   (Run 3 times to resolve all references)

============================================
FILE STRUCTURE
============================================

persian_notes/
├── main.tex          <- Master document (compile this)
├── preamble.tex      <- LaTeX packages and settings
├── commands.tex      <- Math macros
├── lectures/         <- Individual lecture files
│   ├── lecture01.tex <- Vectors
│   ├── lecture02.tex <- Linear Combinations & Basis
│   ├── lecture03.tex <- Linear Transformations
│   ├── lecture04.tex <- Determinants
│   ├── lecture05.tex <- Inverse Matrices
│   ├── lecture06.tex <- Dot Products
│   ├── lecture07.tex <- Cross Products
│   ├── lecture08.tex <- Cramer's Rule
│   ├── lecture09.tex <- Change of Basis
│   ├── lecture10.tex <- Eigenvectors
│   ├── lecture11.tex <- Computing Eigenvalues
│   └── lecture12.tex <- Abstract Vector Spaces
└── output/           <- Generated PDF goes here

============================================
TROUBLESHOOTING
============================================

Error: "Font not found"
-----------------------
Install the Persian fonts XB Zar and XB Titre.
Make sure they are installed system-wide.

Error: "Package not found"
-----------------------
MiKTeX should auto-install packages.
If not, open MiKTeX Console and install:
- xepersian
- bidi
- pgfplots
- tcolorbox

Garbled Persian text
-----------------------
Make sure you're using XeLaTeX, not pdfLaTeX.
The command should be: xelatex main.tex

============================================
CONTENTS
============================================

12 Comprehensive Lectures covering:

1. Introduction to Vectors (مقدمه‌ای بر بردارها)
2. Linear Combinations & Basis (ترکیبات خطی و پایه)
3. Linear Transformations & Matrices (تبدیلات خطی)
4. 3D Transformations & Determinants (دترمینان)
5. Inverse Matrices & Null Space (ماتریس معکوس)
6. Dot Products & Duality (ضرب داخلی)
7. Cross Products (ضرب خارجی)
8. Cramer's Rule (قاعده کرامر)
9. Change of Basis (تغییر پایه)
10. Eigenvectors & Eigenvalues (مقادیر ویژه)
11. Computing Eigenvalues & Eigenbasis (محاسبه مقادیر ویژه)
12. Abstract Vector Spaces (فضاهای انتزاعی)

Each lecture includes:
- Formal definitions with LaTeX math
- Geometric intuition boxes
- Practical examples
- TikZ diagrams
- Exercises

============================================
