# Create Penrose tilings by deflation

For a summary of the theory on Penrose tilings see [here](https://tartarus.org/~simon/20110412-penrose/penrose.xhtml).

The Jupyter-notebook [create_penrose_tiling.ipynb](https://github.com/jlieberherr/penrose-tilings/blob/main/create_penrose_tiling.ipynb) provides some functionalities to generate Penrose tilings of type P2 and P3 by deflation.
   
Example 1: ```draw_penrose_tiling(2, 'A', 'F', 8)``` draws the Penrose tiling with colors of type P3 based on the deflation of an acute front side robinson triangle of type 2 with 8 iterations:
![A P3 Penrose tiling](/images/filled_2_A_F_8.PNG)

Example 2: ```draw_penrose_tiling(1, 'O', 'B', 8, fill=False)``` draws the Penrose tiling of type P2 based on the deflation of an obtuse back side robinson triangle of type 1 with 8 iterations:
![A P2 Penrose tiling](/images/empty_1_O_B_8.PNG)

For more examples and documentation of the two main functions ```draw_rts(...)``` and ```draw_penrose_tiling(...)``` see [create_penrose_tiling.ipynb](https://github.com/jlieberherr/penrose-tilings/blob/main/create_penrose_tiling.ipynb).


## Installation
- Download Python 3 (at least 3.8)
- Clone this repository into your development folder ```git clone https://github.com/jlieberherr/penrose-tilings.git```
- Create a new virtual environment ```path/to/python.exe -m venv /path/to/new/virtual/ENV_PENROSE_TILING``` and activate it ```/path/to/new/virtual/ENV_PENROSE_TILING\Scripts\activate```
- Navigate to your development folder an install libraries ```pip -r requirements.txt```
- Start Jupyter by ```jupyter lab``` and open the Jupyter-notebook ```create_penrose_tiling.ipynb```

