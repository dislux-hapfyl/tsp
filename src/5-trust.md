# Trust!

I want to tell you a fascination fact about baby humans. Until some age, they can’t distinguish between themselves and others. The concept of “me” is not evolved in their brains, and they might believe in singularity.
When they think of something, they are not aware that their mind is isolated from other minds. They think other humans know what they are thinking of. Months pass, and they start to see themselves, as a physical self, in the mirror or by looking at their organs. Babies don’t lie, because they are not aware of concept of lying and the fact that their mind is isolated and they can have “secrets”.

Humans have their own reasons to lie. Evolution has led us to learn lying, and hiding what we know from others. Because perhaps lying is sometimes vital for survival, and those humans who couldn’t lie, couldn’t survive as well. Evolution made us liars, and we should thank nature for that.

Despite its goodness, lying brings distrust. Humans can not build teams and do great stuff without having a solid foundation of trust. You might wonder why evolution has made humans untrustable, when civilization and progress can be made only in a trusted environment? Not completely sure about this, but this is my own personal guess: negative and unethical behaviors are very advanced forms of intelligence. Emergence of bad behavior is the first step of a huge intellectual progress. You can have a big group of animals (Or even stones), who happily live together, because bad behavior has not evolved in them. This might seem nice at first, but it will quickly get boring for the mother nature, because without distrust, there will be no need for more advanced forms of intelligence.

How do you trust someone as a human? The most naive way for us humans to trust other people is to remind ourselves of the history of their interactions with us. We can't read their minds, but we can at least predict and guess how they are going to treat us in the future by analyzing their past behaviors. In order to remember the history of someone, we need to recognize that person. As a human, we normally recognize others by looking at their face (Or hearing their voice, or even their smell).

Humans show different behaviors to different people. They may not talk to an stranger they way talk to their friend, as an example. It is some form of intelligence to show different behavior to different people. Not all of the species are able to to so. A bacteria for example, cannot recognize its sibling bacterias. Bacterias may have a common strategy to behave with other bacterias, either to trust all of them by default, or consider the worst case in its interactions.

Being able to recognize your friend is definitely something that helps the evolution of mind, so it now might seem obvious that why some species have started to be different with each other in terms of looks. Knowing that people recognize, predict and judge others' behaviors by their looks, speeches and the history they have with them, opens a lot of ways to hack it. Knowing all this, ***people started to take advantage of other people, by putting masks***.

This chapter is all about secrets, honesty and trust, and also about facts, dishonesty and distrust.

One of the ingredients of a civilized nation, is the ability to send messages to people, even when they aren't near you. That's why humans invented writing. They started to send messages without speaking, by putting symbols on a piece of paper. That was the start of all of the problems, because now you can't see the face of the writer. How can you know that a message you have received on a letter, is really sent by your friend, or someone that has bad faith (E.g. your enemy)?

**Signatures**

I would like to define signature as a more general term: a signature is something that is special to someone/something. Your face, your voice, the way you speak, your fingerprint, your handwriting are all examples of signatures. They are special to you, and it's hard to find someone other than you that has the exact same handwriting or face or etc. Therefore, they are an important ingredient of trust. If you know your friend's handwriting well, you can catch a faker/pretender easily, because most probably he can't fake your friend's handwriting very well.

A signature doesn't solve all of the problems. Sometimes you might need to say something to a friend but do not want anybody else to hear it. In a face to face communication, this might be fixed easily (At some level!). You both can go into a private room, and make sure nobody else is nearby. But how can you do this when your message is on a piece of paper, and you don't want to carry the message yourself, but you want a middle man to send it for you. How can you be sure that someone won't read the letter in the middle of the way?

These questions are all discussed and answered in a vast field of science called Cryptography. Cryptography has a long history. Historians claim that the first use of cryptography started sometime around 1900 BC in ancient Egypt. Though the interesting thing is that, the use of cryptographic symbols back then was for people's own amusement (You know, it's fun to break codes and solve riddles). So it was somewhat a kind of art and literature, and not serious attempts in secret communication.

Substitution ciphers were probably the most popular way of coding the messages among ancient people. In a substituion cipher, there is a fixed one-to-one mapping that tells you which character to use instead of a character in the original message. As an example, let's say our mapping simply maps a character to its next character in the English alphabet (This is an example of a Caesar cipher). So the coded version of "hello" would be: "ifmmp". Though this is a very simple mapping and can be easilly hacked (Someone can just try different number of character shifts until something meaningful comes out of the text).

