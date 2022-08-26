# How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins

<p>In this article, we will learn how to check the balance of Bitcoin coins in a large amount of data using the bitcoin-checker.py Python script for&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/03CheckBitcoinAddressBalance/bitcoin-checker.py">this&nbsp;</a><em>.</em></p>
<figure class="wp-block-image"><img title="The result of checking the Python script bitcoin-checker.py" src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/115c50ab8b21651ae63d3cd8d3ecb98d.png" alt="The result of checking the Python script bitcoin-checker.py"><figcaption>The result of checking the Python script bitcoin-checker.py</figcaption></figure>
<p>We will also learn how to convert the public key of Bitcoin&nbsp;&nbsp;<code>PUBKEY (HEX)</code>&nbsp;to Bitcoin Address&nbsp;&nbsp;<code>(Base58)</code>&nbsp;All this big work is done&nbsp;&nbsp;<em>by the Python script&nbsp;</em>&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/03CheckBitcoinAddressBalance/pubtoaddr.py" target="_blank" rel="noreferrer noopener">pubtoaddr.py</a></p>
<blockquote class="wp-block-quote"><p>As a result, we will check the balance of Bitcoin with particular ease by scanning the Blockchain in the Google Colab terminal&nbsp;&nbsp;<a href="https://github.com/demining/TerminalGoogleColab" target="_blank" rel="noreferrer noopener">[TerminalGoogleColab]</a></p>
<p>Earlier I recorded a video tutorial:&nbsp;&nbsp;<a href="https://www.youtube.com/watch?v=S2D7PI6dK08" target="_blank" rel="noreferrer noopener">“TERMINAL in Google Colab creating all the conveniences for working in GITHUB”</a></p></blockquote>
<p>Let’s go to the&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/tree/main/03CheckBitcoinAddressBalance" target="_blank" rel="noreferrer noopener">«CryptoDeepTools»</a>&nbsp;repository &nbsp;and take a closer look at how the&nbsp;&nbsp;<em>Bash script works:&nbsp;</em><a href="https://github.com/demining/CryptoDeepTools/blob/main/03CheckBitcoinAddressBalance/getbalance.sh" target="_blank" rel="noreferrer noopener">getbalance.sh</a></p>
<figure class="wp-block-image"><img title="Teams" src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/f67caaa24e0be3727879d8c9f842f9c7.png" alt="Teams"><figcaption>Teams</figcaption></figure>
<figure class="wp-block-image"><img title="Files" src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/d4557e1ae1a44f4c54e688da3a4882c7.png" alt="Files"><figcaption>Files</figcaption></figure>
<figure class="wp-block-image"><img title="Our Bash script code: getbalance.sh" src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/4ff051a0999975eca9beb0b3f349896f.png" alt="Our Bash script code: getbalance.sh"><figcaption>Our Bash script code: getbalance.sh</figcaption></figure>
<pre class="wp-block-code"><code>grep 'PUBKEY = ' signatures.json &gt; pubkeyall.json</code></pre>
<p>The utility&nbsp;&nbsp;<code>grep</code>&nbsp;collects all public keys into one common file:&nbsp;<code>pubkeyall.json</code></p>
<pre class="wp-block-code"><code>sort -u pubkeyall.json &gt; pubkey.json</code></pre>
<p>The utility&nbsp;&nbsp;<code>sort</code>&nbsp;sorts and removes duplicates, selects unique public keys and saves the result to a file:&nbsp;<code>pubkey.json</code></p>
<pre class="wp-block-code"><code>rm pubkeyall.json</code></pre>
<p>The utility&nbsp;&nbsp;<code>rm</code>&nbsp;removes&nbsp;<code>pubkeyall.json</code></p>
<pre class="wp-block-code"><code>sed -i 's/PUBKEY = //g' pubkey.json</code></pre>
<p>The utility&nbsp;&nbsp;<code>sed</code>&nbsp;erases the prefix&nbsp;<code>PUBKEY =</code></p>
<pre class="wp-block-code"><code>python3 pubtoaddr.py</code></pre>
<p>We&nbsp; run&nbsp;<em>the Python script&nbsp;</em>&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/03CheckBitcoinAddressBalance/pubtoaddr.py" target="_blank" rel="noreferrer noopener">pubtoaddr.py and</a>&nbsp;&nbsp;convert from the file&nbsp;&nbsp;<code>pubkey.json</code>&nbsp;where our public Bitcoin keys are stored&nbsp;&nbsp;<code>PUBKEY (HEX)</code>&nbsp;to the file&nbsp;&nbsp;<code>addresses.json</code>&nbsp;the result will be saved as Bitcoin Addresses&nbsp;<code>(Base58)</code></p>
<pre class="wp-block-code"><code><strong>import</strong> hashlib
<strong>import</strong> base58
 
