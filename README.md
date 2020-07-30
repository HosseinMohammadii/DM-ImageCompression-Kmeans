# DM-ImageCompression-Kmeans

We	will	use	self-written KMeans	code	for	a	useful	real-world	problem.	
In	many	RGB	encodings	each	pixel	is	represented	by	24	bits,	8	bits	for	each	one	of	the	main	
colors	(Red,	Green,	Blue)	ranging	from	0	to	255,	and	therefore	each	pixel	can	have	more	than	
16	million	colors.	
In	this	part,	We	will	use	K-means	algorithm	to	reduce	the	number	of	colors	to	16	(or	256)	so	
that	the	color	of	each	pixel	can	be	represented	by	only	4	bits	(or	8	bits).	In	fact,	we	only	need	
to	store	the	RGB	values	of	the	16	(or	256)	selected	colors	in	an	array,	and	for	each	pixel	in	the	
image	we	now	need	to	only	store	the	index	of	the	color	in	the	array.	Since	reducing	the	
number	of	the	colors	result	in	lower	quality	for	the	image,	we	use	K-means	to	find	the	16	(or	
256)	colors	that	best	group	pixels	in	the	image.


![Sample result](https://github.com/HosseinMohammadii/DM-ImageCompression-Kmeans/blob/master/sample-result.png)


The	original	image	has	800x800	pixels	and	with	24	bits	per	pixel	the	image	requires	at	least	
800x800x24	bits	to	be	stored.	By	reducing	the	number	of	colors	to	16	and	256	the	image	only	
requires	about	800x800x4	and	800x800x8	bits	respectively	to	be	stored.	
By	this	point	hopefully	you	have	learnt	the	intuition	behind	the	clustering	and	grasped	a	hands-
on	knowledge	on	how	to	use	clustering	for	real	world	challenges.		

# To see code result please open jupyter file
![jupyter file](https://github.com/HosseinMohammadii/DM-ImageCompression-Kmeans/blob/master/kmeans-image-compression.ipynb)

# For more explanations please read report file image compression section
![Report](https://github.com/HosseinMohammadii/DM-ImageCompression-Kmeans/blob/master/HosseinMohammadi_Report.pdf)
