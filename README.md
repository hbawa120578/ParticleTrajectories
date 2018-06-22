# MSDfromMultipleTrajectories

`@author: HarinderB`

a simple script to determine Mean-Squared Displacements (MSD) from multiple particle trajectories

a part of the MSD code 
`

**args are as follows: directory, number of files (trajectories), dimensions, smallest time-step, timeCMSD = 1000 (pts to consider))**

`msddata,stddata = msd.main()`

`msdplot = plt.plot(msddata)`

`plt.show(msdplot)`

`grad = np.polyfit(range(1,101),msddata[1:101], 1)[0] # using the first 100 values for computing gradient`

`print 'the effective diffusion coefficient is : ' + str(grad/(6*1e-6)) + ' um^2/sec' # effective diffusion coefficient`
`