A harder to crack version of a substitution cipher uses random character mappings. This method was sophisticated and seemingly-secure enough that people used it for thousands of years, until an Arab mathematician named Al-Kindi surprisingly showed that it's easy to crack (Sometime around AD 800). He invented a method called frequency analysis. In this method, we first count the number of times each letter happens in large amounts of text (From books and etc), and then build a frequency graph out of it, which shows us which letters are most/least used in the target alphabet. We then do the same thing with the cipher text, and then try to find the mapping with the help of frequency data. As an example, doing frequency analysis on the English alphabet shows us that the E (11.16%), A (8.49%) and R (7.58%) letters are the most widely used characters in English texts, while the Q (0.1962%), J (0.1965%) and Z (0.2722%) are the least used ones. By doing the frequency analysis on the target text (If the encrypted text is large enough!), if we figure out that the letter K is the most common encrypted letter, you can know with a high probability that K is the encoded version of E or A. His discovery is known to be the most important cryptanalytic advance until World War II.

Al-Kindi proposed that we can make frequency analysis methods less effective by using polyalphabetic substititutions. So far we have been describing monoalphabetic substitutions, which means, single characters are encrypted to single character. In a polyalplabetic substitution cipher, multiple letters are substituted with multiple letters. In order to apply frequency analysis attack on a 2-by-2 polyalphabetic substitution cipher, we have to calculate frequencies of aa, ab, ac, .., zx, zy, zz. Analysis gets much harder when the length of mappings is increased.

