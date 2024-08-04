# Standards, Protocols, and Best Practices

We strictly follow existing standards, protocols, and best practices, and we define our own only if they do not exist.

We adhere to the following guidelines:

1. **Do Standards Exist for What We Want to Do?**  
   - **YES**: If a standard exists, we MUST use it.  
   - **NO**:   
     - We MUST question what we want to use.  
     - We MUST try to find a relevant standard.  
     - We SHOULD rethink the implementation to be able to use existing standards.  

2. **Is There a Library That Does What We Are About to Do?**  
   - If a library exists, we MUST use it.  

3. **Only If All Other Options Have Been Exhausted:**  
   - We MAY implement a new library, but we MUST make sure that if we do, we MUST follow standards, and we MUST be quick in removing our implementation when an existing library is updated to include this feature.  
   - We SHOULD NOT write and maintain any code that already exists or if new code or features come on code we have written, we SHOULD delete our code to use existing libraries in the form of standards or libraries.  

---

## Flow Diagram

Here’s the PlanUML flow diagram based on the above guidelines:

```plantuml
@startuml
title Standards, Protocols, and Best Practices

start

:Do Standards Exist for What We Want to Do?;

if (Standard Exists?) then (yes)
    :Use the Standard;
    stop
else (no)
    :Question What We Want to Use;
    :Try to Find a Relevant Standard;
    :Rethink Implementation to Use Standards;

    if (Relevant Standard Found?) then (yes)
        :Use the Found Standard;
        stop
    else (no)
        :Check for Existing Libraries;

        if (Library Exists?) then (yes)
            :Use the Library;
            stop
        else (no)
            :Implement a New Library;
            :Make Sure to Follow Standards;
            :Be Quick to Remove Implementation When Existing Library is Updated;

            :Avoid Writing and Maintaining Code That Already Exists;
            :Delete Our Code to Use Existing Libraries When New Code or Features Become Available;
            stop
        endif
    endif
endif

@enduml
```
---

## Standards Documentation Links

# Voitto  
- [Voitto Standards](voitto/standards.md)  

# Dooer  
- [Dooer Standards](dooer/standards.md)  

# Roboten  
- [Roboten Standards](roboten/standards.md)  

# K-Star  
- [K-Star Standards](k-star/standards.md)  

# M-Star  
- [M-Star Standards](m-star/standards.md)

---
