#22_10_2024

# Logic operators

# AND
`and a,b`
`a & b`
performs and operation on each pair of bits `(a, b)`
## And operation
1 if both bits are 1
0 otherwise

# OR
`or a,b`
`a | b`
performs or operation on each pair of bits `(a, b)`
## Or operation
1 if one of the bits is 1
0 otherwise

# XOR
`nand a,b`
`a ^ b`
performs xor operation on each pair of bits `(a, b)`
## Xor operation
1 if the bits are distinct
0 otherwise

# Shifting
Fast AsFuuuk 
Shifts all bits to the desired location
! the bits that are overflowing are going to be erased

## SHL
shifts to the left x times

`shl $op1, $number_of_times`
`$op1 << $number_of_times`
`shl $register, $number_of_times or CL ;CL the register`

## SHR
shifts to the right x times

`shr $op1, $number_of_times`
`$op1 >> $number_of_times`
`shr $register, $number_of_times or CL ;CL the register`

## SAL, SAR
SHL and SHR but keeps the sign interpretation
(it fills the empty spaces with the sign bit)
```
SAL 10001110b, 4
; sign bit was one 
; we shift to the left 4 times
; 1110xxxx
; we fill x with sign_bit
; 11101111
```

# Rotations
permutations

## ROL
rotate Left

## ROR
rotate right

## RCR
rotate with carry right

## RCL
rotate with carry right




# TEST
`test, a, b`
And operator without memorization
Used for changing flags

# Tips and tricks

## Masking
Using the and operator, you can create a mask of form 000000100010b you can get the bits that are on the positions that contain 1 in the mask

### Example
``` asm
; we want to get the bits on position 3 and 4 
mov AX, [a] & 00001100b 
```
## Getting 0xFF.. of unknown size
``` asm
or EAX, -1
; or
or EAX, 0xffffffff
```
## Resetting a register
sometimes it can be faster to reset a register with the xor operator
```
xor EAX, EAX
; EAX is now 0
```