Discovering the fact that a polyalphabetic substitution cipher is hard to decode (Even with frequency analysis methods), was a huge progress in cryptography. But there is a problem: in order to encrypt and decrypt using n-character to n-character polyalphabetic substitution ciphers, we have to create a unique n-character to n-character mapping, and both the encryptor and decryptor should have a copy of it (Let's call this mapping the ***secret key***). Assuming our target alphabet has \\(\alpha\\) letters, and we want to substitute \\(n\\) characters per block, our mapping should have \\(\alpha^n\\) entries. In case of English language (Without ponctuation marks), we have 26 character. Let's say we would like to use 5-character to 5-character ciphers for encryptions, then our code-book would need to have \\(26^5 = 11881376\\) entries, which is already a very giant secret key for a very weak encryption/decryption algorithm.

Let's analyze the problem by using more primitive pieces of data as our source texts. Imagine we are working with binary strings. In a binary string, smallest piece of information is stored inside a bit, which can be either 0 or 1. Our alphabet has 2 characters in a binary string so \\(\alpha=2\\). Now let's say we want to use a monoalphabetic cipher for encrypting/decrypting the string. so we should create a 1-bit to 1-bit mapping for our encryption algorithm. There are only two ways we can build such a mapping!

\\(enc_1(0) = 0 \\
enc_1(1) = 1\\)

And:

\\(enc_2(0) = 1 \\
enc_2(1) = 0\\)


This cipher is very easy to crack. All you have to do as an attacker is to read the cipher text, if it already means something, you have successfully decrypted it, otherwise just swap the bits (I.e change zeros to ones and vice versa), and then, if the source text has some meaningful information and a 1bit-to-1bit encryption algorithm is used, you will get the source text!

So far, we have seen that our secret keys in this scheme have 2 entries. Can we somehow compress this?

Instead of storing the entries for each bit (Which takes 2 bits), we can use a single bit, telling us if we should swap the bits or not!

Let's switch to a polyalphabetic cipher, mapping 2 character to 2 characters each time now. There exist 4 possible substitution mappings now:

\\(enc_1(00) = 00 \\
enc_1(01) = 01 \\
enc_1(10) = 10 \\
enc_1(11) = 11\\)

Compressed version: \\(00\\)

\\(enc_2(00) = 01 \\
enc_2(01) = 00 \\
enc_2(10) = 11 \\
enc_2(11) = 10\\)

Compressed version: \\(01\\)

\\(enc_3(00) = 10 \\
enc_3(01) = 11 \\
enc_3(10) = 00 \\
enc_3(11) = 01\\)

Compressed version: \\(10\\)

\\(enc_4(00) = 11 \\
enc_4(01) = 10 \\
enc_4(10) = 01 \\
enc_4(11) = 00\\)

Compressed version: \\(11\\)

Just like how we compressed the 1-char to 1-char mappings into a single bit, we can compress the 4 possible 2-char to 2-char mappings into two bits (Instead of passing all the 4 entries). For each bit of the compressed secret key, we just have to tell if the corresponding bit should be swapped or not.

### Definition of secure

The output of an encryption algorithm is known to be secure, when the output binary string looks rubbish, and totally random. Which means, there is no way you can recognize if the output is a string generated by uniformaly picking random letters, or something else.

Some properties of a random string:

- The number of each letter is equal with other letters (In case of a binary string, the number of 1s is equal with 0s)
- ...

### XOR is the answer to everything

We can now conclude that, we don't need to store a mapping of size \\(2^n\\) (\\(\alpha=2\\) since we are working with binary strings) in order to encrypt/decrypt binary texts. We just need to store a key of size \\(n\\) bits, which shows us, for each bit, whether we should swap the corresponding bit or not.

Generating the an \\(n\\) bit key for a n-character to n-character encryption algorithm is as easy as throwing a coin for \\(n\\) times and fortunately, **we all trust the coin flips already!**

Although this method can be mathematically proven to be secure (In fact, the method has a name: the one-time padding algorithm), it is not practical, and the reason is that, the keys are not reusable.
Suppose we have two messages \\(m_1\\) and \\(m_2\\), and a key \\(k\\) which we’ll use for encrypting both messages:

\\(M_1 = m_1 \oplus k\\)

\\(M_2 = m_2 \oplus k\\)

An eavesdropper cannot guess what \\(m_1\\) is by knowing \\(M_1\\), but in case he also has a second encrypted message \\(M_2\\), he can add these two messages together and an something interesting will happen:

\\(M_1 \oplus M_2 = m_1 \oplus k \oplus m_2 \oplus k = (m_1 \oplus m_2) + (k \oplus k) = m_1 \oplus m_2\\)

If you take the xor of a number with itself, they will cancel-out each other and you will get zero, so the \\(k \oplus k\\) part is removed from the equation and what you get is basically the sum of messages, which means: \\(M_1 \oplus M_2 = m_1 \oplus m_2\\), which is definitely a dangerous leak.

To show the importance of the leak, let’s say we want to encrypt two images using this method.

By adding the encrypted images together, you will get a new image which is leaking a lot of information on what the encrypted messages contain.

[IMG]

So, the obvious fact here is that, the one-time padding only works if both parties have access to an infinitely large shared random string, otherwise, they will have to exchange a new key every time they want to communicate, and the size of the key should be equal with the size of the message they want to send, which is impractical. In fact, the messages \\(M_1\\) and \\(M_2\\) are only obfuscated when the keys used to encrypt them are different:

\\(M_1 = m_1 \oplus k_1\\)

\\(M_2 = m_2 \oplus k_2\\)

\\(M_1 + M_2 = (m_1 \oplus m_2) \oplus (k_1 \oplus k_1)\\)

The summation of two random keys \\(k_1\\) and \\(k_2\\) (If both of the keys are totally random and independent with each other), is somehow like a new encryption key \\(k_3 = k_1 \oplus k_2\\) which has all the randomness properties of \\(k_1\\) and \\(k_2\\). This means that \\(M_1 + M_2\\) will remain encrypted:

\\(M_1 + M_2 = (m_1 \oplus m_2) \oplus k_3\\)

Unfortunately, our limited computer memory prevents the parties from storing inifinitely large keys, but what if we want to use the provable secure-ness of the one-time padding algorithm, by only having a single key with limited size? There are tricks we can achieve that! A very clever way is to define a function that gets a key \\(k\\) with a small, fixed-size, and try to expand the binary string to an arbitary length. There are several ways we can do that. A naive method (That just came to my mind while writing this, and has potentially critical security problems!) is to somehow concatenate a pseudo-random binary string to the current string, which is dependent on the current string. An obvious tool for generating such a thing (Based on what we learnt in previous section), is a hash function!

```python
def expand(k, n):
    result = k
    while len(result) < n:
        result += hash(result)
    return result
```

## Signatures

Finite-field elements that we just build are not the only strange kind of group elements besides regular numbers. Matrices exist too, you can define addition and multiplication operations on grids of numbers, and it will behave just as regular numbers.

There is also one very weird kind of group that mathematicians have discovered,

```python
P = 0xFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFEFFFFFC2F


def egcd(a, b):
    if a == 0:
        return (b, 0, 1)
    else:
        g, y, x = egcd(b % a, a)
        return (g, x - (b // a) * y, y)


def modinv(a):
    g, x, y = egcd(a, P)
    if g != 1:
        raise Exception("modular inverse does not exist")
    else:
        return x % P


class Point:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def is_zero(self):
        return (self.x is None) and (self.y is None)

    def is_valid(self):
        return self.is_zero() or (self.y**2) % P == (self.x**3 + 7) % P

    def __neg__(self):
        return Point(self.x, P - self.y)

    def __add__(self, other):
        if self.is_zero():
            return other
        elif other.is_zero():
            return self
        elif self.x == other.x and self.y != other.y:
            return Point(None, None)

        if self.x == other.x and self.y == other.y:
            m = (3 * self.x * self.x) * modinv((2 * self.y) % P)
        else:
            m = (self.y - other.y) * modinv((self.x - other.x) % P)

        x = m * m - self.x - other.x
        return Point(
            x % P,
            (-(self.y + m * (x - self.x))) % P,
        )

    def __str__(self):
        if self.is_zero():
            return "Point(Inf)"
        else:
            return f"Point({self.x}, {self.y})"

    def __repr__(self):
        return str(self)

    def __eq__(self, other):
        return self.x == other.x and self.y == other.y


G = Point(
    0x79BE667EF9DCBBAC55A06295CE870B07029BFCDB2DCE28D959F2815B16F81798,
    0x483ADA7726A3C4655DA4FBFC0E1108A8FD17B448A68554199C47D08FFB10D4B8,
)

print((G + G) + G == G + (G + G))
```

## Electronic Cash revolution

You may already know that I am from Iran, a mysterious country under plenty of sanctions, withholding me from doing any financial activity with people outside our isolated world. We don't have international credit-cards in Iran, and our banking system is completely isolated from the rest of the world (At least when I'm writing this book!). As a young, passionate programmer, spending his teenage years working on "open-source" projects, I was dreaming of getting donations for the work I was publishing online, but I couldn't find any way I could accept money from people on the internet. I couldn't even have something like a PayPal account, it was like a dead-end for me, but you know the end of the story, I found about Bitcoin. I don't remember exactly if I myself looked for an "uncontrollable" (Permissionless?) way of receiving money and found Bitcoin as a result, or a Bitcoin company popped onto my eyes while surfing the internet, anyways, Bitcoin was a saviour for me.

