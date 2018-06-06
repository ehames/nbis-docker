# nbis-docker
Docker image for NIST Biometric Image Software (NBIS)

## About
This project packages the [NIST Biometric Image Software](https://www.nist.gov/services-resources/software/nist-biometric-image-software-nbis) in a Docker image.

Libraries and binaries are installed in `/opt/nist`. To build your own programs, you need to add to add the following variables to your build systems:

`CFLAGS: -I/opt/nist/include`

`LDFLAGS: -L/opt/nist/lib -lwsq -lcblas -lpca -lf2c -lfft -limage -ljpegb -lmindtct -lnfiq -lpca -lutil -lbozorth3 -lclapck -lfet -lihead -lioutil -ljpegl -lmlp -lnfseg -lpcautil  -lutil -lm`

