# Soap

Example of SOAP web service whith SpringBoot

## Installation

Run

```bash
./gradlew bootRun
```

## Curl

```bash
curl --location --request POST 'http://localhost:8080/ws' \
--header 'Content-Type: text/xml; charset=utf-8' \
--data-raw '<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
				  xmlns:gs="http://spring.io/guides/gs-producing-web-service">
   <soapenv:Header/>
   <soapenv:Body>
      <gs:getCountryRequest>
         <gs:name>Spain</gs:name>
      </gs:getCountryRequest>
   </soapenv:Body>
</soapenv:Envelope>'
```

