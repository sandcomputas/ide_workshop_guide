---
title: Debugger -> Hva, Hvorfor, Hvordan? 🪲
#toc: true
weight: 998
---

## Hva er en debugger?

**Google:** *a computer program that assists in the detection and correction of errors in other computer programs*


## Hvorfor bruke en debugger? 

Hva er galt med `system.out.println("Her er jeg nå")`?

- Du må rydde opp mye rot når du er ferdig.
- Når du bruker `print()` må du antakelig kjøre koden din *veldig* mange ganger for å sjekke ut verdien på ulike 
  variabler. 
- Med en debugger kan se tilstanden til variabler.
- Du kan ikke kjøre kode snutter for å se hvordan de fungerer - uten å faktisk legge de til i kodebasen (mer rot).
- Debuggeren gjør det lettere å se flyten til applikasjonen (business apps er komplekse og ikke alltid lineære.)

## Eksempler 

```python
async def save_datasett(self, datasett: Datasett) -> Datasett:
    logger.info("Datasett:")
    logger.info(datasett)
    logger.info("Headers:")
    logger.info(self.headers)
    logger.info("URL:")
    logger.info(self.url)
    return self._handle(Datasett, await self.client.post("datasett", json=marshall(datasett)))
```

```python
class AuthMiddleware:

    async def prepare_context_for_request(self, request: Request):
        print("Kom jeg hit?")
        print(f"{request.user}")
        print(f"{request.headers}")
        print(self.auth)
        if not self.auth:
            self.auth = create(Authorizer)
        profile = self.profile(request)
        if request.user.is_anonym():
            print("Det ble true her")
            self.as_anonym(profile)
        else:
            print("Nei, det ble ikke true")
            self.auth.access_as(request.user.id, request.headers, profile)

        print("Kom vi hit da? Pleaase!")

        def user() -> User:
            return request.user

        add_factory(profiles=[profile])(user)

        print(f"{get_factories()}")

        self._setup_amqp(profile)
        print("Yes! Vi kom igjennom hele!")
```

## Hvordan?

To be continued...


