# Concurrency is not parallelism

## Literature Notes

### Concurrency vs Parallelism

- Go is a concurrent language
- **Concurrency is the composition of independently executing processes**
- **Parallelism is the simultaneous execution of things** (which may be related)
- It's possible to make existing processes faster by adding concurrency to the design
- You can parallelise an existing concurrent process

### Goroutines

- Goroutines are defined by the keyboard `go`
- Goroutines are **not** threads
- Goroutines are multiplexed onto the OS' threads as required
- A blocked goroutine will not block other goroutines

### Select statemnet

- A `select` statement is like a `switch` statement but for communications
  - A `case` is chosen based on the `channel` that is ready to be unloaded

## Ideas

1. Build simple load balancer to calculate sum of factorials using the help of workers as seen around [slide 39](https://go.dev/talks/2012/waza.slide#39)
2. Think of something cool to implement the practical load balancer as seen in [slide 45](https://go.dev/talks/2012/waza.slide#45)
3. Implement Query replicated database exercise on similar databases as seen in [slide 56](https://go.dev/talks/2012/waza.slide#56)

## Appendix

<ol type="A">
  <li><a href="https://go.dev/talks/2012/waza.slide">Slide Deck</a></li>
</ol>
