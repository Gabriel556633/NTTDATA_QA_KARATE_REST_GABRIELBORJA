
# TEST GABRIEL BORJA KARATE NTTDATA QA

Desarrolle el test solicitado realizando los siguientes pasos.


    





- Según el email recibido se deben hacer pruebas con un manejador o cliente que realice consultas REST, en mi caso utilizado KARATE  se adjunta en el Repositorio la coleccion de infomracin con los respectivos endpoints.

-Los metodos del TEST son los siguientes con su respectivo body:

Feature: Login User
  Scenario: Login User FAIL
    Given url "https://api.demoblaze.com/login"
    And request {  "username":"Gabriel", "password":"123456" }
    When method post
    Then status 200

Feature: Login User
  Scenario: Login User OK
    Given url "https://api.demoblaze.com/login"
    And request {  "username":"GabrielBorjaMoscoso", "password":"123456" }
    When method post
    Then status 200

Feature: SignUp User
  Scenario: SignUp User FAIL
    Given url "https://api.demoblaze.com/signup"
    And request {  "username":"GabrielBorjaMoscoso", "password":"123456" }
    When method post
    Then status 200







