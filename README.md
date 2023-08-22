# OEISGenerator

[![Build Status](https://github.com/frakt0x90/OEISGenerator.jl/actions/workflows/CI.yml/badge.svg?branch=main)](https://github.com/frakt0x90/OEISGenerator.jl/actions/workflows/CI.yml?query=branch%3Amain)

# Usage

Generator produces a lazy iterator that you can then take() elements from

```julia
using OEISGenerator

generator = Generator("A000001")
first_ten = take(generator, 10)
```

Each sequence is also exported as a function so you can just grab values you need:

```julia
tenth_element = A000001(10)
```