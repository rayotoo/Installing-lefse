# Installing-lefse-on-M1-MAC
1. First install Rosetta following this:

  ```
  https://medium.com/@v.yavdoshenko/yet-another-way-to-improve-the-terminal-experience-for-developers-on-the-apple-silicon-ce87af9d6edf
   ```
   
3. Set terminal to open in rosetta mode following this:
   
  ```
  https://medium.com/@v.yavdoshenko/yet-another-way-to-improve-the-terminal-experience-for-developers-on-the-apple-silicon-ce87af9d6edf
  ```

5. Create a new Conda environment specifying the platform: Use the following command in the Terminal to create a new environment, specifying **osx-64** for the       
  platform. Replace **myenv** with the name you want to give to your environment and adjust the Python version as necessary.

  ```
  CONDA_SUBDIR=osx-64 conda create --name myenv python=2.7
  ```

  ```
  conda activate myenv 
  ```
