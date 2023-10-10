cmake_minimum_required(VERSION 3.25)

execute_process(
        COMMAND clang -o executable main.c -Xpreprocessor -fopenmp -L/opt/homebrew/Cellar/libomp/17.0.2/lib -lomp  -I/opt/homebrew/Cellar/libomp/17.0.2/include/
        COMMAND ./executable
)
