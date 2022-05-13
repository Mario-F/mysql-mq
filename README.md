# MySQL Message Queue

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate?hosted_button_id=34NHCDNHRRV6G)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)
![GitHub issues](https://img.shields.io/github/issues/Mario-F/mysql_mq)
[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/mario-f/mysql_mq.svg)](http://isitmaintained.com/project/mario-f/mysql_mq "Average time to resolve an issue")
[![Percentage of issues still open](http://isitmaintained.com/badge/open/mario-f/mysql_mq.svg)](http://isitmaintained.com/project/mario-f/mysql_mq "Percentage of issues still open")

mysql-mq provides a message queueing service based on mysql.

Its not build to down to performance, either its optimized to provide a mysql backed message queue if no other queueing service is available or would be oversized for your application.

## Install

```shell
npm install mysql-mq
```

## Usage

A queue will automatically created when not exists, this create process can be called manually with the "init" method or is executed on first usage of the queue.

### Example usage

```javascript
var mmq = require("mysql-mq");
var testQueue = new mmq('mmq_test', { database: 'mp_example' });

testQueue.put('This is a Test!').then((res) => {
    console.log('Message got ID:', res)

    testQueue.get().then((res) => {
        console.log('Content of Message ID', res.id_message, res.message)

        testQueue.delete(res.id_message).then((res) => {
            console.log('Message deleted')
        })
    })
})
```

## Development

Feel free to fork & contribute!

### Testing

Tests need a MySQL Server running, to simplify tests a docker environment can be used. (You need to have docker installed)

Test with docker:

```shell
npm run dockertest
```

Clear all docker containers:

```shell
npm run dockerend
```
