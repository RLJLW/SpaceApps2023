# NASA International Space Apps Challenge

<p>
NOTE: This README.md file was editted after the project submission date and should serve to connect and describe resources related to the project, and explain the purpose of this repo.
The remaining files in this repo remain uneditted after the submission date.
Full information about this Space Apps Project is on the relevant SpaceApps Project Page, and includes the other files in this repo.
</p>

# Background

<p>
  <strong>NASA International Apps Challenge</strong> is an event where coders, scientists, designers, storytelers, makers, technologiess, and innovators from around the world participate
  in a selection of challenges to use open data from NASA and its Space Agency Partners to create solutions to challenges we face on Earth and in space.
</p>

<p>
  During the challenges participants create their solutions submit them to the Space Apps Challenge website.  This repo contains part of the the solution for the challenge that the developer particpated in.
</p>

## NASA EMIT Sensor Data
<p>
This project used DATA from the NASA EMIT Sensor that was downloaded from the NASA Website at:
https://search.earthdata.nasa.gov/search
<br /><br />
EMIT is an advanced imaging spectrometer aboard the ISS (International Space Station) that takes an image of the surface of the Earth over various locations.
<br /><br />
Each image, that is generated measures a 285 band (number of samples) of the spectrum for every point (pixel).
These bands lie in the aproximate range of 381 to 2493 nanometers, which covers shorter visible light (violet) at the shorter wavelengths, to to far into the the infrared range.
<br /><br />
There are various data files made available relating to the surface image, which can be read more about at the
NASA EMIT Instrument Overview: https://earth.jpl.nasa.gov/emit/instrument/overview/
<br /><br />
The surface reflectance file (known as the Level2a product) which this project uses is a processed version of the original data taken by the sensor which attempts to screen out
the effects of clouds and atmospheric effects as is possible, to provide a more reliable way of characterising a surface.
<br /><br />
See: https://earth.jpl.nasa.gov/emit/data/data-products/
<br /><br />
This data is made available to download on the Earth Data Search Website when an image is selected.
</p>

## In this Repo

<p>
Within this repo are two files:
</p>
<p>
  1) <a href="https://rljlw.github.io/SpaceApps2023/RLJLW-Challenge-2023.pptx">RLJLW-Challenge-2023.pptx</a> (click to view)
</p>
<p>
  2) <a href="https://github.com/RLJLW/SpaceApps2023/blob/main/EMIT_L2A_RFL_001_20230119T114235_2301907_004_ch_100-1.jpg">EMIT_L2A_RFL_001_20230119T114235_2301907_004_ch_100-1.jpg</a>
</p>



### RLJLW-Challenge-2023.pptx

<p>
RLJLW-Challenge-2023.pptx is a power point demonstration that shows some of the features of the Space Apps Challenge Project, and what was created.
</p>
<p>
  Of particular interest inside the presentation the following are demonstrated:
</p>

<ul>
  <li>NASA EMIT Sensor data can be processsed and converted to color images of the surface, as the sensor contains the spectra of human visible light.</li>
  
  <li>Spectographic graphs can be generated for each pixel (location on the surface), as </li>

  <li>Each band of light, for each pixel, is saved in a data file.</li>

  

  <li>Collectively these 285 bands create unique spectographic profiles that can be analysed to classify types of surfaces.</li>

  <li>Vegetation on a surface using a NDVI calculation, which is based on red and infra red light,
  and that plants absorb high amounts of red light but reflect infrared light, this allows for a means of vegetation surface classification, using a well known NDVI vegetation classification
  calculation which is included in this presentation.</li>



</ul>

<p>
The images described in this powerpoint were created from data in NASA EMIT FILE EMIT_L2A_RFL_001_20230119T114235_2301907_004.nc, which was then processed using tools writting
by the developer in Python.
</p>

### EMIT_L2A_RFL_001_20230119T114235_2301907_004_ch_100-1.jpg

<figure>
<img src="https://rljlw.github.io/SpaceApps2023/EMIT_L2A_RFL_001_20230119T114235_2301907_004_ch_100-1.jpg" width="100%" />
  <figcaption>Cropped image file created from NASA EMIT Data, showing band 100 in the infrared spectrum of Cape Town South Africa</figcaption>
</figure>
<p>
  &nbsp;
</p>

<p>

<a href="https://github.com/RLJLW/SpaceApps2023/blob/main/EMIT_L2A_RFL_001_20230119T114235_2301907_004_ch_100-1.jpg">EMIT_L2A_RFL_001_20230119T114235_2301907_004_ch_100-1.jpg</a>
Is a cropped portion of a fully processed NASA EMIT data file, the image image was created while working on the project using an ASP.NET data to image tool created by this developer.
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

## Sources / Files

NASA Earth Data Search:
<br />
https://search.earthdata.nasa.gov/search
<br /><br />

NASA EMIT Instrument Overview:
<br />
https://earth.jpl.nasa.gov/emit/instrument/overview/
<br /><br />

EMIT Data Products:
<br />
https://earth.jpl.nasa.gov/emit/data/data-products/
<br /><br />

NASA Surface Reflectance Files used in this project
<br />
https://data.lpdaac.earthdatacloud.nasa.gov/lp-prod-protected/EMITL2ARFL.001/EMIT_L2A_RFL_001_20230119T114235_2301907_004/EMIT_L2A_RFL_001_20230119T114235_2301907_004.nc (1.8&nbsp;GB)
<br /><br />

Normalized difference vegetation index
<br />
https://en.wikipedia.org/wiki/Normalized_difference_vegetation_index
