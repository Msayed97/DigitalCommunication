# Digital Communication 

# project about the performance simulation of different modulation schemes

-in this project we will try BPSK , QPSK , QAM (16-64) , FSK

- __instructions to reproduce scater plot :__
	 1. Open Matlab then open simulink 
	 2. Open a new Model and add needed blocks (random integer generator , modulator , demodulator , AWGN channel      , constellatoin diagrams , diplay block  )
	 3. set inital seed in random integer
	 4. set Eb/No = 10 in AWGN channel
	 5. connect all blocks together and connect the constellation diagrams just after and before the            AWGN channel 
	 6. run the simulatoin
- __instructions to reproduce BER :__
	 1. Add block simout and rename it  
	 2. change the Eb/No in AWGN channel to the name of simout
	 3. save model then open bertool from matlap command section
	 4. change Eb/No to -10:10 in theoretical tab
	 5. change Eb/No to -10:1:10 and chose your file  in carlo tab
	 6. then press run 
	 	
## BPSK

-Binary phase-shift keying , It uses two phases which are separated by 180° and so can also be termed 2-PSK.It is  the most robust of all the PSKs But it's, however, only able to modulate at 1 bit/symbol and so is unsuitable for high data-rate applications.

- __Extra instructions :__
	- set size to 2 in random integer generator

### - Figures:

* #### Scatter plot Before Noise

	![without RCF](/BPSK/BPSKBefore.png)
    
    
* #### Scatter plot After Noise

	![without RCF](/BPSK/BPSKAfter.png) 
    
* #### BER performance figure
	
    ![BERvsSNR](/BPSK/BER.jpg)

	
## QPSK

Quadrature Phase Shift Keying (QPSK) is a form of Phase Shift Keying in which two bits are modulated at once, selecting one of four possible carrier phase shifts (0, 90, 180, or 270 degrees). QPSK allows the signal to carry twice as much information as ordinary PSK using the same bandwidth

- __Extra instructions:__
	- set size to 4 in random integer generator

### - Figures:

* #### Scatter plot Before Noise
   
	![without RCF](/QPSK/QPSKBefore.png) 
    
* #### Scatter plot After Noise
	
	![without RCF](/QPSK/QPSKAfter.png) 
    
* #### BER performance figure
	
    ![BERvsSNR](/QPSK/BER.jpg)
	
## FSK

Frequency-shift keying (FSK) is a frequency modulation scheme in which digital information is transmitted through discrete frequency changes of a carrier signal.

- __Extra instructions :__
	- set size to 2 in random integer generator

### - Figures:

* #### Scatter plot Before Noise
	
	![without RCF](/FSK/FSKBefore.png) 
    
    
* #### Scatter plot After Noise
	
    ![with RCF](/FSK/FSKAfter.png) 
    
* #### BER performance figure
	
    ![BERvsSNR](/FSK/BER.jpg)

	
## QAM 16

Quadrature Amplitude Modulation) A modulation technique that employs both phase modulation (PM) and amplitude modulation (AM). Widely used to transmit digital signals such as digital cable TV and cable Internet service.QAM 16 used 4 bits

- __Extra instructions :__
	- set size to 16 in random integer generator

### - Figures:

* #### Scatter plot Before Noise
	
    ![with RCF](/QAM16/QAM16Before.png) 
    
* #### Scatter plot After Noise
    
    ![with RCF](/QAM16/QAM16After.png) 
    
* #### BER performance figure
	
    ![BERvsSNR](/QAM16/BER.jpg)
	
## QAM 64

-same as QAM 16  the difference is that it use 6 bits instead of 4 .

- __Extra instructions to reproduce the figures:__
	- set size to 64 in random integer generator

### - Figures:

* #### Scatter plot Before Noise
	
    ![with RCF](/QAM64/QAM64Before.png) 
    
* #### Scatter plot After Noise
	
    ![with RCF](/QAM64/QAM64After.png) 
    
* #### BER performance figure
	
    ![BERvsSNR](/QAM64/BER.jpg)