## Frequently Asked Questions

### Why am I getting a negative compression score?

We calculate the compression score based on the input and output file sizes. If your output files are bigger than your input files on average then you will get a negative value for this component of the score.

### Why am I getting a negative time score?

We calculate the decompression score based on a maximum decompression time of 1 second. If your solution takes more than 1 second on average to decompress the sample models you will get a negative value for this component of the score.

### Why is the image quality calculation failing?

This can happen for a number of reasons but most likely either you are missing some dependencies or there is no GPU available to render the images.
