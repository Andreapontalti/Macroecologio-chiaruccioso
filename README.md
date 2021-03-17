# Nuovo-repositorio
> install.packages("raster")
Warning in install.packages("raster") :
  'lib = "C:/Program Files/R/R-4.0.4/library"' is not writable
--- Please select a CRAN mirror for use in this session ---
also installing the dependencies ‘sp’, ‘Rcpp’

provo con l'URL 'https://cran.stat.unipd.it/bin/windows/contrib/4.0/sp_1.4-5.zip'
Content type 'application/zip' length 1821327 bytes (1.7 MB)
downloaded 1.7 MB

provo con l'URL 'https://cran.stat.unipd.it/bin/windows/contrib/4.0/Rcpp_1.0.6.zip'
Content type 'application/zip' length 3253393 bytes (3.1 MB)
downloaded 3.1 MB

provo con l'URL 'https://cran.stat.unipd.it/bin/windows/contrib/4.0/raster_3.4-5.zip'
Content type 'application/zip' length 3558622 bytes (3.4 MB)
downloaded 3.4 MB

package ‘sp’ successfully unpacked and MD5 sums checked
package ‘Rcpp’ successfully unpacked and MD5 sums checked
package ‘raster’ successfully unpacked and MD5 sums checked

The downloaded binary packages are in
        C:\Users\andrea pontalti\AppData\Local\Temp\RtmpuI7iSW\downloaded_packages
> library(raster)
Carico il pacchetto richiesto: sp
> setwd("C:/lab/")
Error in setwd("C:/lab/") : non posso cambiare la directory di lavoro
> setwd("C:/lab/")
> brick
standardGeneric for "brick" defined from package "raster"

function (x, ...) 
standardGeneric("brick")
<bytecode: 0x000000000d086b30>
<environment: 0x0000000009e10a90>
Methods may be defined for arguments: x
Use  showMethods("brick")  for currently available ones.
> brick("p224r63_2011_masked.grd")
class      : RasterBrick 
dimensions : 1499, 2967, 4447533, 7  (nrow, ncol, ncell, nlayers)
resolution : 30, 30  (x, y)
extent     : 579765, 668775, -522705, -477735  (xmin, xmax, ymin, ymax)
crs        : +proj=utm +zone=22 +datum=WGS84 +units=m +no_defs 
source     : C:/lab/p224r63_2011_masked.grd 
names      :       B1_sre,       B2_sre,       B3_sre,       B4_sre,       B5_sre,        B6_bt,       B7_sre 
min values : 0.000000e+00, 0.000000e+00, 0.000000e+00, 1.196277e-02, 4.116526e-03, 2.951000e+02, 0.000000e+00 
max values :    0.1249041,    0.2563655,    0.2591587,    0.5592193,    0.4894984,  305.2000000,    0.3692634 

> p224r63_2011 <- brick("p224r63_2011_masked.grd")
> p224r63_2011
class      : RasterBrick 
dimensions : 1499, 2967, 4447533, 7  (nrow, ncol, ncell, nlayers)
resolution : 30, 30  (x, y)
extent     : 579765, 668775, -522705, -477735  (xmin, xmax, ymin, ymax)
crs        : +proj=utm +zone=22 +datum=WGS84 +units=m +no_defs 
source     : C:/lab/p224r63_2011_masked.grd 
names      :       B1_sre,       B2_sre,       B3_sre,       B4_sre,       B5_sre,        B6_bt,       B7_sre 
min values : 0.000000e+00, 0.000000e+00, 0.000000e+00, 1.196277e-02, 4.116526e-03, 2.951000e+02, 0.000000e+00 
max values :    0.1249041,    0.2563655,    0.2591587,    0.5592193,    0.4894984,  305.2000000,    0.3692634 

> plot(p224r63_2011)
>  plot(p224r63_2011)
> cl <- colorRampPalette(c("black", "grey", "light grey"))(100)
> plot(p224r63_2011, col=cl)
> > cl <- colorRampPalette(c("black", "grey", "light grey"))(100)
Errore: unexpected '>' in ">"
> > plot(p224r63_2011, col=cl)
Errore: unexpected '>' in ">"
> cl <- colorRampPalette(c("blue","magenta","red","yellow" "green", "light grey"))(100)
Errore: unexpected string constant in "cl <- colorRampPalette(c("blue","magenta","red","yellow" "green""
>  cl <- colorRampPalette(c("blue","magenta","red","yellow", "green", "light grey"))(100)
> > plot(p224r63_2011, col=cl)
Errore: unexpected '>' in ">"
> plot(p224r63_2011, col=cl)
> cl <- colorRampPalette(c("blue","magenta","red","yellow", "green", "light grey","light blue","dark green", "black","white","light green"))(100)
> plot(p224r63_2011, col=cl)
> save.image("C:\\lab\\Prova1")
> 
