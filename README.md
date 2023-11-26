<h1 align="center">Style Transfer using CNN:</h1>

## Follow the steps 
**Downloading and Preparing Dataset**

```bash
!wget http://images.cocodataset.org/zips/test2017.zip
!mkdir './dataset'
!unzip -q ./test2017.zip -d './dataset'
```
Downloads the COCO dataset's test set, which is commonly used for computer vision tasks.

Creates a directory named 'dataset' and extracts the contents of the downloaded ZIP file into it.

**Downloading Pre-trained Model**

```bash
!mkdir ./checkpoints
!wget -q -O 'best_model.pth' https://www.dropbox.com/s/7xvmmbn1bx94exz/best_model.pth?dl=1
!mv best_model.pth ./checkpoints
```
Creates a directory named 'checkpoints.'

Downloads a pre-trained model named 'best_model.pth' from Dropbox and saves it in the 'checkpoints' directory.

**Creating Directories for Content and Style Images**


```bash
!mkdir ./content
!mkdir ./style
!wget -q https://github.com/myelinfoundry-2019/challenge/raw/master/japanese_garden.jpg -P './content'
!wget -q https://github.com/myelinfoundry-2019/challenge/raw/master/picasso_selfportrait.jpg -P './style'
```
Creates directories named 'content' and 'style' to store input images.

Downloads a content image ('japanese_garden.jpg') and a style image ('picasso_selfportrait.jpg') from GitHub and saves them in the corresponding directories.

**Sample Result**

Input:

![Dog-Pre](https://github.com/ritikas20/dashtoon-Gen-AI/assets/108460591/1cfafad9-7767-44cb-8e2c-f96fe4b22ce8)

Result:

![Dog-after](https://github.com/ritikas20/dashtoon-Gen-AI/assets/108460591/01cd4ffd-701b-462a-ab83-c02663c9a5c3)

