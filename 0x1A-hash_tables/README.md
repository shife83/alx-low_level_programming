Project: 0x1A. C - Hash Tables

This project implements a hash table data structure in C, providing efficient key-value pair storage and retrieval.

Features:

Dynamic Hash Table Creation: Creates hash tables with a user-specified size, adapting to your data requirements.
Optimized Key-Value Pairing: Stores key-value pairs using strings for keys and strings for values, ensuring compatibility with common use cases.
Hash Function: Employs a basic hash function to map keys to unique indices within the hash table, enabling efficient lookup.
Collision Resolution (Linear Probing): Handles collisions (when different keys map to the same index) using linear probing, searching for an available slot in the hash table.
Essential Hash Table Operations:
hash_table_t *hash_table_create(unsigned long int size): Allocates memory and initializes a hash table of the specified size.
int hash_table_set(hash_table_t *ht, const char *key, const char *value): Inserts a key-value pair into the hash table, handling potential collisions.
char *hash_table_get(hash_table_t *ht, const char *key): Retrieves the value associated with the given key, returning NULL if not found.
int hash_table_delete(hash_table_t *ht, const char *key): Removes a key-value pair from the hash table, adjusting the table if necessary.
void hash_table_destroy(hash_table_t *ht): Deallocates memory associated with the hash table.