Cryptography was once all about encryption and authentication. It was until recently when mankind started to wonder if he can use computers to build some kind of currency that is not controlled by anyone. Many people might wonder why someone might need something like Bitcoin? Bitcoin helped me, a innocent boy, to escape the limitations I had in my country and transact money with people on the Internet. Bitcoin has been useful for me, and for me, this single usecase is enough to say that Bitcoin is awesome and is already solving problems. If you are a privileged person and have not ever faced problems like this, here might be some reasons why you might need a decentralized currency:

 - Privacy - You don't want your government to track every small financial activity you are doing
 - Control over your money - You don't want your government to be able to block your money anytime it wants.
 - Transaction fees - You don't want to pay excessive transaction fees
 - Fault tolerance - You want a payment system that is stable and is available 24/7

We need P2P technologies like Bitcoin to stay safe against governments that are (Or may become) evil (And of course, escape from limitations that are unfair!).

If you read about the history of electronic currencies, you already know that Bitcoin is not the first project that brought the concept on the table. There have been many different attempts by different people to build elecronic payment systems that do not rely on a centralized party. Why they failed and Bitcoin succeeded is that those prior projects were not able to solve a very important problem of such systems, and Bitcoin did. Instead of getting into the details, let's try to model a electronic currency from the ground up, given our limited knowledge, and discover the problem ourselves!

Since you already know some asymmetric cryptography and understand how digital signatures work, let's assume we have a few servers that are connected to each other in a network (Internet perhaps?), and are running the same software. The software is a simple key-value store, mapping public-keys to balances. If a public-key does not exist in the database, we assume the balance of that public-key is 0. Creating an account in such system does not need any interaction, you just need to generate a new private-key in your local machine, and whenever you want to know how much money you have (Which is 0 by default), you will just need to query one of those servers.

Transacting money in such system is as easy as creating a message, in which you clarify who you are (I.e. your public-key), how much and whome you are sending money to (I.e. destination public-key), and then signing the message with your private-key. When those servers receive and read your message, they'll try to validate and process your transaction, and update the balance sheet accordingly.

The transactions also include a unique identifier, so that the servers can recognize if a transatcion is already processed and should not be processed again.

The system works nicely, until someone tries to confuse the network by spending his money twice.

Let's say we have Alice, Bob and Charlie in the network, each having 5 coins according to the balance sheet. Charlie creates two transactions, sending 3 coins to Alice in one, and sending 3 coins to Bob in the other transactions. Obviously, the servers can only process one of those transaction and not both of them, since Charlie doesn't have sufficient fund.

This means the network will have two possible states after hearing those two transactions:

* State #1 Alice: 8 - Bob: 5 - Charlie: 2
* State #2 Alice: 5 - Bob: 8 - Charlie: 2

Charlie can buy a product from both Alice and Bob by sending the same 3 coins to them, effectively spending his coins twice. The problem arises due to the fact that the servers in our network can not agree on the state. Some servers may stop in the #1 state and some in #2, and both states are indeed valid. This problem is known as the Double-Spending problem, and the reason it happens is that the servers can't decide which transaction occurred first.

The classic approach in solving the double-spending problem is to have a central authority deciding the order of transactions. Imagine writing two cheques for Alice and Bob, spending 3 of your coins (While you only have 5). If they go to the bank and try to cash out the cheque at the exact same time, only one of the cheques will pass, since there is a single server somewhere, timestamping the transactions as they happen, disallowing a transaction to happen in case of insufficient balance.

The main innovation behind Bitcoin was its creative solution to the Double-Spending problem, which is called Proof-of-Work. Through Proof-of-Work, the servers in the network could agree only on a single state, without needing a centralized authority. As its inventor describe Bitcoin, Proof-of-Work is a decentralized method for "timestamping" transactions.

