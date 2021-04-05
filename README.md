# Advanced Node.js: Scaling Applications

While Node.js is great for creating small apps with minimal surface areas, it was designed to scale.

Learn here sophisticated programming techniques that can help you scale your Node.js applications.

Repo author: [Francis Rodrigues][1]

## Learning objectives

This repo is based on [Alex Banks][2] course, that goes over the scale cube, discussing the different directions in which an app can be scaled:

- Cloning
- The scale cube
- Scaling the x-axis, z-axis, and y-axis
- Forking Node.js processes *(and work with clusters with PM2)*
- Implementing a database instance
- Database scaling
- Setting up horizontal partitioning *(to split data between databases)*
- Decomposing your app into microservices

## Development

For simulating some traffic, uses the `loadtest` package as the following command:

```bash
./node_modules/.bin/loadtest -n 300 http://localhost:3000

[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO Requests: 0 (0%), requests per second: 0, mean latency: 0 ms
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO 
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO Target URL:          http://localhost:3000
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO Max requests:        300
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO Concurrency level:   1
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO Agent:               none
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO 
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO Completed requests:  300
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO Total errors:        300
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO Total time:          0.143740377 s
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO Requests per second: 2087
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO Mean latency:        0.4 ms
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO 
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO Percentage of the requests served within a certain time
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO   50%      1 ms
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO   90%      1 ms
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO   95%      1 ms
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO   99%      1 ms
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO  100%      15 ms (longest request)
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO 
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO  100%      15 ms (longest request)
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO 
[Mon Apr 05 2021 02:40:55 GMT-0300 (Brasilia Standard Time)] INFO    -1:   300 errors
```

## License

MIT

[1]: https://github.com/francisrod01
[2]: https://www.linkedin.com/in/banksalex
