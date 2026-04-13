# Installing C++ 

This course uses c++. There are many ways to install a c++ compiler on your machine and you may already have c++ installed. If you don't, here are some suggestions on how to do that.

# MinGW for Windows
- MinGW is an open-source project that provides a c++ compiler for windows. The steps to getting a c++ compiler on windows with MinGW are: 1. Get an archive of MinGW, 2. Extract the archive. 3. Add the `bin` folder to your path, and 4. Test that the compile works.
1. Get a MinGW archive
   - Go to the release page for the portable version of MinGW here: https://github.com/niXman/mingw-builds-binaries/releases
   - There are a lot of release on the release page. They will probably all work on a modern Windows environment. If you want the version compatible with most systems, choose a release that starts with `x86_64` and includes `posix-seh-ucrt`.
2. Extract the archive
   - Download the appropriate archive and extract it at a location with a simple path, e.g., `c:\mingw\`.
3. Add the `bin` folder to your path
   - Add the the `bin` folder to your PATH variable. For example, if you extracted the mingw archive to `c:\mingw\` then you would add `c:\mingw\bin` to your PATH variable.
   - There are many ways to add this folder to your path. One way is to run the command: `setx PATH "%PATH%;C:\mingw\bin"` (if c:\mingw is where you extracted your archive)
4. Test your installation
   - The program that compiles c++ in MinGW is called `g++`. After you have updated your path variable, close your command prompt (terminal), open a new one, and run the command `g++ -v`. 
   - If the command prompt gives you the details of your g++ compile, then you have successfully installed c++. If not, please review these steps or contact the instructor.