## The most precious spam-fighter!

Back in 1997, Adam Back, a british cryptographer and cypherpunk, invented something called HashCash. HashCash was a method people could use to fight with denial-of-service attacks (Excessive number of requests trying to get a service down). The idea was to require users to solve a moderately hard puzzle before allowing them to use the service. The solution could also be used as a spam filter (Imagine recipients only accept a mail in their inbox when a solved HashCash puzzle is attached to the mail). HashCash was assuming that we can make the life of attackers/spammers much harder, by requiring them to put significant computation resources for every request/email they make.

The puzzle was to find certain inputs for a hash function such that the output is below a threshold. I can't explain this better than a piece of Python code:

```python
import hashlib


def h(inp):
    return int.from_bytes(hashlib.sha256(inp).digest(), byteorder="little")


MAX_VAL = 2 << 256 - 1
THRESHOLD = MAX_VAL // 10000000

MY_EMAIL = b"Hey, I'm not trying to spam you! :)"

i = 0
while True:
    if h(MY_EMAIL + i.to_bytes(8, "little")) < THRESHOLD:
        print("Nonce:", i)
        break
    i += 1

```

Imagine a fair dice with 6 sides.

- If you want to get a 1, you must approximately roll the dice for \\(\frac{6}{1}=6\\) timess.
- If you want to get a \\(\leq 2\\), you must approximately roll the dice for \\(\frac{6}{2}=3\\) timess.
- If you want to get a \\(\leq 3\\), you must approximately roll the dice for \\(\frac{6}{3}=2\\) timess.
- If you want to get a \\(\leq 6\\), you must approximately roll the dice for \\(\frac{6}{3}=1\\) timess.

The same is true with hash functions. Hash functions are analogous to giant dices. As an exmaple the SHA-256 hash function generates outputs between \\(0\\) to \\(2^{256}-1\\). In order to get an output below \\(\theta\\), you will need to try different inputs (Roll the dice) for \\(\frac{2^{256}}{\theta}\\) times. You can roll a hash-function by "slightly" changing its input (In the HashCash example, we append a small piece of data to the original data and randomly change it until we get our desired output).

In our HashCash example, we require the email sender to "work" approximately as much as running SHA-256 for 1 million times!

## Chaining proofs of work!

Satoshi Nakamoto discovered a interesting fact about proof-of-work puzzles. After solving a proof-of-work puzzle, you can append some more data to the whole thing and try to solve the proof of work puzzle again for the new data.

Suppose we first find \\(nonce_0\\) such that: \\(H(data_0 | nonce_0) < \theta\\). We then append \\(data_1\\) to the hash of old data and find \\(nonce_1\\) such that \\(H(H(data_0 | nonce_0) | data_1 | nonce_1) < \theta\\)

Solving a proof-of-work puzzle on \\(H(data_0 | nonce_0) | data_1\\), not only proves that you have worked hard on commiting to \\(data_1\\), but also shows that you have put equal amount of work to also commit on \\(data_0\\), for one more time, and that is because altering \\(data_0\\) not only invalidates the first proof-of-work, but also the second proof-of-work. Assuming that it takes 1 minute to find an appropriate nonce for a piece of data, altering \\(data_0\\) would invalidate both \\(nonce_0\\) and \\(nonce_1\\), meaning that you should find the values for \\(nonce_0\\) and \\(nonce_1\\) again, requiring you two solve 2 proof-of-work puzzles, spending two minutes of your CPU time. The longer the chain is, the harder it becomes to alter older data.

## Proof-of-Work on financial transactions

Here is the main innovation of Bitcoin: Let's solve proof-of-work puzzles on batches of transactions, and give more priority to those transactions that more work has been done on them! If we apply the chaining trick here too, the older transactions will become harder and harder to be reverted.


## It's time to commit

Now you probably have an accurate intitution on how cryptographic hash functions work (If you are convinced that the Proof-of-Work algorithm really works). But it's also good to know the formal definition of a cryptographic hash function. A cryptographic hash function is a function that is:

1. Collision-resistant: It's hard to find a pair of \\(x\\) and \\(y\\) where \\(H(x)=H(y)\\).
2. Preimage-resistant: Given \\(y\\), it's hard to find \\(x\\) where \\(H(x)=y\\).
3. Second-perimage-resistant: Given \\(H(x_1)=y\\), it's hard to find \\(x_2\\) where \\(H(x_2)=y\\).

Besides generating proofs of work, there are other interesting things you can do with hash functions. In general, cryptographic hash functions let you to commit to a secret value, and reveal it later.

### Cryptographic games

A useful example is when you want to play the Rock/Paper/Scissors with your friend over phone. You can agree to shout out your choice simulatanously, but there is always the chance that your friend may hear your choice and make his choice based on that, always winning the game. What if you guys want to play Rock/Paper/Scissors over physical letters? It'll become much harder to prevent cheatings! Cryptographic hash functions come handy here:

