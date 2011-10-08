# SlowSHA

This single-file module implements the hashing algorithms
sha1, sha224, sha256, sha384, and sha512 in pure Python.
The code doesn't contain too many optimisations,
which makes it fairly easy to read.

Note that this code is for educational purposes.
Python's native C implementation of SHA1/SHA2
is much faster and better tested.

## Usage

    >>> import slowsha
    >>> slowsha.sha224(b"Python 3000").hexdigest()
    'ca10838d71bcd91cfc3e474867a5ed2f13feb14ee91a6dab2526a96b'
    >>> slowsha.sha1(b"hello").digest()
    b'\xaa\xf4\xc6\x1d\xdc\xc5\xe8\xa2\xda\xbe\xde\x0f;H,\xd9\xae\xa9CM'
    >>> slowsha.sha224(b"Hello World")
    <slowsha.SHA224 object at 0xb742262c>
