# ParseExp
	A class used to parse a String into a mathematical expression.

	ParseExp(String exp)
		Initializes a ParseExp object with the string exp.

	double evaluate()
		Parses the string which the ParseExp object was initiallized 
		with. If the string contains "=", calls equate.

	double evaluate(String exp)
		Parses the string passed to the function. If the string contains "=", calls equate.

	double equate()
		Parses the equation with which the ParseExp object was initialized with.
		Return 1 if true and 0 if false.	

	double equate(String exp)
		Parses the equation passed to the function.
		Return 1 if true and 0 if false.
			
	double nextNum()
		Returns the next number in the expression. Throws ParseException
		if no number is found. Use hasNextNum to avoid this.

	boolean hasNextNum()
		Returns true if there is another number in the expression, false
		otherwise.

	double nextOp()
		Returns the next operation in the experssion. Throws ParseException
		if no operation is found. Use hasNextOp to avoid this.	

	boolean hasNextOp()
		Returns true if there is another operation in the expression, false
		otherwise.

	String getExp()
		Returns the original expression as a String.	

# ParseFn
	A class used to parse a String into a mathematical function.
	Character in the range a..z are acceptable variable names.

	ParseFn(String fn) throws ParseExption
		Initializes a ParseFn object with the string fn

	String defVar(char[] var, double[] values) throws ParseException
		Assigns the vars to specified values.
		returns "" if some vars aren't assigned yet