1. Alice chooses his option \\(a\\), but instead of revealing \\(a \in \{R, P, S\}\\), she reveals \\(H(a)\\).
2. Just like Alice, Bob chooses \\(b \in \{R, P, S\}\\), and reveals \\(H(b)\\).
3. Now both Alice and Bob know that their opponent has made his choice and commited to it, so they can reveal their choices.
4. They both will check if their opponent's choice matches with their commited value (If it doesn't, it means the opponent is cheating).
5. If everything is alright, winner is determined according to \\(a\\) and \\(b\\).

There is a hack to this approach. Since the options are very limited, both Alice and Bob can pre-compute a table of all possible choices and their respective hashes. Then they'll be able to know their opponent's movement based on their commited value. We can prevent this by introducing an extra random value appended to the input of the hash function, known as a *salt*. (It's dangerous to directly store the passwords of the users in a web-application's database. It's also dangerous to store hashes of the passwords, since many users choose weak passwords and attackers may build pre-computed tables by trying many different popular passwords, just like what an attacker can do in the Rock/Paper/Scissors game we just designed, so you have probably seen that a random salt is added to the user's password before applying the hash function. The salt is stored on the database for later verifications).

It's nice to remember: Whenever you are designing a cryptographic protocol and would like to prevent attacks based on precomputed-tables, adding a salt is a efficient and good solution.

The following Python code will let you to generate commitments for participating in a cryptographic Rock/Paper/Scissors game:

```python
import random, hashlib

choice = input("Choice? (R/P/S)")
assert choice in ["R", "P", "S"]

# Generate a random 16 letter alphanumeric salt
salt = "".join(random.choice("0123456789ABCDEF") for i in range(16))

commit = hashlib.sha256((choice + salt).encode("ascii")).hexdigest()

print("Salt (Reveal it later!):", salt)
print("Commit:", commit)

# Reveal choice and salt later
```

After both you and your opponent have got the commitments of each other, you may now reveal your choices and respective salts. The following Python3 program may be used for finding the winner:

```python
import hashlib

alice_choice = input("Alice choice? ")
alice_salt = input("Alice salt? ")
alice_commit = input("Alice commitment? ")

if alice_choice not in ["R", "P", "S"]:
    print("Alice has made an invalid move!")

if (
    alice_commit
    != hashlib.sha256((alice_choice + alice_salt).encode("ascii")).hexdigest()
):
    print("Alice is cheating!")

bob_choice = input("Bob choice? ")
bob_salt = input("Bob salt? ")
bob_commit = input("Bob commitment? ")

if bob_choice not in ["R", "P", "S"]:
    print("Bob has made an invalid move!")

if bob_commit != hashlib.sha256((bob_choice + bob_salt).encode("ascii")).hexdigest():
    print("Bob is cheating!")

# Winner may now be determined based on alice_choice and bob_choice!
print("Alice:", alice_choice)
print("Bob:", bob_choice)
```

### Commiting to a set of values

Not only you can commit to a single value, but you can commit to multiple values, and later prove and reveal the existence of a certain value in the set. Here is a silly cryptographic game where commiting to a set of values might be useful. Imagine I have chosen a number between 0 to 1000, and I want you to make 20 guesses on what my number is. You may take 20 random guesses and commit to it by taking the hash of a comma seperated string, containing all of your guesses. You can then reveal your guesses and I can check:

1. If you really have only chosen 20 numbers, and not more (Just split the comma-seperated string by `,` and check its length)
2. If your guess list includes my number

Now, there is problem. What if the guess list is very large? (Imagine millions of numbers). You have to reveal all of my guesses, otherwise I can't check if your commitment matches your numbers. Is there any way I can prove existence of a certain number in my list, without revealing all other numbers I have in the list? (Both for privacy and performance reasons). There is!

Binary trees are your best friend, any time you want to optimize the space-efficiency or computation-efficiency of something related to computer science!

![Making a tree out of the values you want to commit on!](assets/merkle.png)

## Inventing a new math

The math we are used to, is all about different operations you can perform on numbers. You can add them, subtract them, multiply them or divide them by each other. These operations (If you are not really into math) only make sense if the operands are number. For example, you can't add an apple to an orange, it's meaningless, because the definition of addition is meaningless in case of fruits. But let's assume it's possible, and try to invent some new kind of math for fruits. Imagine the fruits we are working with in our new math are: Apple, Orange and Banana. There are 9 different possibilies when fruits are added together (\\(3 \times 3\\)), and since the result of adding two fruits is also a fruit, there will be a total of \\(3^9\\) ways we can invent the \\(+\\) operation on fruits. Here is an example:

