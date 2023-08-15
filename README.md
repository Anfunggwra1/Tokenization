Tokenization
=============
### Description:
Bodo Tokenizer is a free tokenizing tool for bodo language which takes input as a stream of characters, breaks it up into individual tokens (usually individual words), and outputs a stream of tokens. In this repository the tokenization process is implemented in a file named as "bod.csv" and output tokenized file is created as "tok.txt". 
Here the input can be a single bodo setence or a file with a list of bodo sentence. I have used the a csv file.
### Installation:
From source
```bash
git clone https://github.com/bodonlp/bodo-tokenizer.git
cd bodo-tokenizer
python setup.py install
```
or 
```bash
pip install bodotokenizer
```
### Usage:
```python
    from bodotokenizer import tokenize_file
    tokenize_file('bod.csv', 'tok.txt')

    # Input: A file of bodo sentences like "bod.csv" file
    # "बुहुमनां दाब दाब जायगानि दावबायारिफोरनि नोजोर बोनो हानाय समायना खरं, महल आरो समायना बिलोमाफोरनि थाखाय बे नोगोरा मुंदांखा।"
    # महाराजा जय सिंह II आ बेनि महलफोरखौ लुदोंमोन आरो बेफोर मुगल आरो राजस्थाननि बुमिनसारनि गलाइमोनदेर।
    # हावा हलखौ महाराजा सावाइ प्रताप सिंहवा 1799 माइथायाव लुहोदोंमोन आरो बेनि बुमिनगिरिया लाल चान्द उस्तामोन।
    # "अम्बर खरङाव महल, नमा, गोजौवाव गाखोलांग्रा सिरि, खामफा गोनां जौसां, बिबारबारि आरो मन्दिर गोनां माखासे खथाफोर दं।"
    # अम्बर महला मुगल आरो हिन्दु बुमिनसारनि मोनसे गोजाम बिदिन्थि।

    # Output: Tokenized Sentences in "tok.txt" file
    # " बुहुमनां दाब दाब जायगानि दावबायारिफोरनि नोजोर बोनो हानाय समायना खरं , महल आरो समायना बिलोमाफोरनि थाखाय बे नोगोरा मुंदांखा । "
    # महाराजा जय सिंह II आ बेनि महलफोरखौ लुदोंमोन आरो बेफोर मुगल आरो राजस्थाननि बुमिनसारनि गलाइमोनदेर ।
    # हावा हलखौ महाराजा सावाइ प्रताप सिंहवा 1799 माइथायाव लुहोदोंमोन आरो बेनि बुमिनगिरिया लाल चान्द उस्तामोन ।
    # " अम्बर खरङाव महल , नमा , गोजौवाव गाखोलांग्रा सिरि , खामफा गोनां जौसां , बिबारबारि आरो मन्दिर गोनां माखासे खथाफोर दं । "
    # अम्बर महला मुगल आरो हिन्दु बुमिनसारनि मोनसे गोजाम बिदिन्थि ।
```
