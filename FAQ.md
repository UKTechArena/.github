## Frequently Asked Questions

## Participating
1. What skills I need to be able to solve the challenge?

In order to participate, you only need to be competent in C++ and/or Python programming language and
a good level of understanding of how 3D geometry data is represented and how a correlated data can be
compressed and decompressed.

2. Do I have to be familiar with gltf/obj data?

A familiarity with gltf/obj file format would be an added advantage and will help you to develop a
good solution for this competition.
Here are few reference materials that would help to improve your understanding
glTF Tutorial
https://github.khronos.org/glTF-Tutorials/gltfTutorial/gltfTutorial_009_Meshes.html
glTF Specification
https://registry.khronos.org/glTF/specs/2.0/glTF-2.0.html#reference-mesh-primitive
OBJ FILE FORMAT
https://www.cs.cmu.edu/~mbz/personal/graphics/obj.html

3. Do I need to form a team to participate?

Yes, you have to form a team of at least 2 and maximum of 4 to be part of this competition.
We value a team work and would like to see more participants working together.
## Understanding the problem and working with input output datasets
1. How would I make sure that my understanding of the problem is correct?

The best way to ensure that you understand the problem correctly is to post on the task forum QA section.
Other participants will confirm or comment on your problem statement and the mentors from Huawei will
confirm or correct any misunderstanding.

2. What programing language, tech stack or libraries should I use?

We recommend using C++ and/or Python programming language but any language and libraries can be used as
long you can make it to work on fixed testing AWS cloud platform.
## Code submission, scoring & leader board
1. How frequently can I submit my solution for scoring?

You can submit your solution as often as you like. You can also run the test script locally to calculate your score, however the score will not be submitted if you run it locally.

2. Why am I getting a negative compression score?

We calculate the compression score based on the input and output file sizes. If your output files are bigger than your input files on average then you will get a negative value for this component of the score.

3. Why am I getting a negative time score?

We calculate the decompression score based on a maximum decompression time of 1 second. If your solution takes more than 1 second on average to decompress the sample models you will get a negative value for this component of the score.

4. Why is the image quality calculation failing?

This can happen for a number of reasons but most likely either you are missing some dependencies or there is no GPU available to render the images.
