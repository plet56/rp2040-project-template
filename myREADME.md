https://reltech.substack.com/p/getting-started-with-rust-on-a-raspberry
https://reltech.substack.com/p/getting-started-with-raspberry-pi



starting ocd requires (the -c command is apparently necessary but wasn't mentioned):

~/src/rust/openocd/src/openocd -f interface/cmsis-dap.cfg -f target/rp2040.cfg -s ./tcl  -c "adapter speed 5000"


Due to setup compilation  and running just need cargo run  after starting openocd above

when in gdb: c c runs  it.