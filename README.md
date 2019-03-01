# ltcaddressgenie
A standalone Litecoin keypair/address generator, written in Go.

# ltcaddressgenie

## Disclaimer

**This project was written in May 2013 for educational purposes.**

**Modern cryptocurrency wallets should use hierarchical deterministic (HD) keys instead.**

## Introduction

ltcaddressgenie is a standalone litecoin keypair/address generator written in Go.
ltcaddressgenie generates an ECDSA secp256k1 keypair, dumps the public key in
compressed and uncompressed litecoin address, hexadecimal, and base64 formats,
and dumps the private key in Wallet Import Format (WIF), Wallet Import Format
Compressed (WIFC), hexadecimal, and base64 formats.

ltcaddressgenie includes a lightweight Go package called btckey to easily generate
keypairs, and convert them between compressed and uncompressed varieties of
litecoin Address, Wallet Import Format, and raw bytes.


Donations are welcome at `LT3kw2fnpR2SZF2jCwBaKEmCgKzpR22xfx` :-)

## Usage

#### Generating a new keypair

    $ ltcaddressgenie
Litecoin Address (Compressed)        LT3kw2fnpR2SZF2jCwBaKEmCgKzpR22xfx
Public Key Bytes (Compressed)        02932A12D91791231F50D451627E80A8210D72560531E11D974D10208B29C33C03
Public Key Base64 (Compressed)       ApMqEtkXkSMfUNRRYn6AqCENclYFMeEdl00QIIspwzwD

Litecoin Address (Uncompressed)      LPqUN7bssBQQqEjcK2ovmjQmy9FNM65zUM
Public Key Bytes (Uncompressed)      04932A12D91791231F50D451627E80A8210D72560531E11D974D10208B29C33C0
                                     3A6CCBF2512B0FC2429C3A14BDED0E0FFA33E6A8B5B9C86DEF15F799F00AC9124
Public Key Base64 (Uncompressed)     BJMqEtkXkSMfUNRRYn6AqCENclYFMeEdl00QIIspwzwDpsy/JRKw/CQpw6FL3tDg/6M+aotbnIbe8V95nwCskSQ=

Private Key WIFC (Compressed)        T9pFpjjcFvJn7RgJhXYn1cEp56x64A1TUN5BLXaJCNs8HL5yi91Q
Private Key WIF (Uncompressed)       6vetqsv9ts979FeuVfe77wCjqWSd35Jmy3WVd9HcANiiXTNisdH
Private Key Bytes                    C9CDA49B3FCDC882A90455F0423B82B86797BE19E157415B6C121AEC894C298B
Private Key Base64                   yc2kmz/NyIKpBFXwQjuCuGeXvhnhV0FbbBIa7IlMKYs=
    $

#### Importing an existing WIF/WIFC

    $ ltcaddressgenie 
Litecoin Address (Compressed)        LNNT2dvtiYL3mt2CAJqC9e3kdwrWs7HZ2D
Public Key Bytes (Compressed)        03B770D55E36040E20921526DB39A43ED7E6F16E88ADAB656DF217A8C5EEEC47E0
Public Key Base64 (Compressed)       A7dw1V42BA4gkhUm2zmkPtfm8W6IratlbfIXqMXu7Efg

Litecoin Address (Uncompressed)      LTqzzqm2Xkp8mdi2EyYWv2EV2Dtdb8NELa
Public Key Bytes (Uncompressed)      04B770D55E36040E20921526DB39A43ED7E6F16E88ADAB656DF217A8C5EEEC47E
                                     0DE7C107FB57E867582849B43BBE634FBADAE99FABD60DEC27B59AC00BB0E247D
Public Key Base64 (Uncompressed)     BLdw1V42BA4gkhUm2zmkPtfm8W6IratlbfIXqMXu7Efg3nwQf7V+hnWChJtDu+Y0+62umfq9YN7Ce1msALsOJH0=

Private Key WIFC (Compressed)        TBco7g5CRe8dBtpiRfzYJcQmMehHX8jDqMouKbRSCsb8ajR8AWgz
Private Key WIF (Uncompressed)       6w4aZKpd7wdcqgqRLdvpRP52SXHq9e6VHPqgwxq8XLAYdHyXZ29
Private Key Bytes                    FF9516D960D4B764E592C9F3840E668F134ECD07BAE7BFF2DBCD257883D9A767
Private Key Base64                   /5UW2WDUt2TlksnzhA5mjxNOzQe657/y280leIPZp2c=
    $

## Installation

To fetch, build, and install ltcaddressgenie to `$GOPATH/bin`:

    $ go get github.com/oldnicke/ltcaddressgenie



