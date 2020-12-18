# EthCon-DORINIC
This is a repository for introducing the "Dorinic" idea of the 2020 Ethcon project.


## Team ETHEREAL 


성신여자대학교 일반대학원 미래융합기술공학과 1학년 윤선우


성신여자대학교 지식서비스공과대학교 4학년 이은영


성신여자대학교 지식서비스공과대학교 4학년 임은지


## Overview of the Project(프로젝트 개요)
>DORINIC, Mobile application for safe storage of Mnemonic
>>1) DORI + Mnemonic: A program that helps Dori (sounds like Dory) remember Mnemonic
>>2) DORI + NICK: Dory from movie ‘Finding Nemo’ & Nick from movie ‘Zootopia’ (similar with fox from MetaMask)


>DORINIC, 니모닉을 안전하게 보관할 수 있는 크롬 확장 프로그램
>>1) DORI + Mnemonic: 도리가 니모닉을 기억할 수 있게 도와주는 프로그램
>>2) DORI + NICK: 니모를 찾아서의 도리와 주토피아 닉(여우-MetaMask)


## Problems
When we create the account, the Mnemonic phrase is generated to protect the private key of the wallet. Mnemonic consists of 12 words to restore the wallet. This phrase should not be leaked to others, so it should be kept and managed in a separate way. However, the online environment always exposes the leakage of clipboard or documents and off-line environments are not useful for managing because of risk of loss. Although the Mnemonic is made of 12 words that can be easily recognized, it is hard to be memorized. In addition, the Mnemonic phrases from entropy become hard to assure confidentiality, because it can be easily exposed and remembered by others.


지갑의 개인 키를 보호하기 위해 계정 생성 시 니모닉(Mnemonic) 문구가 생성된다. 이때, 니모닉이란 지갑을 복구하기 위한 12개의 단어를 말하는데, 이 문구는 타인에게 유출되면 안 되기 때문에 별도의 방법으로 보관하여 관리 해야한다. 그러나 온라인 환경은 클립보드나 문서 취약점 등으로 인한 유출 가능성이 높고, 오프라인 환경은 분실 위험이 크고 관리가 용이하지 않으며, 사용자가 인식하기 쉽게 만든 12 단어이지만 쉽게 기억하기엔 어렵다. 더불어 엔트로피로부터 형성되는 니모닉은 결과적으로 12글자가 타인에게 쉽게 노출 및 기억될 수 있어 기밀성 또한 보장하기 어렵다.


## Final Product


Mobile application


모바일 앱

## Proposed Methodologies


DORINIC will be implemented as a mobile application including OCR function. When we create a wallet, the Mnemonic phrases that consist of 12 words are generated. Mnemonic on the screen is automatically recognized through the OCR function and application’s camera. Subsequently, the extracted text is encrypted through the AES algorithm and stored in a folder within the mobile device. When a user needs to restore a wallet, the stored Mnemonics automatically call it up through biometric recognition by accessing the DORINIC. During the limited time (approximately one minute), mnemonic is exposed on the mobile screen, which allows users to easily restore their wallets even if they don't remember the mnemonic phrase.


## Benefits of the Project


# Convenience
It solves the inconvenience of users writing down their Mnemonic, and helps them not forget their Mnemonic.

# Security
At the same time as reducing the risk of loss, it can also reduce the burden of leakage by reducing the exposure of the plain text of the Mnemonic itself.

# Compatibility
This application can easily be used by generating wallets on any platform.


