# Virtualization

- One computer can run multiple os.
- Instead of running multiple main services inside one computer we can run multiple os in one computer and run all our services on top of that.
- Virtualization partitions our physical resource into virtual resource.
- Server virtualization, Network Virtualization, Storage Virtualization

```mermaid
flowchart TB
    HW[Hardware]

    HYP[Hypervisor]

    subgraph VM1[Virtual Machine 1]
        OS1[Guest OS]
        A1[App 1]
        A2[App 2]
        OS1 --> A1
        OS1 --> A2
    end

    subgraph VM2[Virtual Machine 2]
        OS2[Guest OS]
        B1[App 1]
        B2[App 2]
        OS2 --> B1
        OS2 --> B2
    end

    HW --> HYP
    HYP --> VM1
    HYP --> VM2
```
