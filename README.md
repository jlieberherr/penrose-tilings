# Create Penrose tilings by deflation

For a summary of the theory on Penrose tilings see [here](https://tartarus.org/~simon/20110412-penrose/penrose.xhtml).

The Jupyter-notebook [create_penrose_tiling.ipynb](https://github.com/jlieberherr/penrose-tilings/blob/main/create_penrose_tiling.ipynb) provides some functionalties to generate Penrose tilings of type P2 and P3 by deflation. The main functions are:
- ```draw_rts(rts)```: plots the Robinson triangles in list ```rts```. This generates a Penrose tiling.
- ```draw_penrose_tiling()```: plots a Penrose tiling.
- Both functions have (amongst others) the following optional arguments:
   - ```draw_common_side```: draws the common side of two Robinson triangles forming a Penrose tile if ```True``` .
   - ```fill```: fills the Robinson triangles with the color defined in ```TRIANGLE_COLOR_PER_TYPE_SHAPE_SIDE``` if ```True```.
   - ```svg_file_name```: saves the generated Penrose tiling to an svg-file (only if not '')
   
Example 1: ```draw_penrose_tiling(2, 'A', 'F', 8)``` draws the Penrose tiling with colors of type P3 based on the deflation of an acute front side robinson triangle of type 2 with 8 iterations:
![A P3 Penrose tiling](/images/filled_2_A_F_8.PNG)

Example 2: ```draw_penrose_tiling(1, 'O', 'B', 8, fill=False)``` draws the Penrose tiling of type P2 based on the deflation of an obtuse back side robinson triangle of type 1 with 8 iterations:
![A P2 Penrose tiling](/images/empty_1_O_B_8.PNG)

For more examples see [create_penrose_tiling.ipynb](https://github.com/jlieberherr/penrose-tilings/blob/main/create_penrose_tiling.ipynb).


## Installation
- Download Python 3 (at least 3.8)
- Clone this repository into your development folder ```git clone https://github.com/jlieberherr/penrose-tilings.git```
- Create a new virtual environment ```path/to/python.exe -m venv /path/to/new/virtual/ENV_PENROSE_TILING``` and activate it ```/path/to/new/virtual/ENV_PENROSE_TILING\Scripts\activate```
- Navigate to your development folder an install libraries ```pip -r requirements.txt```
- Start Jupyter by ```jupyter lab```