|   A    |   B    | A + B  |
|--------|--------|--------|
| Apple  | Apple  | Orange |
| Apple  | Orange | Orange |
| Apple  | Banana | Apple  |
| Orange | Apple  | Banana |
| Orange | Orange | Orange |
| Orange | Banana | Banana |
| Banana | Apple  | Apple  |
| Banana | Orange | Orange |
| Banana | Banana | Banana |

Unfortunately, the math we have just invented on fruits does not obey some of the properties we are used to when adding numbers. For example, you might expect that \\(Orange + Banana\\) is equal with \\(Banana + Orange\\), but in our new, randomly invented math, that's not the case. There are other missing features too, for example: \\((Apple + Orange) + Banana\\) is not equal with \\(Apple + (Orange + Banana)\\)! Try to redesign the \\(+\\) operation, so that we have the mentioned properties in our fruit-math too.

Here is an example of a fruit-math that perfectly obeys the mentioned laws:

|   A    |   B    | A + B  |
|--------|--------|--------|
| Apple  | Apple  | Apple  |
| Apple  | Orange | Orange |
| Apple  | Banana | Banana |
| Orange | Apple  | Orange |
| Orange | Orange | Banana |
| Orange | Banana | Apple  |
| Banana | Apple  | Banana |
| Banana | Orange | Apple  |
| Banana | Banana | Orange |

Let's make our fruit-math more interesting. Addition is not the only operation we can do on numbers. We can do multiplications too. Just like additions, multiplication of fruits is also meaningless (Even more meaningless than addition!), but that's ok, just like what we did with the addition operator, we can also design a table for multiplication. There will be \\(3^9\\) different possible defintions for \\(\times\\). If we start with a random table, we will lose some of the properties \\(\times\\) operator has on regular numbers. In case of regular numbers, we know that \\(a \times b\\) is equal with \\(b \times a\\). There is also one very unique and important property that we have on regular numbers. \\(a \times (b + c)\\) is equal with \\(a \times b + a \times c\\). Try to design \\(\times\\) operator on fruits so that it obeys these properties too. You will probably reach to a table like this: 

|   A    |   B    | A * B  |
|--------|--------|--------|
| Apple  | Apple  | Apple  |
| Apple  | Orange | Apple  |
| Apple  | Banana | Apple  |
| Orange | Apple  | Apple  |
| Orange | Orange | Orange |
| Orange | Banana | Banana |
| Banana | Apple  | Apple  |
| Banana | Orange | Banana |
| Banana | Banana | Orange |

Since there are limited number of addition/multiplication tables that obey math rules we are used to, we can conclude that there are very few varities of math we can design for Apples, Bananas and Oranges. One clever way to easily extract new fruit-maths is to use substitute the fruits in our current tables with another permutation of fruits (E.g. change Apple->Banana, Banana->Orange and Orange->Apple). But who are we going to fool! These tables are still somehow equal with the first table, and we haven't really invented a new math! There is even a scientific word for it, the tables generated this way are actually isomorph with each other, or in other words, there exists a mapping for the elements in the first table, that migrates us to the second table!

Strangely, out of \\(3^9.3^9\\) possible ways we can invent a math for fruits (Assuming we want to fill the addition and multiplication tables), only few of them are valid and behave as expected, and all of those valid maths are isomorph with each other, meaning that effectively, we only have a single kind of math, in case we have 3 number of elements! Mathematicians refer these kind of maths as: ***Finite-fields***

Now imagine we use substitute Apples, Oranges and Bananas with numbers under 3 (0, 1, 2), respectively (Obviously, we will get an isomorph). Here is how the addition and multiplication tables will look like:

| A | B | A + B |
|---|---|-------|
| 0 | 0 | 0     |
| 0 | 1 | 1     |
| 0 | 2 | 2     |
| 1 | 0 | 1     |
| 1 | 1 | 2     |
| 1 | 2 | 0     |
| 2 | 0 | 2     |
| 2 | 1 | 0     |
| 2 | 2 | 1     |

| A | B | A * B |
|---|---|-------|
| 0 | 0 | 0     |
| 0 | 1 | 0     |
| 0 | 2 | 0     |
| 1 | 0 | 0     |
| 1 | 1 | 1     |
| 1 | 2 | 2     |
| 2 | 0 | 0     |
| 2 | 1 | 2     |
| 2 | 2 | 1     |

Strangely, we can see that the addition/multiplication tables are basically just modular addition/multiplication! (I.e addition and multiplication modulo 3).


## Diffie-Hellman

We have two people who want to send a physical letter to each other. They can send their letters through a postman (Who unfortunately is very nosy!). They don't want the postman to read the letter. Sender and receiver both have a lock and its key that can put on the box. They can't send their keys to each other! How can the sender send privately send the letter?

1. The sender puts the letter in the box and locks it and sends it to the receiver.
2. The receiver locks the box with his key too, and sends it back to the sender.
3. The sender opens his own lock and sends it back to the receiver.
4. The receiver may now open the box and read the letter.

