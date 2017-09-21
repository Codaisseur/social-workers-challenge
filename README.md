# Social Workers

A challenge to build social workers on top of RabbitMQ.

## Getting Started

Clone the repo, run `bundle install`.

Check Slack for the `RABBITMQ_URL` and run the example:

```bash
RABBITMQ_URL=... ./example $(whoami)
```

## Challenges

Build some Social Workers

  - Find a (random?) friend
  - Say hi to someone (specific)
  - Say hi to everyone
  - Assassin (kill one by one)
  - Terrorist (kill all at once)

Implement the workers and the actions

  - join room / leave room on init/exit
  - send friend request + accept (personal / random) friend request
  - say (personal / random) hi + respond to (personal / random) hi
  - say hi to all
  - kill one other + die on receive kill
  - kill all others and yourself

**NOTE**: Use JSON to serialize complex messages! (don't forget to
`require 'json'` in your code)