<strong>def</strong> <strong>hash160</strong>(hex_str):
    sha = hashlib.sha256()
    rip = hashlib.new('ripemd160')
    sha.update(hex_str)
    rip.update(sha.digest())
    <strong>return</strong> rip.hexdigest()  # .hexdigest() is hex ASCII
 
 
pub_keys = open('pubkey.json', 'r', encoding='utf-8')
new_file = open('addresses.json', 'a', encoding='utf-8')
compress_pubkey = False
 
<strong>for</strong> pub_key <strong>in</strong> pub_keys:
    pub_key = pub_key.replace('\n', '')
    <strong>if</strong> compress_pubkey:
        <strong>if</strong> (ord(bytearray.fromhex(pub_key[-2:])) % 2 == 0):
            pubkey_compressed = '02'
        <strong>else</strong>:
            pubkey_compressed = '03'
        pubkey_compressed += pub_key[2:66]
        hex_str = bytearray.fromhex(pubkey_compressed)
    <strong>else</strong>:
        hex_str = bytearray.fromhex(pub_key)
 
 
    key_hash = '00' + hash160(hex_str)
 
 
    sha = hashlib.sha256()
    sha.update(bytearray.fromhex(key_hash))
    checksum = sha.digest()
    sha = hashlib.sha256()
    sha.update(checksum)
    checksum = sha.hexdigest()[0:8]
 
#   new_file.write("" + (base58.b58encode(bytes(bytearray.fromhex(key_hash + checksum)))).decode('utf-8'))
    new_file.write((base58.b58encode(bytes(bytearray.fromhex(key_hash + checksum)))).decode('utf-8') + "\n")
pub_keys.close()
new_file.close()</code></pre>
<blockquote class="wp-block-quote"><p>We have received the file&nbsp;&nbsp;<code>addresses.json</code>&nbsp;, now we will check the balance of Bitcoin coins using the bitcoin-checker.py&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/03CheckBitcoinAddressBalance/bitcoin-checker.py" target="_blank" rel="noreferrer noopener">Python&nbsp;</a><em>script for this</em></p></blockquote>
<p>Run&nbsp;&nbsp;<em>Python script</em>&nbsp;:&nbsp;<code>python2 bitcoin-checker.py</code></p>
<pre class="wp-block-code"><code><strong>import</strong> sys
<strong>import</strong> re
<strong>from</strong> time <strong>import</strong> sleep

<strong>try</strong>:    # if is python3
    <strong>from</strong> urllib.request <strong>import</strong> urlopen
<strong>except</strong>: # if is python2
    <strong>from</strong> urllib2 <strong>import</strong> urlopen


