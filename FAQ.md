# Frequently Asked Questions

## Participating

**1. What skills I need to be able to solve the challenge?**

In order to participate, you only need to be competent in C++ and/or Python programming language and
a good level of understanding of how 3D geometry data is represented and how a correlated data can be
compressed and decompressed.

**2. Do I have to be familiar with gltf/obj data?**

A familiarity with gltf/obj file format would be an added advantage and will help you to develop a
good solution for this competition.
Here are few reference materials that would help to improve your understanding:

[glTF Tutorial](https://github.khronos.org/glTF-Tutorials/gltfTutorial/gltfTutorial_009_Meshes.html)

[glTF Specification](https://registry.khronos.org/glTF/specs/2.0/glTF-2.0.html#reference-mesh-primitive)

[OBJ File Format](https://www.cs.cmu.edu/~mbz/personal/graphics/obj.html)

**3. Do I need to form a team to participate?**

Yes, you have to form a team of at least 2 and maximum of 4 to be part of this competition.
We value a team work and would like to see more participants working together.
## Understanding the problem and working with input output datasets

**1. How would I make sure that my understanding of the problem is correct?**

The best way to ensure that you understand the problem correctly is to post on the task forum QA section.
Other participants will confirm or comment on your problem statement and the mentors from Huawei will
confirm or correct any misunderstanding.

**2. What programing language should I use?**

We recommend using C++ and/or Python programming language but any languages can be used as
long you can make it to work on fixed testing AWS cloud platform.

**3. Are external libraries such as Draco allowed in the submissions? Draco example gets a score of ~65.5/80**

This challenge expects you to innovate and develop core part of compression and decompression algorithm.
External libraries for core part of compression and decompression algorithm are **not allowed** including Draco, zlib/zstd, etc.
Draco is just for reference (~65.5/80).

**4. Are there any requirements for file formats after compression? AI and non-AI examples writes .gltf file formats after compression while the Draco example just uses .drc. If any file format is allowed after compression or are there required formats?**

There are file format requirement **due to limitation of automatic evaluation framework**, 

It expects:
- input and decoded file format needs to be .obj or .gltf
- input and encoded file format should contain the same information along side original and compressed geometry data respectively, to be able to calculate the compression ratio correctly.

## Code submission, scoring & leader board

**1. How frequently can I submit my solution for scoring?**

You can submit your solution as often as you like. You can also run the test script locally to calculate your score, however the score will not be submitted if you run it locally.

**2. Why am I getting a negative compression score?**

We calculate the compression score based on the input and output file sizes. If your output files are bigger than your input files on average then you will get a negative value for this component of the score.

**3. Why am I getting a negative time score?**

We calculate the decompression score based on a maximum decompression time of 1 second. If your solution takes more than 1 second on average to decompress the sample models you will get a negative value for this component of the score.

**4. Why is the image quality calculation failing?**

This can happen for a number of reasons but most likely either you are missing some dependencies or there is no GPU available to render the images.

**5. I want to ask are we just going to compress the .obj file?**

.obj file can contain a lot of info, not just the geometry or the mesh information but it can contain or appoint to other files like materials or other information.
So, what we are interested in is focusing on just compressing the mesh or the geometry part, not the whole file itself.

**6. I also had an issue with jq not working on windows**

You can try using WSL on windows to work with all the Linux tools if you are just using windows environment on your local system. The jq can work on WSL, or windows system on Linux so you should be able to use that. If not, then you might have to modify an equivalent Json working script to work through the JSON file.

**7. How much do the contest value on the originality and creativity?**

We value and encourage students to be original and creative for core part of Compression/Decompression Algorithm design.
We strongly discourage copying other external solutions for core part of Compression/Decompression Algorithm design.
We highly encourage solutions to be novel, performant and good quality.