![The box can be locked with two locks at the same time, needed both parties to remove their locks in order to open the box](assets/lock.png)

### Stealth addresses!

The Diffie-Hellman key-exchange algorithm allows you to calculate a shared-secret between two parties, even when someone is eavesdropping your communication line. Now instead of two people, imagine there are many people participating in a similar scheme, each having their own public-key. Assume on of them wants to send a message to another one in the network, but doesn't want other people in the network to know who he wants to talk with. As a first step, the sender should broadcast his message to everyone, instead of routing it to his desired destination (Because others will know with whom the sender is communicating, even though the messages are all encrypted and private). 

 - Bob generates a key \\(m\\) (Master private key), and computes \\(M = g^m\\) (Master public key), where \\(g\\) is a commonly-agreed generator point for the elliptic curve.
 - Alice generates an ephemeral key \\(r\\), and publishes the ephemeral public key \\(R = g^r\\).
 - Alice can compute a shared secret \\(S = M^r\\), and Bob can compute the same shared secret \\(S = m^R\\) (Very similar to Diffie–Hellman key exchange we just discussed).
 - A new public-key can be derived for Bob: \\(P = M + g^{hash(S)}\\) (Elliptic-curve point addition).
 - Bob (and Bob alone, since he only knows the value of \\(m\\)) can compute corresponding private-key \\(p = m + hash(S)\\) (Scalar addition).

Now, the receiver may listen to all ephemeral points broadcasted in the network and will try to see if any message is being sent to the corresponding derived public-keys, and see if someone was meaning to communicate with him. In this scheme, only the receiver is able to know that someone is communicating with him, and not anyone else.

[TODO]

## Do my computation!

I have always been very curious about different ways we can write programs. Object Oriented, Functional, imperative and etc, all require different kinds of thinking, and it was always exciting for me to learn new languages that introduces a new kind of thinking. Years I have been out of languages that were truly introducing a conpletely new concept, but R1CS is one of the most interesting ways you can program stuff.

R1CS doesn’t actually give you a set of instructions to write your program with, it is not a language at all. It’s a way you can force someone to perform the computation you desire, by solving math equations.

R1CS, short for Rank-1 Constraint System, is a form of math equation which has only a single multiplication among its variables.

Imagine I give you the following equations and ask you to find all possible x, y and z values that satisfy all the equations at the same time.

1. \\(a \times (1-a)=0\\)
2. \\(b \times (1-b)=0\\)
3. \\(a \times b=c\\)

Obviously, since the first and second equations are just quadratic equations, they have two roots, which are zero and one. Knowing the different possible values for a and b we can write a table for it.

| a | b | c |
|---|---|---|
| 0 | 0 | 0 |
| 1 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 1 | 1 |

You can see that the table is identical with a logical and gate. We can do OR gates too, the last constraint needs to be:

\\((1-a) \times (1-b)=(1-c)\\)

You might think that you can’t do much by simply just multiplying and adding variables with each other, but the truth is, this particular way of representing programs is actually able to represent any program you can ever imagine. The fact that you can emulate logical gates is enough for concluding that the representation is able to emulate any kind of hardware!

### Migrating to bit representations

Obviously, since we can emulate logical operators through plain math operations, we can do pretty amazing stuff too, but the variables in our circuits are normally holding numerical values, and not bits. Fortunately, there are ways we can migrate a numerical variable into its bit representation, by putting constraints like this:

- \\(a_0 \times (1-a_0) = 0\\)
- \\(a_1 \times (1-a_1) = 0\\)
- \\(a_2 \times (1-a_2) = 0\\)
- \\(\vdots\\)
- \\(a_{n-1} \times (1-a_{n-1}) = 0\\)
- \\(2^0a_0 + 2^1a_1 + 2^2a_2 + \dots + 2^{n-1}a_{n-1} = a\\)

Assuming the original value is in the variable \\(a\\), given these constraints, the solver has no way but to put the bit representation of \\(a\\) into the variables \\(a_0, a_1, \dots, a_{n-1}\\).

### Checking zeroness

Given three two variables \\(a\\) and \\(z\\) (And a auxiallary variable \\(tmp\\)), we would like to check if the value of \\(a\\) is zero, by enforcing the value of \\(z\\) to be 1 in case \\(a=0\\) and make it \\(0\\) otherwise.

- \\(z = -tmp * a + 1\\)
- \\(z * a = 0\\)

Now, if \\(a\\) is not zero, \\(z\\) has no choice but to be zero in order to satisfy the second constraint. If \\(z\\) is 0, then \\(tmp\\) should be set to inverse of \\(a\\) in order to satisfy the first constraint. Inverse of \\(a\\) exists, since \\(a\\) is not zero. If \\(a\\) is zero, then the first constraint is reduced to \\(z=1\\).

## Computer programs inside polynomials
