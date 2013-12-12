Apple Documentation Style Latex Template
===============================

Using this template you can generate PDFs similar to Apple documentation PDFs.


Code highlighting using minted:

To compile document that uses minted powered code listings use the following command:
$ xelatex --file-line-error --synctex=1 --shell-escape "Apple Documentation Template.tex"

To use Xcode pygments style this extra setup is required:

1) Copy xcode.py into pygments "styles" directory
/Library/Python/2.7/site-packages/Pygments-1.6-py2.7.egg/pygments/styles/

2) Edit file pygments/styles/ __init__.py and add the following line to the STYLE_MAP dictionary:
'xcode':    'xcode::XcodeStyle',