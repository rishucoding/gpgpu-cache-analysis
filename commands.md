### Mounting host file system in docker: 
Assume you have a gpgpu-sim diretory which you wish access in the docker. It will mounted in the copy directory.
```sh
docker run -v ~/gpgpu-sim:/root/copy -w /root -it socalucr/gpgpu-sim /bin/bash
```

### Running benchmarks:
1. Create a test directory
2. Copy the gpgpu configurations files for a chosen arch. Copy from "gpgpu-sim_distribution/configs/"
3. Runing a benchmark application: Run the command similar to:
```sh
root@aad2e5c6f20f:~# cat ispass2009-benchmarks/BFS/README.GPGPU-Sim
../bin/release/BFS ./data/graph65536.txt
```
Inside test directory: 
```sh
~/ispass2009-benchmarks/bin/release/BFS ~/ispass2009-benchmarks/BFS/data/graph65536.txt > log
```