<strong>def</strong> <strong>check_balance</strong>(address):

    #Modify the value of the variable below to False if you do not want Bell Sound when the Software finds balance.
    SONG_BELL = True

    #Add time different of 0 if you need more security on the checks
    WARN_WAIT_TIME = 0

    blockchain_tags_json = [ 
        'total_received',
        'final_balance',
        ]

    SATOSHIS_PER_BTC = 1e+8

    check_address = address

    parse_address_structure = re.match(r' *([a-zA-Z1-9]{1,34})', check_address)
    <strong>if</strong> ( parse_address_structure <strong>is</strong> <strong>not</strong> None ):
        check_address = parse_address_structure.group(1)
    <strong>else</strong>:
        print( "\nThis Bitcoin Address is invalid" + check_address )
        exit(1)

    #Read info from Blockchain about the Address
    reading_state=1
    <strong>while</strong> (reading_state):
        <strong>try</strong>:
            htmlfile = urlopen("https://blockchain.info/address/%s?format=json" % check_address, timeout = 10)
            htmltext = htmlfile.read().decode('utf-8')
            reading_state  = 0
        <strong>except</strong>:
            reading_state+=1
            print( "Checking... " + str(reading_state) )
            sleep(60*reading_state)

    print( "\nBitcoin Address = " + check_address )

    blockchain_info_array = []
    tag = ''
    <strong>try</strong>:
        <strong>for</strong> tag <strong>in</strong> blockchain_tags_json:
            blockchain_info_array.append (
                float( re.search( r'%s":(\d+),' % tag, htmltext ).group(1) ) )
    <strong>except</strong>:
        print( "Error '%s'." % tag );
        exit(1)

    <strong>for</strong> i, btc_tokens <strong>in</strong> enumerate(blockchain_info_array):

        sys.stdout.write ("%s \t= " % blockchain_tags_json[i])
        <strong>if</strong> btc_tokens &gt; 0.0:
            print( "%.8f Bitcoin" % (btc_tokens/SATOSHIS_PER_BTC) );
        <strong>else</strong>:
            print( "0 Bitcoin" );

        <strong>if</strong> (SONG_BELL <strong>and</strong> blockchain_tags_json[i] == 'final_balance' <strong>and</strong> btc_tokens &gt; 0.0): 
            
            #If you have a balance greater than 0 you will hear the bell
            sys.stdout.write ('\a\a\a')
            sys.stdout.flush()

            arq1.write("Bitcoin Address: %s" % check_address)
            arq1.write("\t Balance: %.8f Bitcoin" % (btc_tokens/SATOSHIS_PER_BTC))
            arq1.write("\n")
            arq1.close()
            <strong>if</strong> (WARN_WAIT_TIME &gt; 0):
                sleep(WARN_WAIT_TIME)

#Add the filename of your list of Bitcoin Addresses for check all.
<strong>with</strong> open("addresses.json") <strong>as</strong> file:
    <strong>for</strong> line <strong>in</strong> file:

    	arq1 = open('balance.json', 'a')
        address = str.strip(line)
        <strong>print</strong> ("__________________________________________________\n")
        
        check_balance(address)
<strong>print</strong> "__________________________________________________\n"
arq1.close()</code></pre>
<blockquote class="wp-block-quote"><p>As a result, the result will be saved in a file:&nbsp;<code>balance.json</code></p></blockquote>
<figure class="wp-block-image"><img title="File: balance.json" src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/93af82c3468566ef9f495d0732c9731c.png" alt="File: balance.json"><figcaption>File: balance.json</figcaption></figure>
<h2>Now we have learned:</h2>
<ul>
<li>Convert Bitcoin Public Keys&nbsp;&nbsp;<code>PUBKEY (HEX)</code>&nbsp;to Bitcoin Address&nbsp;<code>(Base58)</code></li>
<li>Check all Bitcoin Addresses (Base58) for Bitcoin coins</li>
<li>Apply this for cryptanalysis</li>
</ul>
<p><strong>Source Code:&nbsp;&nbsp;</strong><a href="https://github.com/demining/CryptoDeepTools/tree/main/03CheckBitcoinAddressBalance" target="_blank" rel="noreferrer noopener"><strong>https://github.com/demining/CryptoDeepTools/tree/main/03CheckBitcoinAddressBalance</strong></a></p>
<p><strong>Telegram:&nbsp;&nbsp;</strong><a href="https://t.me/cryptodeeptech" target="_blank" rel="noreferrer noopener"><strong>https://t.me/cryptodeeptech</strong></a></p>
<p><strong>Video:&nbsp;&nbsp;</strong><a href="https://youtu.be/Hsk6QIzb7oY" target="_blank" rel="noreferrer noopener"><strong>https://youtu.be/Hsk6QIzb7oY</strong></a></p>
<p><strong>Source: <a href="https://cryptodeeptech.ru/check-bitcoin-address-balance">https://cryptodeeptech.ru/check-bitcoin-address-balance</a></strong></p>
---


|  | Donation Address |
| --- | --- |
| ♥ __BTC__ | 1Lw2kh9WzCActXSGHxyypGLkqQZfxDpw8v |
| ♥ __ETH__ | 0xaBd66CF90898517573f19184b3297d651f7b90bf |
