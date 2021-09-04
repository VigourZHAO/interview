

import base64


res = 11111111111

a = 'zpx' + str(res)


def encode_method(arg):
    res = base64.b64encode(arg.encode('utf-8'))
    base64_str = str(res, 'utf-8')

    return base64_str[:len(base64_str) - 1] + base64_str[3:9]


def decode_method(arg):
    base64_str = arg[:len(arg) - 6] + '='
    res = base64.b64decode(base64_str)
    result = str(res, 'utf-8')
    return result


if __name__ == '__main__':
    vvv = encode_method(a)
    rrr = decode_method(vvv)
    print(vvv)

    # print(base64.b64encode(a.encode('utf-8')))
    print(rrr)


Output = """
enB4MTExMTExMTExMTE4MTExM
zpx11111111111
"""
