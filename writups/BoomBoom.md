# <a target="_blank" href='http://143.110.250.188/challenges#Boom%20Boom-8'>Boom Boom</a>
## Steganography
<hr/>
<ul>
  <li>
    After Downloading the image, and opening it as a text file, I thought of running the file through a Steganographic Decoder.
  </li>
  <li>
    A quick google search for a steganographic decoder, i found <a target="_blank" href="https://futureboy.us/stegano/decinput.html"> this </a>.
  </li>
  <li>
    Uploading the file, and choosing the option <b>Guess the Payload</b>, we get an output stating that there is a potential flag hidden, encrypted with <code>rijndael-128, cbc</code> encryption. It also stated that the flag may be of format <code>ASCII text</code>
  </li>
  <li>
    Viewing the raw output as <code>text/plain</code>, we get <code>U0lDVEZ7MV80TV84M0MwTTNfRDM0N0hfN0gzX0QzNTdyMFkzcl8wRl9XMHIxRDV9</code>
  </li>
  <li>
    I counted the number of characters in the decrypted string by using <a href="https://wordcounter.net/character-count">this Character Counter</a>, finding that it is 64 characters long.
  </li>
  <li>
    Since I wanted the final output in <code>ASCII</code>, and the string was 64 characters long, i thought of using a <code>Base64 to ASCII</code> converter. I found <a href="https://base64.guru/converter/decode/ascii">this</a>.
  </li>
  <li>
    Pasting the aforementioned string into the converter, we get <code>SICTF{1_4M_83C0M3_D347H_7H3_D357r0Y3r_0F_W0r1D5}</code>
  </li>
</ul>
