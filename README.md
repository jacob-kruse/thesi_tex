# thesi_tex

This repository contains all of the LaTeX files for compiling my Thesis for my Master of Science degree in Computer Science at the University of Georgia.

## Instructions

The following instructions are written to compile the LaTeX files and produce the resulting `.pdf` file. Compiling the present version of the LaTeX files will produce the current version of `Thesis_Jacob_Kruse.pdf`. 

First, go to the `/perl` directory of this repository using File Explorer or with the command below.

    cd /perl 

Run the Strawberry Perl shell by double clicking on `portableshell` in File Explorer or with the following command.

    portableshell.bat

This will open a Command Prompt window with the following statement.

    ----------------------------------------------
    Welcome to Strawberry Perl PDL Edition!
    * URL - https://strawberryperl.com + http://pdl.perl.org
    * to launch perl script run:      perl c:\my\scripts\pdl-test.pl
    * to start PDL console run:       pdl2
    * to update PDL run:              cpanm PDL
    * to install extra module run:    cpanm PDL::Any::Module
            or if previous fails:    ppm PDL::Any::Module
    * or you can use dev tools like:  gcc, g++, gfortran, gmake
    * see README.TXT for more info
    ----------------------------------------------
    Perl executable: C:\Users\jacob\Downloads\thesi_tex\perl\perl\bin\perl.exe
    Perl version   : v5.42.0 / MSWin32-x64-multi-thread
    PDL version    : 2.100

If you see something similar to what is shown above, you have successfully started Strawberry Perl and are ready to compile the document with LaTeX. If this does not work, the third party code included in this repository may be out of date or not functioning correctly. To download Strawberry Perl go to the link below. <br>
[Strawberry Perl](https://strawberryperl.com/)

In the Strawberry Perl shell, go back to the `/thesi_tex` directory with the following command.

    cd ..

Then, compile the `Thesis_Jacob_Kruse.tex` file with the command below.

    latexmk -pdf Thesis_Jacob_Kruse.tex

The command above compiles the file once and produces the `Thesis_Jacob_Kruse.pdf` file. If you wish to compile once and then wait for changes use the following command.

    latexmk -pdf -pvc Thesis_Jacob_Kruse.tex

This causes the `Thesis_Jacob_Kruse.tex` file to compile automatically when any of the files are modified and saved.