# pointeroverflowctf - Exploit 200 "Overrun and Outdone"
## Table of Contents
- [Introduction](#introduction)
- [Code Analysis](#code-analysis)
- [Exploit Development](#exploit-development)
- [Usage](#usage)
- [Results](#results)
- [Conclusion](#conclusion)
- [References](#references)

## Introduction
<div align="center">
![challenge](images/exploit_200.png)
</div>
The User Record application has a buffer overflow vulnerability due to improper handling of user input. The `name` field in the `user_record` struct has a fixed size, which allows for an overflow when a longer string is provided. This exploit demonstrates how to manipulate the memory layout to change the `id` variable.

