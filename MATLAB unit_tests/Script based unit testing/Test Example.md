
In one folder there are two files:
- function with name `my_super_function.m`
- script named `super_test.m`

`my_super_function.m` file contains the following code:
```
function outputArg = my_super_function(inputArg1,inputArg2)

    %MY_SUPER_FUNCTION Summary of this function goes here
    %   Detailed explanation goes here
    outputArg1 = inputArg1;
    outputArg2 = inputArg2;
    outputArg = outputArg1 + outputArg2;
    
end
```

`super_test.m` file contains the following code:
```
x1 = int64('a');
x2 = int64('b');

%% Test1 - the test one name
assert(3 == my_super_function(1, 2));

%% Test2 - the test two name
assert(x1 + x2 == my_super_function('a', 'b'))
```

After running the `runtests` command in console we get the test output:
```
Running super_test
..
Done super_test
__________


ans = 

  1×2 TestResult array with properties:

    Name
    Passed
    Failed
    Incomplete
    Duration
    Details

Totals:
   2 Passed, 0 Failed, 0 Incomplete.
   0.01639 seconds testing time.
```

