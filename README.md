# go-amqp-reconnect
This is a wrapper for this rabbitmq client https://github.com/rabbitmq/amqp091-go to allow rabbitmq client to reconnect when there are any connectivity issue between consumer and broker
This is a carbon copy based on [isayme](https://github.com/isayme/go-amqp-reconnect) which based on streadway RabbitMQ client implementation

## How to change existing code
1. add import `import "github.com/kitabisa/go-amqp-reconnect/rabbitmq"`
2. Replace `amqp.Connection`/`amqp.Channel` with `rabbitmq.Connection`/`rabbitmq.Channel`!

## Example
### Close by developer
> go run example/close/demo.go

### Auto reconnect
> go run example/reconnect/demo.go

