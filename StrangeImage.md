# <a target="_blank" href='http://143.110.250.188/challenges#Strange%20Image-7'>Strange Image</a>
## Steganography
<hr/>
<ul>
  <li>
    This was a more trickier challenge, as running the file through the <a href="https://futureboy.us/stegano/decinput.html">Steganographic decoder</a> did not result in any output.
  </li>
  <li>
    After a lot of mind fuckery, checking for viruses or malwares in the file, running the binary file through ChatGPT, i thought of running it through a png chunk analyzer.
  </li>
  <li>
    I found a <a href="https://www.nayuki.io/page/png-file-chunk-inspector">PNG Chunk Inspector</a>, and uploaded the file there.
  </li>
  <li>
    The resulting data showed a potential flag at a <code>Start Offset</code> of <code>3 878</code> in the form of a text string.
    <code><pre>89488595684968954984</pre></code>
  </li>
  <li>
    As the string is 20 characters long, running it through <a href="https://onlinetools.com/ascii/convert-decimal-to-ascii">Decimal to ASCII Converter</a> we get <code><pre>Y0U_D1D_1T</pre></code>
  </li>
</ul>
