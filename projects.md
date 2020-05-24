---
title: "Academic Projects: Deven Bansod"
---

<style>

h4 {
    margin-bottom: 10px;
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
    margin-left: 0.5%;
}

.mr-1 {
    margin-right: 0.5%;
}

ul, p {
    margin-bottom: 12px;
}

</style>

## Academic Projects

### At Georgia Tech

<!-- #### Implementation-based -->

#### Map-Reduce Infrastructure <a class="pointer ml-1">[Github]</a>

<div class="smaller">
    <span class="intro-sentence">Implemented a library that provides a simplified implementation for <a href="https://static.googleusercontent.com/media/research.google.com/en//archive/mapreduce-osdi04.pdf">MapReduce framework</a> to process large datasets</span>

    <ul style="margin-top: 1%">
        <li>The library automatically parallelizes and executes the user-defined Mapper and Reducer functions on a cluster</li>
        <li>Uses <a href="https://grpc.io/">gRPC</a> and <a href="https://developers.google.com/protocol-buffers">Protocol Buffers</a> to achieve communication between the framework, Master process and the Mapper/Reducer workers</li>
        <li>Provides in-built support for fault tolerance and handles slow straggler workers efficiently, maintaining the overall performance of the MapReduce job</li>
    </ul>
</div>

#### Database System Application for SysLog analysis <a class="pointer ml-1" href="https://github.com/devenbansod/log-data-analysis-db-system">[Github]</a> <a class="pointer ml-1" href="https://docs.google.com/presentation/d/1ZWzANJ9xi8FZeIqD7K0QuEHuY6InUSNafHj6FY9x_mo/edit?usp=sharing">[Slides]</a>

<div class="smaller">
    <span class="intro-sentence">Designed and implemented a database system to enable the efficient forensic analysis on system call audit logs</span>

    <ul style="margin-top: 1%">
        <li>Designed a database system backed by <a href="https://neo4j.com/">Neo4j Graph database</a> for efficient storage and forensic querying of Linux audit logs</li>
        <li>Implemented the online log reduction algorithm proposed by <a href="https://dl.acm.org/doi/10.1145/2976749.2978378">Xu, Zhang, et. al.</a> for the <a href="https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/6/html/security_guide/chap-system_auditing">Linux Audit system</a> that guarantees full forward and backward trackability</li>
        <li>Developed a CLI that supports in-built forensic queries and allows for automatic online ingestion of new logs</li>
    </ul>
</div>

#### Distributed service of store using gRPC and ThreadPool <a class="pointer ml-1">[Github]</a>

<div class="smaller">
    <span class="intro-sentence">Implemented a distributed service of an e-commerce store interfacing multiple clients and vendors</span>

    <ul style="margin-top: 1%">
        <li>Developed a three-layered distributed system comprising of a store with multiple clients and vendors</li>
        <li>The multi-threaded store handles product queries from the clients, queries the vendors for their respective quotes and serves them back to the client using asynchronous RPC calls</li>
        <li>Developed a user-space ThreadPool mini-library to handle multiple client requests concurrently</li>
    </ul>
</div>

#### Virtual Machine Memory coordinator & vCPU scheduler <a class="pointer ml-1">[Github]</a>

<div class="smaller">
    <span class="intro-sentence">Developed a vCPU scheduler and Memory coordinator for guest virtual machines using the <a href="https://libvirt.org/">libvirt API</a></span>

    <ul style="margin-top: 1%">
        <li>Implemented a user-space vCPU scheduler and a memory coordinator to dynamically manage the resources assigned to different virtual (guest) machines on a host</li>
        <li>The scheduler and coordinator collect statistics for each guest machine through hypervisor calls and take appropriate actions to <i>balance</i> CPU and memory assignments each time a predefined interval has passed</li>
    </ul>
</div>

#### FindMyAir <a class="pointer ml-1" href="https://github.com/devenbansod/findmyair">[Github UI]</a><a class="pointer ml-1" href="https://github.com/devenbansod/findmyair-api">[Github API]<a class="pointer ml-1" href="https://drive.google.com/open?id=1V_19Ef73J3FtK-pAJTiZUQqxaKkp6ihh">[Poster]</a><a class="pointer ml-1" href="https://drive.google.com/open?id=1-A8lodZkHr40tcMImCvS67GZS0iH4OGr">[Report]</a>

