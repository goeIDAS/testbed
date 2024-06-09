# eIDAS-Testbed
## What is the goal of the eIDAS-Testbed?
The aim of the **[eIDAS-Testbed](https://test.eID.AS)**, which has been launched within the **[OpenID-Wallet-Plugfest (23.-24. May 2024)](https://gaia-x.eu/tech-x-2024/)**, is to push forward the interoperable implementation of [European Digital Identity Wallets](https://ec.europa.eu/digital-building-blocks/sites/display/EUDIGITALIDENTITYWALLET/EU+Digital+Identity+Wallet+Home) in the sense of Art. 5a [(EU) 2024/1183](https://eur-lex.europa.eu/eli/reg/2024/1183/oj) and similar sorts of [Personal](https://gitlab.eclipse.org/eclipse/xfsc/pcm) or [Organisational](https://gitlab.eclipse.org/eclipse/xfsc/organisational-credential-manager-w-stack) Credential Managers used in the [Gaia-X](https://gaia-x.eu/) domain
(collectively called “**Wallets**”), which are able to handle [Verifiable Credentials](https://en.wikipedia.org/wiki/Verifiable_credentials) according 
to the [W3C Data Model](https://www.w3.org/TR/vc-data-model/) using protocols such as [OpenID for Verifiable Credential Issuance](https://openid.net/specs/openid-4-verifiable-credential-issuance-1_0.html) 
(**OpenID4VCI**) and [OpenID for Verifiable Presentations](https://openid.net/specs/openid-4-verifiable-presentations-1_0.html) (**OpenID4VP**) with a view to the 
current [Architecture Reference Framework](https://github.com/eu-digital-identity-wallet/eudi-doc-architecture-and-reference-framework/blob/main/docs/arf.md) (ARF) and an outlook to application domains,
including the [**Open European Health Data Space**](https://github.com/eu-digital-identity-wallet/eudi-doc-architecture-and-reference-framework/blob/main/docs/arf.md) (EHDS) for example.

## What is currently supported with the eIDAS-Testbed? 
The current functionality and the context of the **[eIDAS-Testbed](https://test.eID.AS)** is outlined in the following figure:

![eIDAS-Testbed](https://github.com/goeIDAS/testbed/assets/78415390/a40a4412-b248-4d2e-b400-9c89cae6c734)

It currently supports 
* the issuance of a Personal Identity Data (PID) attestation according to the current version of the **[PID-Rulebook](https://eu-digital-identity-wallet.github.io/eudi-doc-architecture-and-reference-framework/latest/annexes/annex-3/annex-3.01-pid-rulebook/)**,
* with the latest draft of the **[SD-JWT](https://datatracker.ietf.org/doc/draft-ietf-oauth-selective-disclosure-jwt/)**-format
* using the latest draft of [OpenID for Verifiable Credential Issuance](https://openid.net/specs/openid-4-verifiable-credential-issuance-1_0.html) 
(**OpenID4VCI**, Draft 13 / Implementers Draft 1) using either 
* your personal **eIDAS-means**, if you come from
  *  [Austria](https://ec.europa.eu/digital-building-blocks/sites/display/EIDCOMMUNITY/Austria),
  *  [Germany](https://ec.europa.eu/digital-building-blocks/sites/display/EIDCOMMUNITY/Germany),
  *  [Luxembourg](https://ec.europa.eu/digital-building-blocks/sites/display/EIDCOMMUNITY/Luxembourg),
  *  [Poland](https://ec.europa.eu/digital-building-blocks/sites/display/EIDCOMMUNITY/Poland) or
  * [Slovakia](https://ec.europa.eu/digital-building-blocks/sites/display/EIDCOMMUNITY/Slovakia+-+eID+Scheme), or
* your personal **Test account**, which will be created [upon request](https://www.linkedin.com/in/michael-rauh-0b3218151/), if you come from another region.

Additional functionality will be supported as soon as there are more Wallets and resources to create comprehensive test specification. 
Please do not hesitate to [contact us](https://www.linkedin.com/in/dr-detlef-h%C3%BChnlein-12476439/), if you have any questions, suggestions or if you
want to contribute to the further development of the community-driven eIDAS-Testbed.

## How can I use the eIDAS-Testbed?
Using the eIDAS-Testbed to issue your PID to your wallet consists of the following steps:
1) Providing your identity information via either
   * your *eIDAS-means* or via
   * *login* in to your personal test account
2) Starting your Wallet
3) Retrieving [OpenID Credential Offer](https://openid.net/specs/openid-4-verifiable-credential-issuance-1_0.html#name-credential-offer) via QR-Code (or Link in the future)
4) Let your Wallet perform the PID-issuance according to [OpenID4VCI](https://openid.net/specs/openid-4-verifiable-credential-issuance-1_0.html) and
5) Check whether the PID-attestation has been correctly issued to your Wallet.

Please provide feedback with respect to the results of your tests [here](https://github.com/goeIDAS/testbed/issues) or within LinkedIn. Please make sure to 
include #eIDASTest and [@go_eIDAS Association](https://www.linkedin.com/company/go-eidas-ev/) or [Detlef Hühnlein](https://www.linkedin.com/in/dr-detlef-h%C3%BChnlein-12476439/).

## Successfully tested Wallets so far
The hopefully growing list of successfully tested Wallets so far is as follows:

### [Talao wallet](#talao) (https://talao.io/)

#### Successfully tested version(s):
  
* Version 2.6.0 on [Android](https://play.google.com/store/apps/details?id=co.talao.wallet)

#### Guidance for your own tests

1)	Selecting the appropriate language MAY be helpful (…*/Wallet Settings)
2)	You MUST select …*/Wallet Profiles/OWF Baseline Profile
3)	Visit https://test.eID.AS and use your eID or [reach out to us for other regions]({https://www.linkedin.com/in/dr-detlef-h%C3%BChnlein-12476439/)
4)	Click the “Retrieve Offer” button to display the QR code
5)	Capture the QR code to trigger the issuance of your PID-credential in SD-JWT-format
