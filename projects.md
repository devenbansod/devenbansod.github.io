---
title: "Academic Projects: Deven Bansod"
---

<style>

h5 {
    margin-bottom: 12px;
}

.smaller {
    font-size: 0.82rem;
}

.float-right {
  float: right;
}

.pointer {
    cursor: pointer;
}

.hide {
    display: none;
}

.intro-sentence {
    margin-bottom: 20%;
}

.ml-1 {
    margin-left: 1%;
}

.mr-1 {
    margin-right: 1%;
}

ul, p {
    margin-bottom: 12px;
}

</style>

## Academic Projects

### At Georgia Tech

#### Implementation-based

##### Map-Reduce Infrastructure <a class="pointer ml-1">[Github]</a>

<div class="smaller">
    <span class="intro-sentence">Implemented a library that provides a simplified implementation for <a href="https://static.googleusercontent.com/media/research.google.com/en//archive/mapreduce-osdi04.pdf">MapReduce framework</a> to process large datasets.</span>

    <ul style="margin-top: 1%">
        <li>The library automatically parallelizes and executes the user-defined Mapper and Reducer functions on a cluster</li>
        <li>Used <a href="https://grpc.io/">gRPC</a> and <a href="https://developers.google.com/protocol-buffers">Protocol Buffers</a> to achieve communication between the framework, Master process and the Mapper/Reducer workers</li>
        <li>The library also provides in-built support for fault tolerance and handles slow straggler workers efficiently, maintaining the overall performance of the MapReduce job</li>
    </ul>
</div>

##### Database System Application for SysLog analysis

<div class="smaller">
<p>TBD</p>
</div>

##### Distributed service of store using gRPC and ThreadPool <a class="pointer ml-1">[Github]</a>

<div class="smaller">
    <span class="intro-sentence">Implemented a distributed service of an e-commerce store interfacing multiple clients and vendors.</span>

    <ul style="margin-top: 1%">
        <li>Developed a three-layered distributed system comprising of a store with multiple clients and vendors.</li>
        <li>The multi-threaded store processes product queries from the clients, queries the vendors for their respective quotes and serves them back to the client using asynchronous RPC calls.</li>
        <li>Uses a self-developed user-space ThreadPool mini-library to handle multiple client requests concurrently.</li>
    </ul>
</div>

##### Virtual Machine Manager: Memory coordinator and vCPU scheduler <a class="pointer ml-1">[Github]</a>

<div class="smaller">
    <span>Developed a vCPU scheduler and Memory coordinator for guest virtual machines using the <a href="https://libvirt.org/">libvirt API</a>.</span>

    <ul>
        <li>Implemented a user-space vCPU scheduler and a memory coordinator to dynamically manage the resources assigned to different virtual (guest) machines.</li>
        <li>The scheduler and coordinator collect statistics for each guest machine through hypervisor calls and take appropriate actions to <i>balance</i> CPU and memory assignments each time a predefined interval has passed.</li>
    </ul>
</div>

##### FindMyAir

TBD


##### PECSS

TBD

<hr style="height:1.75px;"/>

#### Analysis-based

##### Barrier synchronization for parallel systems <a class="pointer ml-1">[Github]</a><a class="pointer ml-1">[Report]</a>

<div class="smaller">
    <span class="intro-sentence">Implemented various <a href="https://dl.acm.org/doi/10.1145/103727.103729">barrier synchronization algorithms</a> and analyzed their performance on a multicore system, a distributed system and a combination of both.</span>

    <ul style="margin-top: 1%">
        <li>Implemented sense-reversing, tree-based, dissemination barriers using OpenMP and MPI parallelization frameworks</li>
        <li>Developed a OpenMP-MPI combined barrier targetting a distributed system consisting of multicore nodes</li>
        <li>Evaluated the performance of these barriers against the native OpenMP and Open MPI barrier implementations.</li>
    </ul>
</div>

##### DNS transport

TBD

##### Approximate Query Processing

TBD

<hr style="height:1.75px;background:#000"/>

### At BITS Pilani

TBD

<hr/>
