# EthCon-DORINIC
This is a repository for introducing the "Dorinic" idea of the 2020 Ethcon project.


##Overview of the Project
>DORINIC, Mobile application for safe storage of Mnemonic
>>1) DORI + Mnemonic: A program that helps Dori (sounds like Dory) remember Mnemonic
>>2) DORI + NICK: Dory from movie ‘Finding Nemo’ & Nick from movie ‘Zootopia’ (similar with fox from MetaMask)

##Problems
When we create the account, the Mnemonic phrase is generated to protect the private key of the wallet. Mnemonic consists of 12 words to restore the wallet. This phrase should not be leaked to others, so it should be kept and managed in a separate way. However, the online environment always exposes the leakage of clipboard or documents and off-line environments are not useful for managing because of risk of loss. Although the Mnemonic is made of 12 words that can be easily recognized, it is hard to be memorized. In addition, the Mnemonic phrases from entropy become hard to assure confidentiality, because it can be easily exposed and remembered by others.

##Final Product
Mobile application

##Proposed Methodologies
DORINIC will be implemented as a mobile application including OCR function. When we create a wallet, the Mnemonic phrases that consist of 12 words are generated. Mnemonic on the screen is automatically recognized through the OCR function and application’s camera. Subsequently, the extracted text is encrypted through the AES algorithm and stored in a folder within the mobile device. When a user needs to restore a wallet, the stored Mnemonics automatically call it up through biometric recognition by accessing the DORINIC. During the limited time (approximately one minute), mnemonic is exposed on the mobile screen, which allows users to easily restore their wallets even if they don't remember the mnemonic phrase.


##Benefits of the Project
>>Convenience
It solves the inconvenience of users writing down their Mnemonic, and helps them not forget their Mnemonic.

>>Security
At the same time as reducing the risk of loss, it can also reduce the burden of leakage by reducing the exposure of the plain text of the Mnemonic itself.

>>Compatibility
This application can easily be used by generating wallets on any platform.


