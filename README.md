<div align="center">
<img src="https://github.com/fastify/graphics/raw/master/full-logo.png" width="650" height="auto"/>
</div>

<div align="center">

[![Build Status](https://travis-ci.org/fastify/fastify.svg?branch=master)](https://travis-ci.org/fastify/fastify)
[![Coverage Status](https://coveralls.io/repos/github/fastify/fastify/badge.svg?branch=master)](https://coveralls.io/github/fastify/fastify?branch=master)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](http://standardjs.com/)
[![NPM version](https://img.shields.io/npm/v/fastify.svg?style=flat)](https://www.npmjs.com/package/fastify)
[![NPM downloads](https://img.shields.io/npm/dm/fastify.svg?style=flat)](https://www.npmjs.com/package/fastify) [![Gitter](https://badges.gitter.im/gitterHQ/gitter.svg)](https://gitter.im/fastify)
</div>
<br />

# TL;DR

* [Fastify](https://github.com/fastify/fastify) is, fast and low overhead web framework for Node.js
* This package shows how fast it is comparatively.

# Installing

```
npm i -g fastify-benchmarks
```

# Usage

```
benchmark [arguments (optional)]
```

#### Arguments

* `-h`: Help on how to use the tool.
* `compare`: Get comparative data for your benchmarks.

> You may also compare all test results, at once, in a single table; `benchmark compare -t`

> You can also extend the comparison table with percentage values based on fastest result; `benchmark compare -p`
# Benchmarks
* __Machine:__ Linux fv-az60 5.3.0-1020-azure #21~18.04.1-Ubuntu SMP Wed Apr 15 09:35:56 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.16.3`
* __Run:__ Mon Jun  1 00:49:14 UTC 2020

|                          | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:    | :-:        | --:     | --:           |
| bare                     | ✗      | 35665.2    | 2.70    | 5.58          |
| connect-router           | ✓      | 30748.0    | 3.15    | 4.81          |
| connect                  | ✗      | 34727.6    | 2.78    | 5.43          |
| egg.js                   | ✓      | 12201.0    | 8.11    | 4.03          |
| express-route-prefix     | ✓      | 19420.7    | 5.03    | 6.76          |
| express-with-middlewares | ✓      | 14751.2    | 6.67    | 5.33          |
| express                  | ✓      | 18485.9    | 5.31    | 2.89          |
| fastify-big-json         | ✓      | 8006.0     | 12.34   | 91.92         |
| fastify                  | ✓      | 34420.0    | 2.81    | 5.38          |
| foxify                   | ✓      | 36810.8    | 2.62    | 5.23          |
| hapi                     | ✓      | 17639.3    | 5.60    | 2.76          |
| koa-router               | ✓      | 23255.3    | 4.21    | 3.64          |
| koa                      | ✗      | 27139.2    | 3.59    | 4.24          |
| micro-route              | ✓      | 31874.8    | 3.04    | 4.99          |
| micro                    | ✗      | 35349.0    | 2.73    | 5.53          |
| microrouter              | ✓      | 18789.6    | 5.22    | 2.94          |
| polka                    | ✓      | 36479.8    | 2.64    | 5.71          |
| polkadot                 | ✗      | 40844.0    | 2.33    | 6.39          |
| rayo                     | ✓      | 33820.0    | 2.86    | 5.29          |
| restify                  | ✓      | 24021.2    | 4.07    | 3.80          |
| server-base-router       | ✓      | 31713.4    | 3.05    | 4.96          |
| server-base              | ✗      | 31344.6    | 3.09    | 4.90          |
| spirit-router            | ✓      | 32403.6    | 2.78    | 5.07          |
| spirit                   | ✗      | 33324.8    | 2.70    | 5.21          |
| take-five                | ✓      | 0.0        | 0.00    | 0.00          |
| total.js                 | ✓      | 22536.0    | 4.33    | 6.40          |
| trek-engine              | ✗      | 27642.8    | 3.53    | 3.93          |
| trek-router              | ✓      | 30367.8    | 3.20    | 4.31          |
| vapr                     | ✓      | 23944.8    | 4.07    | 3.40          |
| yeps-router              | ✓      | 27737.6    | 3.51    | 4.34          |
| yeps                     | ✗      | 32828.8    | 2.95    | 5.13          |
