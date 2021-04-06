# DOA_Experiments
Setup to perform DOA experiments using a FMCOMM-S5 board along with a Xilinx Zync 702 setup. 
# First make sure you have all dependencies - pyadi, libiio, and their respective python bindings
https://analogdevicesinc.github.io/pyadi-iio/guides/quick.html#install-checks<br/>
https://github.com/analogdevicesinc/libiio

# Setup - 

FMCOMMs5 allows up to 6 GHz of testing. First connect loopback cables and perform MCS sync. Verify this by the GUI, and use a little bit of offset in the reciever phase to synchronise all the channels. <br/>

Make sure you have access to the board by pinging and if so, proceed by executing saverx.py to recieve samples and save them into a csv file. Change the parameters as required. <br/>

After file is saved, open it up in MATLAB  and import it as a numeric matrix.(default type is table). Run the music script. 

#Future work - 

Streamline entire process as one script.<br/>
Include measurements to calibarate the array performance.<br/>



