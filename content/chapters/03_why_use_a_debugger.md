---
title: Debugger -> What, why, how? 🪲
#toc: true
weight: 998
---

## What is a debugger?

**Google:** *a computer program that assists in the detection and correction of errors in other computer programs*


## Why use a debugger? 

What is wrong with `system.out.println("Her er jeg nå")`?

- You have to clean up a lot of mess when you are done.
- When using `print()` probably have to run your code *very* many times to inspect different variables.
- You cannot run code snippets to see the effect - without actually adding it to your codebase. 
- It is easier to see the flow of your application (a lot of business applications are complex and not particularly linear.)

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

## How?

To be continued...


