# SpaceApps2023

## NASA Space Apps Challenge 2023

<p>
NOTE: This README.md file was editted after the project submission date and should serve to connect and describe resources related to the project, and explain the purpose of this repo.
The remaining files in this repo remain uneditted after the submission date.
Full information about this Space Apps Project is on the relevant SpaceApps Project Page, and includes the other files in this repo.
</p>
<p>
Within this repo are two files:
</p>
<p>
  1) RLJLW-Challenge-2023.pptx  
</p>
<p>
  2) EMIT_L2A_RFL_001_20230119T114235_2301907_004_ch_100-1.jpg  
</p>

### RLJLW-Challenge-2023.pptx

<p>
RLJLW-Challenge-2023.pptx is a power point demonstration that shows some of the features of the Space Apps Challenge Project, and what was created.
</p>
<p>
  Of particular interest inside the presentation the following are demonstrated:
</p>

<p>
  Freely available NASA EMIT Sensor data can be downloaded, processsed and converted to color images of the surface, as the sensor contains the spectra of human visible light.
  <br /><br />
  There are various bands (285 bands) of light that the sensor can detect, an aproximate range of 381 to 2493 nanometers, many which are in the infrared range.
  <br /><br />
  Each band of light, for each pixel, is saved in a data file.
  <br /><br />
  Collectively these 285 bands create unique spectographic profiles that can be analysed to classify types of surfaces.
  <br /><br />
  Vegetation on a surface using a NDVI calculation, which is based on red and infra red light,
  and that plants absorb high amounts of red light but reflect infrared light, this allows for a means of vegetation surface classification, using a well known NDVI vegetation classification
  calculation which is included in this presentation.  
</p>
<p>
The images described in this powerpoint were created from data in NASA EMIT FILE EMIT_L2A_RFL_001_20230119T114235_2301907_004.nc, which was then processed using tools writting
by the developer in Python.
</p>

### EMIT_L2A_RFL_001_20230119T114235_2301907_004_ch_100-1.jpg
<p>
<a href="https://rljlw.github.io/SpaceApps2023/EMIT_L2A_RFL_001_20230119T114235_2301907_004_ch_100-1.jpg">EMIT_L2A_RFL_001_20230119T114235_2301907_004_ch_100-1.jpg</a>
Is cropped portion of a fully processed NASA EMIT data file, the image image was created while working on the project using an ASP.NET data to image tool created by this developer.
</p>
<p>
A 1.8GB data file was downloaded from NASA, EMIT_L2A_RFL_001_20230119T114235_2301907_004.nc, which contains the region of Cape Town, South Africa.
</p>
<p>
A C# ASP.NET tool was created to process the data file, to show band 100 (counting from band 0 as the first band) of the EMIT sensor data, which is an infrared band in the region of aproximately 1.1 microns.
</p>
<p>
The image reflectance intensity was then mapped to a full 1242 x 1280 grey scale BMP image.
</p>
<p>
The image was then cropped and converted to a JPG file showing a portion of the image.
</p>
