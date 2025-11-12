# address
The Qoin address type defines multiple address types within the Post-Quantum Qoin network.

## Install

Install this library with `go mod`

## Usage

Addresses support various types of encoding formats and have constructors
for each format

```golang
// address from ID
idAddress := NewIDAddress(id)
```

Serialization

```golang
var outBuf io.writer
err := address.MarshalCBOR(outbuf)
var inBuf io.reader
err := address.UnmarshalCBOR(inbuf)
```
