Reference
```
https://forum.qiime2.org/t/lefse-after-qiime2-to-test-at-all-taxonomic-levels/15462/22
```

# A. Installing-lefse-on-Linux
```
$ conda create -n lefse -c conda-forge python=2.7.15
```
```
$ conda activate lefse
```
```
$ conda install -c bioconda -c conda-forge lefse
```
                      or 
```
conda install -c bioconda lefse=1.0.8.post1
```


# B. Installing-lefse-on-M1-MAC
1. First install Rosetta following this:

  ```
  https://github.com/rayotoo/rosetta-2-installation
   ```
   
2. Set terminal to open in rosetta mode following this:
   
  ```
  https://medium.com/@v.yavdoshenko/yet-another-way-to-improve-the-terminal-experience-for-developers-on-the-apple-silicon-ce87af9d6edf
  ```

3. Create a new Conda environment specifying the platform: Use the following command in the Terminal to create a new environment, specifying **osx-64** for the       
  platform. Replace **myenv** with the name you want to give to your environment and adjust the Python version as necessary.

  ```
  CONDA_SUBDIR=osx-64 conda create --name myenv python=2.7
  ```

  ```
  conda activate myenv 
  ```

4. Installing Docker:
Download Docker and Navigate to this directory and run these:
   ```
   sudo hdiutil attach Docker.dmg
   ```
   ```
   sudo /Volumes/Docker/Docker.app/Contents/MacOS/install
   ```
   ```
   sudo hdiutil detach /Volumes/Docker
   ```

5. Check to confirm that Docker is installed
   ```
   docker --version
   ```
   ```
   docker info
   ```
   
6. Link to download Debian Miniconda image (Python 2.7) with the bioBakery tool Lefse installed.
   Image didn't seem to contain an installed lefse so this was installed.

   Download the docker image to a directory of interest
   ```
   docker run -it biobakery/lefse bash
   ```
   to exit, use
   ```
   exit
   ```
   
7. To run:
   ```
   docker run --platform linux/amd64 -it biobakery/lefse bash
   ```

   
