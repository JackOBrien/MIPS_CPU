####################################################################
#
# This program does simple multiplication.  It will (partially) test
# bne and j; however, you will want verify that your branch and jump
# instructions work before running this test.  (If they don't work,
# this script will probably enter an infinite loop.)
#
###################################################################
	
# set up registers with the two multipliers and the product
	addi $16, $0, 15	# i0  $16 = 15
	addi $17, $0, 10	# i1  $17 = 10
	and  $18, $0, $0	# i2  $18 = 0 

# if the first multiplier is 0, then there is nothing to do
	beq  $16, $0, END	# i3

# add the second multipler to the product, then decrement the first
# multiplier by 1, until it reaches 0.
TOP:	add  $18, $18, $17      # i4  $18 += $17
	addi $16, $16, -1       # i5  $16--
	# Once the first multipler reaches 0, we're done.
	beq  $16, $0, END       # i6
	j    TOP      		# i7

# We're done.  The extra lines are just to make sure the final jump
# goes to the right place.
END:   addi $19, $19, 70	# i8
       addi $20, $20, 80	# i9
       addi $21, $21, 90	# i10  
