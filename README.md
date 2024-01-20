<h1 align="center">File Permissions - UNIX </h1>

In Unix-like operating systems, file permissions are represented by a three-digit octal (base-8) number. Each digit corresponds to a specific set of permissions for the owner, group, and others. Here's the breakdown:

-   **Read (r): 4**
-   **Write (w): 2**
-   **Execute (x): 1**

Now, each digit in the three-digit octal number represents the permission set for a specific entity:

1.  **Owner (User):**

    -   Read (r): 4
    -   Write (w): 2
    -   Execute (x): 1
2.  **Group:**

    -   Read (r): 4
    -   Write (w): 2
    -   Execute (x): 1
3.  **Others:**

    -   Read (r): 4
    -   Write (w): 2
    -   Execute (x): 1

So, when you see a three-digit octal number like 755:

-   The leftmost digit (7) represents the permissions for the owner.

    -   7 = 4 (read) + 2 (write) + 1 (execute): read, write, and execute.
-   The middle digit (5) represents the permissions for the group.

    -   5 = 4 (read) + 1 (execute): read and execute.
-   The rightmost digit (5) represents the permissions for others.

    -   5 = 4 (read) + 1 (execute): read and execute.

Here are a few examples:

-   **755**: Read, write, and execute for the owner; read and execute for the group and others.
-   **644**: Read and write for the owner; read-only for the group and others.
-   **700**: Read, write, and execute for the owner; no permissions for the group and others.

These octal permissions are often used with the `chmod` command to set or modify file permissions.