<div class="smaller">
    <span class="intro-sentence">Demo at: <a href="https://findmyair.herokuapp.com/">https://findmyair.herokuapp.com</a></span>
    <ul></ul>
</div>

#### PE Collective Sensing System (PECSS)

<div class="smaller">
    <span class="intro-sentence">Working with <a href="https://www.cc.gatech.edu/people/rosa-arriaga">Dr. Rosa Arriaga</a>, developed a <a href="https://www.hhs.gov/hipaa/for-professionals/security/laws-regulations/index.html">HIPAA-compliant</a> Android application to augment the <a href="https://www.apa.org/ptsd-guideline/treatments/prolonged-exposure">Prolonged Exposure (PE) therapy</a> for <a href="https://www.nimh.nih.gov/health/topics/post-traumatic-stress-disorder-ptsd/index.shtml">PTSD</a></span>

    <ul style="margin-top: 1%">
        <li>Aimed at PTSD patients undergoing PE therapy, the Android application passively measures their engagement/stress levels, provides a progress platform, and augments the treatment best-practices</li>
        <li>The application, designed to be HIPAA compliant, is built on the principle of "<i>data: encrypted at-rest and encrypted in-flight</i>" and also supports an offline mode of operation</li>
    </ul>
</div>

<hr style="height:1.75px;"/>

<!-- #### Analysis-based -->

#### Barrier synchronization for parallel systems <a class="pointer ml-1">[Github]</a><a class="pointer ml-1" href="https://drive.google.com/open?id=1sArKrOzTHyAM4DCCd74EAFJzzdxqk1O_">[Report]</a>

<div class="smaller">
    <span class="intro-sentence">Implemented various <a href="https://dl.acm.org/doi/10.1145/103727.103729">barrier synchronization algorithms</a> and analyzed their performance on a multicore system, a distributed system and a combination of both</span>

    <ul style="margin-top: 1%">
        <li>Implemented sense-reversing, tree-based, dissemination barriers using OpenMP and MPI parallelization frameworks</li>
        <li>Developed an OpenMP-MPI combined barrier targetting a distributed system consisting of multicore nodes</li>
        <li>Evaluated the performance of these barriers against the native OpenMP and Open MPI barrier implementations</li>
    </ul>
</div>

#### Evaluating Alternative DNS implementations <a class="pointer ml-1" href="https://drive.google.com/open?id=1gDIVREgpcm4uN7M7EuQ_hbcDV4yg4LQl">[Report]</a>

<div class="smaller">
    <span class="intro-sentence">Implemented the domain name service using different transport protocol alternatives: <a href="https://tools.ietf.org/html/rfc8484">HTTPS</a>, <a href="https://tools.ietf.org/html/rfc7858">TLS</a>, <a href="https://tools.ietf.org/id/draft-huitema-quic-dnsoquic-06.html">QUIC</a>, <a href="https://tools.ietf.org/html/rfc6347">DTLS</a> and <a href="https://www.dnscrypt.org/">DNSCrypt</a>, and analyzed their performance and privacy implications through a set of experiments</span>

    <ul style="margin-top: 1%">
        <li>Implemented or setup the alternative DNS implementations, conducted qualitative and quantitative analysis, and evaluated its viability in the current Internet scenario</li>
        <li>The experiments considered the metrics like resolution times, protocol overhead, effect of reusing connections, effect of packet loss while also studying the security implications of privacy provided by these protocols
        </li>
    </ul>
</div>

#### Approximate Query Processing <a class="pointer ml-1" href="https://drive.google.com/open?id=1Y2xW1KG07fvD1nNpsyKqBohYHvlC7cND">[Paper]</a>

<div class="smaller">
    <span class="intro-sentence">Wrote a term paper surveying the area of Approximate Query Processing (AQP) in database systems through its approaches, extensions and applications</span>

    <ul style="margin-top: 1%">
        <li>This survey presents the development of Approximate Query Processing (AQP) over the past couple of decades</li>
        <li>We cover the online (ex. naive sampling, online aggrgation, distinct couting etc.) and the offline (ex. histograms, sketches, wavelets etc.) aggregation approaches to AQP</li>
        <li>We review the modern applications of AQP to spatial data and visual analytics and conclude our discussion outlining the future research opportunities and challenges in the field</li>
    </ul>
</div>

<hr style="height:1.75px;background:#000"/>

### At BITS Pilani

TBD

<hr/>
