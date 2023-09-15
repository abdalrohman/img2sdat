# img2sdat

This Python script converts a system image into a new.dat format. It uses the SparseImage class to create a sparse image from the input system image, and then computes the block image difference between the sparse image and an empty image. The block image difference is then written to an output file.

# Usage

You can run this script from the command line using the following syntax:

    python img2sdat.py <image> [-c cachesize] [-o outdir] [-v version] [-p prefix]

Here’s what each argument does:

    image: This is the path to the input system image. This argument is required.
    -c or --cachesize: This sets the cache size. The default value is 402653184.
    -o or --outdir: This sets the output directory. If not specified, the current directory will be used.
    -v or --version: This sets the transfer list version number. The default value is 4.
    -p or --prefix: This sets the name of the image (prefix.new.dat). The default value is “system”.

For example, if you have a system image named “system.img” in your current directory, you can convert it into a new.dat format using the default settings with this command:

    python img2sdat.py system.img
