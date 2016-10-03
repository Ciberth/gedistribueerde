# Voorbereiding Labo 1: Webservices Java

## WSDL

- What is the name of the provided service?

	* Word Dictionary Web Service

- Which ports have been defined?

	* DictServiceSoap
	* DictServiceSoap12
	* DictServiceHttpGet
	* DictServiceHttpPost

- Which transmit protocol uses the DictServiceSoap-binding?

	* HTTP

- Which operations are defined in the DictServiceSoap-binding?

	* ServerInfo
	* DictionaryList
	* DictionaryListExtended
	* DictionaryInfo
	* Define
	* DefineInDict
	* StrategyList
	* Match
	* MatchInDict

- What are the parameters expected in the operation MatchInDict?

```xml
	<s:element name="MatchInDict">
	<s:complexType>
	<s:sequence>
	<s:element minOccurs="0" maxOccurs="1" name="dictId" type="s:string"/>
	<s:element minOccurs="0" maxOccurs="1" name="word" type="s:string"/>
	<s:element minOccurs="0" maxOccurs="1" name="strategy" type="s:string"/>
	</s:sequence>
	</s:complexType>
	</s:element>
```

	* dictId (string)
	* word (string)
	* strategy (string)

- What does the operation MatchInDict returns?


```xml
	<s:element name="MatchInDictResponse">
	<s:complexType>
	<s:sequence>
	<s:element minOccurs="0" maxOccurs="1" name="MatchInDictResult" type="tns:ArrayOfDictionaryWord"/>
	</s:sequence>
	</s:complexType>
	</s:element>
```

