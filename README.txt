RASPBERRY PI CAMERA SETUP
1) Download and unzip RASPI_CAM.zip into a Raspberry Pi
2) Ensure that the Pi is connected to a camera
3) Install the required packages using "pip install -r raspi_req.txt"
4) Edit settings.txt. More information as provided:
	url should be a valid firebase url
	apikey should be the api key for the aforementioned firebase
	base_dir is where the image recognition weights are stored (default is same directory as final.py)
	min_confidence is a float between 0 and 1 (default 0.5)
	min_threshold is a float between 0 and 1 (default 0.3)
	rotation is the rotation adjustment for the Raspberry Pi camera
	rm_no is the room number is <block><floor> format
	debug is True if you want to save analysed images for debugging purposes (default False)
5) Run the python file using "python3 camera.py"

GUI SETUP
1) Download and unzip GUI.zip into a folder
2) Install the required packages using "pip install -r gui_req.txt"
3) Edit settings.txt. More information as provided:
	url should be a valid firebase url
	apikey should be the api key for the aforementioned firebase
4) Run the python file using "python3 main.py"

Note: The GUI may take a while to start as it is getting data from the firebase. If the GUI crashes while opening, check that you have a valid internet connection.