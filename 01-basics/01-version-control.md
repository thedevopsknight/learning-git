# Version Control System

## Definition

- Version Control System (VCS) is a software tool that helps manage changes to source code over time. 

## Features

- It keeps track of every modification to the code in a special kind of database.
- It is also known as Source Control Management(SCM) tool or Revision Control System(RCS).
- It is independent of the kind of project / technology / framework

## Advantages 

- **Collaboration**:
    - Multiple developers can work on the same project simultaneously without interfering with each other’s work. 
    - Changes can be integrated smoothly, and conflicts can be resolved systematically.
- **History and Backup**:
    - Every change is recorded along with who made the change and why. 
    - This historical context is invaluable for understanding how the project has evolved. 
    - It also acts as a backup mechanism.
- **Branching and Merging**:
    - Features, fixes, and experiments can be developed in parallel in separate branches.
    - Merging these branches can integrate these developments into the main codebase.
- **Traceability**:
    - Every change is logged, which helps in tracking down bugs by examining when and where they were introduced.
- **Reverting Changes**:
    - If a mistake is made, it's easy to revert back to a previous version of the code, minimizing the impact of errors.

## Types

### Local Version Control System

- These are simple databases that keep track of changes to files on the local system. 
- An example is RCS (Revision Control System).

### Centralized Version Control System

- These systems have a single server that contains all the versioned files, and a number of clients that check out files from that central place
- Examples include CVS (Concurrent Versions System) and Subversion (SVN).

### Distributed Version Control Systems (DVCS)

- In a DVCS, clients don’t just check out the latest snapshot of the files; they fully mirror the repository, including its full history.
- Examples include Git, Mercurial, and Bazaar.

### Comparing CVCS and DVCS

| Aspect                      | CVCS                                     | DVCS                                        |
| --------------------------- | ---------------------------------------- | ------------------------------------------- |
| **Repository Model**        | Centralized                              | Distributed                                 |
| **Network Dependency**      | High (for most operations)               | Low (most operations are local)             |
| **Single Point of Failure** | Yes                                      | No                                          |
| **Speed**                   | Slower due to network dependency         | Faster due to local operations              |
| **Offline Capabilities**    | Limited                                  | Extensive                                   |
| **Branching/Merging**       | More challenging                         | Easier and more flexible                    |
| **Backup**                  | Central server backup needed             | Each clone acts as a backup                 |
| **Scalability**             | Limited by central server capacity       | Better scalability for large projects       |
| **Learning Curve**          | Easier to grasp for beginners            | Steeper learning curve for beginners        |
| **Security**                | Easier to manage centralized security    | More complex as each clone has full history |
| **Collaboration**           | Centralized, simpler to manage           | More flexible, supports various workflows   |
| **Performance Bottlenecks** | Network latency and server load          | Minimal, as operations are local            |
| **Administrative Control**  | Centralized, simpler to enforce policies | Decentralized, more complex to manage       |
