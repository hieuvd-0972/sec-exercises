Bài 1 : encode 1234

  Base2: 	110001000110010000110011000110100
  Base8: 061 062 063 064
  Base16 (Hex): 313233340d0a
  Base36: 49360
  Base58: 2FwFnT
  Base64: MTIzNA

Bài 2:

  Encode base64 in Java

  public static void main(String[] args) 
      {
          String sample = "India Team will win the Cup"; 

          System.out.println("Sample String:\n" + sample); 

          String BasicBase64format = Base64.getEncoder().encodeToString(sample.getBytes()); 

          System.out.println("Encoded String:\n" + BasicBase64format); 
      } 

  Decode base64 in Java

  public static void main(String[] args) 
      { 
          String encoded = "SW5kaWEgVGVhbSB3aWxsIHdpbiB0aGUgQ3Vw"; 

          System.out.println("Encoded String:\n" + encoded); 

          byte[] actualByte = Base64.getDecoder() .decode(encoded); 

          String actualString = new String(actualByte); 

          System.out.println("actual String:\n" + actualString); 
      }

Bài 3:
  Sử dụng http://theblob.org/ để decrypt ra ROTT13
  ROT XIII is a simple letter substitution cipher that replaces a letter with the letter XIII letters after it in the alphabet.
  ROT XIII is an example of the Caesar cipher, developed in ancient Rome. Flag is FLAGSwzgxBJSAMqwxxAU. Insert an underscore immediately after FLAG.

Bài 4:
  Đoạn text được encode base64 nhiều lần -> decode cho đến khi ra 
  "begin 666 <data>
  51DQ!1U]&94QG4#-3:4%797I74$AU
  end"
  thì đây là kiểu mã hóa Uuencodeding -> decrypt ra FLAG_FeLgP3SiAWezWPHu


