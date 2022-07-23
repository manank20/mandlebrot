# mandlebrot
## About
A multi-threaded mandelbrot set plotter written in rust with crossbeam and rayon scoped threads. The branch non-parallel contains the serial version.
## Usage

```
$ ./mandelbrot <image name> <resolution> <complx number upper left> <complx number lower right>
```

### Usage example

```
$ ./mandelbrot output.png 6000x4000 -0.5,0.65 -1,0.2
```
or
```
$ cargo run --release output.png 6000x4000 -0.5,0.65 -1,0.2   
## make sure you compile with --release, the degug binary is very slow(it takes about 30s as opposed to about 1s in release mode)!
```
### Output
![Sample Output](https://github.com/manank20/mandlebrot/blob/master/sample_outputs/outpt.png)
