##RDMPWD

#INSTALLATION INSTRUCTIONS
===============================================================================

  1. Open terminal

  2. Type:

       ls  		#This will show the files listed in the present directory.
			 If rdmpwd is not visible, navigate to the Downloads folder.

  3. Once, the file is visible, type:
	sudo cp rdmpwd /usr/bin/[optional]	 #enter a shortname for the service
	 				    	generator, rdmpwd will be set by default

  4. Execute the command, if the output shows command not found, type:
	sudo chmod +x /usr/bin/rdmpwd 	#change rdmpwd if a different was 
						given at the time of installation

  

#USAGE INSTRUCTIONS
===============================================================================

  The serivce generator works on terminal user interface, 
and flags are used for taking inputs.
  For now, there are two flags 
	1. Username(-u)
	2. Passwordlogic(-p)


command example:
	sudo rdmpwd -u "user1" -p '$hour ** 2 + $minute * 3'
	with the above command the password for the user at 06:15 will be 81 and
	 the password at 07:59 will be 226
	

	Note: The allowed time variables are $year, $month, $day, $hour, $minute,
		 $second
		And the allowed operations are addition(+), subtraction(-), 
		multiplication(*), division(/), exponentiation(**)
