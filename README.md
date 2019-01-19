# YAMF-TLV

> Yet-Another-Multi-Format - Type-Length-Value

Yamf-tlv is a binary encoding for [type-length-value](https://en.wikipedia.org/wiki/Type-length-value). The type is an unsigned 64 bit integer, the value can have a length of up to 2^64 - 1 bytes.

The binary encoding is defined as the concatenation of:

- the type, encoded as a [VarU64](https://github.com/AljoschaMeyer/varu64)
- the length of the value, encoded as a [VarU64](https://github.com/AljoschaMeyer/varu64)
- the value itself

That's it. There's nothing fancy here, it just needs to be defined somewhere.
