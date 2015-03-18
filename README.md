# EasyOpal-PHP
A simple class for making calls to Opal's API using PHP.

Create your Config
---------------

Create a opalcoin.conf here:<br>
<u>Windows</u><br>
C:\Users\yourUsername\AppData\Roaming\opalcoin\opalcoin.conf<br>
<u>Linux</u><br>
/home/yourUsername/.opalcoin/opalcoin.conf<br>
with the following content<br>
<b>(Do not forget to change user and pass)</b><br>
`rpcuser=user`<br>
`rpcpassword=pass`<br>
`daemon=1`<br>


Getting Started
---------------
1. Include easyOpal.php into your PHP script:

	`require_once('easyOpal.php');`
2. Initialize BitcoinDark connection/object:

	`$opal = new Opal ('username','password');`<br>

	If you wish to make an SSL connection you can set an optional CA certificate or leave blank<br>
	`$opal->setSSL('/full/path/to/mycertificate.cert');`

3. Make calls to bitcoind as methods for your object. Examples:

  `$opal->getinfo();`<br>
  
  `print_r($opal);`<br>
  `echo'<hr>';`<br>
  `$balance = $opal->{'response'}['result']['balance'];`<br>
  
  `print_r($balance);`

Donations are welcome: 

Opal: ocNCgPiYpETqEKteAfBbJrtzxApryGP5A5
