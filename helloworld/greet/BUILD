# Copyright 2020 Pants project contributors.
# Licensed under the Apache License, Version 2.0 (see LICENSE).


python_library(
    # name defaults to the name of this directory, i.e., `greet`.
    # sources defaults to ['*.py', '!*_test.py', '!test_*.py', '!conftest.py'].
    dependencies = [
        "//:translate",
        ":greetings",
        "helloworld/util"
    ],
    compatibility = ">=3.6",
)


python_tests(
    name = 'tests',
    # sources defaults to ['*_test.py', 'test_*.py', 'conftest.py'].
    dependencies = [
        ":greet"
    ]
)


resources(
    name = 'greetings',
    sources = ['greetings.txt'],
)
