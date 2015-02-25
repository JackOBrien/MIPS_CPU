############################################################################
# 
# A simple (and incomplete) demonstration of one you might test lw and
#  sw.  (Make sure lui and other basic arithematic works first!)
#
# When writing your own tests, make sure you test non-zero offsets.
# Also, make sure your test will detect any timing errors (i.e., a
# clock cycle that is too short).
#
###########################################################################

	.data
val1:	1983
val2:	2007

	.text

	# Remember, this is a pseudo instruction!
	lw $16, val1
	lw $17, val2

	addi $16, $16, 17

	# store the value in val2 (remember, this is a pseduo instruction)
	sw   $16, val2

	# load the address of val2 into $18
	la   $18, val2  
	# store the value in the slot after val2
	sw   $16, 4($18)
