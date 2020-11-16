# mymath
A free and open source advanced calculator

USAGE:
=====
		This is a simple math solver that takes a sring as a input and procees it and give the float output.
	This the argument string can contain numeric digits and operators like addition, subtraction, multipliction, 
	division and power(^ operator for power)
		This does the same work as eval function but the difference is this allows partial braces.
	This does not need any extra python packages

NOTE:
=====
	The argument string should not contain any alphabets otherwise this will return "Invalid Syntax"

EXAMPLES:
=========
	sample_program:
	_______________
		import mymath # importing mymath library
		print(mymath.calc('67'))
		# The above will return 67 as there is no operators

		print(mymath.calc('56+67'))
		# the above will return 123 

		print(mymath.calc('56*(5+6)'))
		# you can change the priority of operations using braces 
		# without braces the priority for operations is power > divide > multiply > addition and subtraction

		print(mymath.calc('67)(78'))
		# the above operation will give no error message and it returns 5226
		# even '67)7' can also be processed 
