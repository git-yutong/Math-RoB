# Math-RoB

A dataset for evaluating the reasoning robustness of large language models.

## math500
This dataset is taken from Hugging Face: `HuggingFaceH4/MATH-500`.

## newmath500
Three questions are combined into different triplets, and the model is instructed to answer **only the first**, **only the second**, or **only the third** question.

## selected_math_define_operation_real
The original problems in Math500 are modified to create new and still valid mathematical questions.

## selected_math_define_operation
A prompt that defines custom operators is added before the original question.

## selected_math_define_operation_1shot
Based on `selected_math_define_operation`, a one-shot example prompt is further added.

## selected_math_define_operation_control
As a control experiment, some numbers used for mathematical calculation in the original questions are deleted or forcibly changed, in order to test the model's instruction-following ability when the input is inconsistent with training-style samples.

## selected_math_define_operation_replace_numbers
Some numbers in the original questions are replaced with Greek letters, and a prompt is added at the beginning to explain how to substitute them back.

## selected_math_delete_crucial_data
Some crucial numbers in the Math500 dataset are removed, making the problems unsolvable. This setting is designed to test whether the model hallucinates answers when key information is missing.
