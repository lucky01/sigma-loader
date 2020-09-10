# sigma-loader

Load SigmaStudio project to your ADAU1401/1701 through i2c.

1. Verify the address in sigma_loader.c here: (default 0x34)

char *i2c[] = {"dsp", "i2c", "/dev/i2c-1", "0x34"};

2. compile the code executing make

3. Export the project from SigmaStudio 

4. Take the xml file (not the NetList)

5. Execute the command ./sigma_loader myprogram.xml

6. Your DSP should be running the uploaded code

NB: the DSP has to be in self boot mode