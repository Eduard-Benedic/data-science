## Key objectives at the heart of computer security

* Confidentiality
  * Data Confidentiality - data not disclosed to unathorized individuals
  * Privacy - individuals control what information is disclosed about them
* Integrity
* Availability

CIA

## A model for Computer Security

System resource (asset) can be:
* Hardware
* Software
* Data
* Communication facilities and networks

Categories of vulnerabilities
* **corrupted** - does the wrong thing or gives wrong answers
* **leaky** - unathorized people have partly or total access to data or system
* **unavailable** - very slow, the system becomes impractical

Attack - a threat carried out
**Thret agent** - attacker

## Security Design Principles

### Echonomy of mechanism
The design of security measures in hardware and software should be as simple as possible

### Fail-safe default
The default situation is lack of access

### Complete mediation
Every access must be checked against the access control mechanism.

### Open design
The design of a security mechanism should be open rather than seceret.

### Separation of privilege
Multiple privilege attributes are required to achieve access (Multifactor user authentication)

### Least privilege
Every process and every user of the system should operate using the least set of privileges necessary to perform the task.

### Least common mechanism
The design should minimize the functions shared by different users, providing mutual security

## Psychological acceptability

## Computer Security Strategy
* Specification/policy
* Implementation/mechanisms
* Correctness/assurance