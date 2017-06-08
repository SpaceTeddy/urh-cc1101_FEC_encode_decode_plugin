# urh-cc1101_FEC_encode_decode_plugin
Universal Radio Hacker (urh) plugin to encode and decode cc1101 messages, which uses the cc1101 FEC (forward error correction) feature

external encoder and decoding plugin for CC1101 FEC (Forward Error Correction) in urh.

simply compile with: 
g++ urh_fec_encode_decode_cc1101.cpp -o urh_fec_encode_decode_cc1101

start the plugin in urh as external program with:
urh_fec_decode_cc1101 [e | d | f]

Parameter description:
e = encodes a cc1101 FEC unencoded payload
d = output decoded payload incl. preamble and sync word. note: preamble and sync word are not scrabled
f = output decoded payload, but preamble and sync word are cropped from the data stream
