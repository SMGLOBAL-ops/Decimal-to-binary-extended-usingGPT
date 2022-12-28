def decimal_to_binary(w):
    b = []

    if w == 0:
        return '0'
    else:
        while w > 0:
            if w % 2 != 0:
                b.insert(0, 1)
                w = (w - 1) / 2
            elif w % 2 == 0:
                b.insert(0, 0)
                w = w / 2

            if w == 0:
                return ''.join(map(str, b))
            else:
                continue

def binary_to_int(binary):
    # convert the binary string to a list of integers
    binary = [int(c) for c in binary]

    # initialize the result to zero
    result = 0

    # iterate over the binary list in reverse order
    for i in range(len(binary) - 1, -1, -1):
        # add 2^i * binary[i] to the result
        result += 2**i * binary[i]

    return result

for i in range(0, 16):
    print(f'For value, {i}, binary equivalent is: ')
    binary = decimal_to_binary(i)
    print(binary)
    print(f'And the integer equivalent is: {binary_to_int(binary)}')
