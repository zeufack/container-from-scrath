# Containers

When processes run in their own separate namespace, the resource isolation of the namespace ensures that the processes do not affect each other and everyone thinks they are in a separate OS. Such processes can be called containers.

## Namespace

A namespace wraps a global system resource in an abstraction that makes it appear to the processes within the namespace that they have their own isolated instance of the global resource.  Changes to the global resource are visible to other processes that are members of the namespace, but are invisible to other processes. One use of namespaces is to implement containers.

[tutorial](https://www.sobyte.net/post/2022-05/go-linux-container/)

> It is a bad way to try to ubdertend container by comparing it to virtual machine. Container is all about process and ressources sharing. 