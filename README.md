Download link : https://programming.engineering/product/com-sgn-110-exercise-2/

COM-SGN.110 EXERCISE 2
The tasks should be completed and presented to TA during the lab session. Do not forget to upload your solutions to Moodle! Questions about exercises should be addressed to the TA personally, through Moodle messages or via email, which can be found on the Moodle page of the course.

    Familiarization with MATLAB’s Quantization Functions

        Check help quant and help quantiz.

        Create vector A with numbers 0 … 255.

        Run the following MATLAB codes:

step = 256/4;

QA1 = quant(A, step);

partition = step:step:256-step; codebook = step/2:step:256-step/2; [indx,QA2] = quantiz(A, partition, codebook);

Explain what each line of the code does and what the results mean.

        Find out the values in quantized vectors QA1 and QA2 (Hint: help unique).

    Quantization

        Load the image lena_face.png (it is included with MATLAB) as matrix I.

        Using quantiz function, design 128, 64, 32, 16, 8 and 4-level uniform quantizers and quantize the gray-level image lena_face.png. (Hint: reshape)

        Try to use noise (add noise to the image before the quantization, help randn) to reduce the contouring effects. Quantize again lena_face.png to 16 levels and compare the result with the noiseless image quantized to 16 levels.

    Simultaneous Contrast

Using MATLAB, generate two 8-bit images as in the Figure 1, where the small squares have gray level values of 127 and the backgrounds have the values 63 and 223. (Size of the large square is 400×400 and the small is 160×160 pixels.) Verify the simultaneous contrast: the small squares in the middle have equal luminance but do not appear equally bright. Next, change the gray level in one of the small squares until the small squares will appear equally bright. What is the value of the obtained gray level?

(Hint: help ones, imshow. Avoid using for loops).
